# Comparing `tmp/yet_another_wizz-2.4.tar.gz` & `tmp/yet_another_wizz-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yet_another_wizz-2.4.tar", last modified: Sat Jul  8 22:00:57 2023, max compression
+gzip compressed data, was "yet_another_wizz-2.5.tar", last modified: Sun Jul  9 16:12:24 2023, max compression
```

## Comparing `yet_another_wizz-2.4.tar` & `yet_another_wizz-2.5.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:57.558508 yet_another_wizz-2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-08 22:00:57.558508 yet_another_wizz-2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:57.542508 yet_another_wizz-2.4/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      107 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/bin/yaw
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-08 22:00:57.558508 yet_another_wizz-2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:57.542508 yet_another_wizz-2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:57.542508 yet_another_wizz-2.4/src/yaw/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:57.546508 yet_another_wizz-2.4/src/yaw/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/catalogs/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/catalogs/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/catalogs/linkage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:57.546508 yet_another_wizz-2.4/src/yaw/catalogs/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/catalogs/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/catalogs/scipy/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/catalogs/scipy/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/catalogs/scipy/patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:57.546508 yet_another_wizz-2.4/src/yaw/catalogs/treecorr/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/catalogs/treecorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/catalogs/treecorr/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:57.550508 yet_another_wizz-2.4/src/yaw/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/config/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/config/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)    14657 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/config/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/config/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/config/resampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/config/scales.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:57.550508 yet_another_wizz-2.4/src/yaw/core/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/core/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/core/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/core/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/core/cosmology.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/core/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/core/math.c
--rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/core/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/core/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:57.554509 yet_another_wizz-2.4/src/yaw/correlation/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/correlation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40621 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/correlation/corrfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/correlation/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)    41926 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/correlation/paircounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:57.554509 yet_another_wizz-2.4/src/yaw/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   129479 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/examples/auto_reference.hdf
--rw-r--r--   0 runner    (1001) docker     (123)   123032 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/examples/auto_unknown_1.hdf
--rw-r--r--   0 runner    (1001) docker     (123)   100475 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/examples/cross_1.hdf
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)    22441 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw/redshifts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:57.554509 yet_another_wizz-2.4/src/yaw_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:57.554509 yet_another_wizz-2.4/src/yaw_cli/commandline/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw_cli/commandline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw_cli/commandline/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    17350 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw_cli/commandline/subcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw_cli/commandline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:57.558508 yet_another_wizz-2.4/src/yaw_cli/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw_cli/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17836 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw_cli/pipeline/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw_cli/pipeline/default_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw_cli/pipeline/directories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw_cli/pipeline/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw_cli/pipeline/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw_cli/pipeline/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    16034 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw_cli/pipeline/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw_cli/pipeline/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-07-08 21:58:49.000000 yet_another_wizz-2.4/src/yaw_cli/pipeline/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:57.558508 yet_another_wizz-2.4/src/yet_another_wizz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-08 22:00:57.000000 yet_another_wizz-2.4/src/yet_another_wizz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-08 22:00:57.000000 yet_another_wizz-2.4/src/yet_another_wizz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:00:57.000000 yet_another_wizz-2.4/src/yet_another_wizz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-08 22:00:57.000000 yet_another_wizz-2.4/src/yet_another_wizz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-08 22:00:57.000000 yet_another_wizz-2.4/src/yet_another_wizz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.595285 yet_another_wizz-2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-09 16:12:24.595285 yet_another_wizz-2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 16:12:24.595285 yet_another_wizz-2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.563283 yet_another_wizz-2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.563283 yet_another_wizz-2.5/src/yaw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.567283 yet_another_wizz-2.5/src/yaw/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/linkage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.567283 yet_another_wizz-2.5/src/yaw/catalogs/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/scipy/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/scipy/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/scipy/patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.571283 yet_another_wizz-2.5/src/yaw/catalogs/treecorr/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/treecorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/catalogs/treecorr/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.575284 yet_another_wizz-2.5/src/yaw/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14657 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/resampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/scales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.579284 yet_another_wizz-2.5/src/yaw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/math.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.579284 yet_another_wizz-2.5/src/yaw/correlation/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/correlation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40621 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/correlation/corrfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/correlation/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41926 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/correlation/paircounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.583284 yet_another_wizz-2.5/src/yaw/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129479 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/examples/auto_reference.hdf
+-rw-r--r--   0 runner    (1001) docker     (123)   123032 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/examples/auto_unknown_1.hdf
+-rw-r--r--   0 runner    (1001) docker     (123)   100475 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/examples/cross_1.hdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22441 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw/redshifts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.583284 yet_another_wizz-2.5/src/yaw_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.587284 yet_another_wizz-2.5/src/yaw_cli/commandline/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/commandline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/commandline/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/commandline/subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/commandline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.591284 yet_another_wizz-2.5/src/yaw_cli/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17836 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/default_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16034 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15241 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-07-09 16:10:21.000000 yet_another_wizz-2.5/src/yaw_cli/pipeline/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:12:24.591284 yet_another_wizz-2.5/src/yet_another_wizz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-09 16:12:24.000000 yet_another_wizz-2.5/src/yet_another_wizz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-09 16:12:24.000000 yet_another_wizz-2.5/src/yet_another_wizz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 16:12:24.000000 yet_another_wizz-2.5/src/yet_another_wizz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-09 16:12:24.000000 yet_another_wizz-2.5/src/yet_another_wizz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-09 16:12:24.000000 yet_another_wizz-2.5/src/yet_another_wizz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-09 16:12:24.000000 yet_another_wizz-2.5/src/yet_another_wizz.egg-info/top_level.txt
```

### Comparing `yet_another_wizz-2.4/README.rst` & `yet_another_wizz-2.5/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -24,24 +24,24 @@
 Installation
 ------------
 
 The yet_another_wizz package can be installed directly with pip::
 
     pip install yet_another_wizz
 
-This will install the python package ``yaw``, as well as the ``yaw`` executable
-command line tool.
+This will install the python package ``yaw``, as well as the ``yaw_cli``
+executable command line tool.
 
 
 Usage
 -----
 
 There are two main ways to use yet_another_wizz,
 
-- the ``yaw`` commmand line tool and
+- the ``yaw_cli`` commmand line tool and
 - the python package ``yaw`` directly.
 
 Most people will probably get started with the command line tool, which should
 cover all necessary tasks for a standard clustering redshift calibration. For
 custom solutions, use the python package. A basic example as well as the API
 reference can be found in the official documentation.
```

### Comparing `yet_another_wizz-2.4/src/yaw/__init__.py` & `yet_another_wizz-2.5/src/yaw/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 measurement of the correlation amplitude, introduced by Schmidt et al. (2013,
 `arXiv:1303.0292 <https://arxiv.org/abs/1303.0292>`_).
 
 Author: Jan Luca van den Busch
         (Ruhr-Universität Bochum, Astronomisches Institut)
 """
 
-__version__ = "2.4"
+__version__ = "2.5"
 
 import logging as _logging
 
 _logging.getLogger(__name__).addHandler(_logging.NullHandler())
 
 
 from yaw.catalogs import NewCatalog
```

### Comparing `yet_another_wizz-2.4/src/yaw/catalogs/__init__.py` & `yet_another_wizz-2.5/src/yaw/catalogs/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/catalogs/catalog.py` & `yet_another_wizz-2.5/src/yaw/catalogs/catalog.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/catalogs/factory.py` & `yet_another_wizz-2.5/src/yaw/catalogs/factory.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/catalogs/linkage.py` & `yet_another_wizz-2.5/src/yaw/catalogs/linkage.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/catalogs/scipy/catalog.py` & `yet_another_wizz-2.5/src/yaw/catalogs/scipy/catalog.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/catalogs/scipy/kdtree.py` & `yet_another_wizz-2.5/src/yaw/catalogs/scipy/kdtree.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/catalogs/scipy/patches.py` & `yet_another_wizz-2.5/src/yaw/catalogs/scipy/patches.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/catalogs/treecorr/catalog.py` & `yet_another_wizz-2.5/src/yaw/catalogs/treecorr/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import itertools
 import os
 import sys
 from collections.abc import Iterator
-from typing import TYPE_CHECKING, NoReturn
+from typing import TYPE_CHECKING, Dict, NoReturn, Tuple
 try:  # pragma: no cover
     from typing import TypeAlias
 except ImportError:  # pragma: no cover
     from typing_extensions import TypeAlias
 
 import numpy as np
 import pandas as pd
@@ -24,15 +24,15 @@
 from yaw.redshifts import HistData
 
 if TYPE_CHECKING:  # pragma: no cover
     from pandas import DataFrame, Interval
     from yaw.catalogs import PatchLinkage
 
 
-TypeNNResult: TypeAlias = dict[tuple[int, int], NNCorrelation]
+TypeNNResult: TypeAlias = Dict[Tuple[int, int], NNCorrelation]  # supports py3.8
 
 
 def _iter_bin_masks(
     data: NDArray,
     bins: NDArray,
     closed: str = "left"
 ) -> Iterator[tuple[Interval, NDArray[np.bool_]]]:
```

### Comparing `yet_another_wizz-2.4/src/yaw/config/__init__.py` & `yet_another_wizz-2.5/src/yaw/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/config/backend.py` & `yet_another_wizz-2.5/src/yaw/config/backend.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/config/binning.py` & `yet_another_wizz-2.5/src/yaw/config/binning.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/config/config.py` & `yet_another_wizz-2.5/src/yaw/config/config.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/config/default.py` & `yet_another_wizz-2.5/src/yaw/config/default.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/config/options.py` & `yet_another_wizz-2.5/src/yaw/config/options.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/config/resampling.py` & `yet_another_wizz-2.5/src/yaw/config/resampling.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/config/scales.py` & `yet_another_wizz-2.5/src/yaw/config/scales.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/config/utils.py` & `yet_another_wizz-2.5/src/yaw/config/utils.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/core/__init__.py` & `yet_another_wizz-2.5/src/yaw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/core/abc.py` & `yet_another_wizz-2.5/src/yaw/core/abc.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/core/containers.py` & `yet_another_wizz-2.5/src/yaw/core/containers.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/core/coordinates.py` & `yet_another_wizz-2.5/src/yaw/core/coordinates.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/core/cosmology.py` & `yet_another_wizz-2.5/src/yaw/core/cosmology.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/core/docs.py` & `yet_another_wizz-2.5/src/yaw/core/docs.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/core/logging.py` & `yet_another_wizz-2.5/src/yaw/core/logging.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/core/math.c` & `yet_another_wizz-2.5/src/yaw/core/math.c`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/core/math.py` & `yet_another_wizz-2.5/src/yaw/core/math.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/core/parallel.py` & `yet_another_wizz-2.5/src/yaw/core/parallel.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/core/utils.py` & `yet_another_wizz-2.5/src/yaw/core/utils.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/correlation/__init__.py` & `yet_another_wizz-2.5/src/yaw/correlation/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/correlation/corrfuncs.py` & `yet_another_wizz-2.5/src/yaw/correlation/corrfuncs.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/correlation/estimators.py` & `yet_another_wizz-2.5/src/yaw/correlation/estimators.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/correlation/paircounts.py` & `yet_another_wizz-2.5/src/yaw/correlation/paircounts.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/deprecated.py` & `yet_another_wizz-2.5/src/yaw/deprecated.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/examples/__init__.py` & `yet_another_wizz-2.5/src/yaw/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/examples/auto_reference.hdf` & `yet_another_wizz-2.5/src/yaw/examples/auto_reference.hdf`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/examples/auto_unknown_1.hdf` & `yet_another_wizz-2.5/src/yaw/examples/auto_unknown_1.hdf`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/examples/cross_1.hdf` & `yet_another_wizz-2.5/src/yaw/examples/cross_1.hdf`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/randoms.py` & `yet_another_wizz-2.5/src/yaw/randoms.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw/redshifts.py` & `yet_another_wizz-2.5/src/yaw/redshifts.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw_cli/commandline/main.py` & `yet_another_wizz-2.5/src/yaw_cli/commandline/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 class _Commandline:
 
     def __init__(self) -> None:
         self._subcommands: dict[str, SubCommand] = {}
         # add parser
         self.parser = argparse.ArgumentParser(
+            prog="yaw_cli",
             description="yet_another_wizz: modular clustering redshift pipeline.",
             epilog="Thank you for using yet_another_wizz. Please consider citing 'A&A 642, A200 (2020)' when publishing results obtained with this code.")
         self.parser.add_argument(
             "--version", action="version", version=f"yet_another_wizz v{__version__}")
         self.subparsers = self.parser.add_subparsers(
             title="modules",
             description="The pipeline is split into modules which perform specifc tasks as listed below. Each module has its own dedicated --help command.",
```

### Comparing `yet_another_wizz-2.4/src/yaw_cli/commandline/subcommands.py` & `yet_another_wizz-2.5/src/yaw_cli/commandline/subcommands.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,16 +59,16 @@
             threads=False,
             progress=False)
         parser.add_argument(  # manual since special help text
             "wdir", metavar="<path>", type=utils.Path_absolute,
             help="project directory, must not exist")
         parser.add_argument(
             "-s", "--setup", type=utils.Path_exists, metavar="<file>",
-            help="optionl setup YAML file (e.g. from 'yaw run -d') with base "
-                 "configuration that is overwritten by arguments below")
+            help="optionl setup YAML file (e.g. from 'yaw_cli run -d') with "
+                 "base configuration that is overwritten by arguments below")
 
         group_other = parser.add_argument_group(
             title="additional arguments")
         group_other.add_argument(
             "--backend", choices=OPTIONS.backend, default=DEFAULT.backend,
             help="backend used for pair counting (default: %(default)s)")
         group_other.add_argument(
```

### Comparing `yet_another_wizz-2.4/src/yaw_cli/commandline/utils.py` & `yet_another_wizz-2.5/src/yaw_cli/commandline/utils.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw_cli/pipeline/data.py` & `yet_another_wizz-2.5/src/yaw_cli/pipeline/data.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw_cli/pipeline/default_setup.py` & `yet_another_wizz-2.5/src/yaw_cli/pipeline/default_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 setup_default += format_line("weight: weight", "(opt) object weight", indents=level)
 setup_default += format_line("cache: false", "(opt) whether to cache the file in the cache directory", indents=level)
 level -= 1
 setup_default += format_line("rand: null", "random catalog for data sample, omit or repeat arguments from 'data' above ('filepath' format must must match 'data' above)", indents=level)
 
 # tasks
 setup_default += "\n"
-setup_default += wrap_comment("The section below is entirely optional and used to specify tasks to execute when using the 'yaw run' command. The list is generated and updated automatically when running 'yaw' subcommands. Tasks can be provided as single list entry, e.g.")
+setup_default += wrap_comment("The section below is entirely optional and used to specify tasks to execute when using the 'yaw_cli run' command. The list is generated and updated automatically when running 'yaw_cli' subcommands. Tasks can be provided as single list entry, e.g.")
 setup_default += f"{COMM_SEP}  - cross\n{COMM_SEP}  - zcc\n"
 setup_default += wrap_comment("to get a basic cluster redshift estimate or with the optional parameters listed below (all values optional, defaults listed).")
 setup_default += "tasks:\n"
 for task in tasks.Task.all_tasks():
     setup_default += format_line(task.get_name(), task.get_help(), indents=DASH)
     setup_default += make_doc(task, indent=2, indicate_opt=False)
 setup_default = setup_default.strip("\n")
```

### Comparing `yet_another_wizz-2.4/src/yaw_cli/pipeline/directories.py` & `yet_another_wizz-2.5/src/yaw_cli/pipeline/directories.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw_cli/pipeline/logger.py` & `yet_another_wizz-2.5/src/yaw_cli/pipeline/logger.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw_cli/pipeline/merge.py` & `yet_another_wizz-2.5/src/yaw_cli/pipeline/merge.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw_cli/pipeline/plot.py` & `yet_another_wizz-2.5/src/yaw_cli/pipeline/plot.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw_cli/pipeline/processing.py` & `yet_another_wizz-2.5/src/yaw_cli/pipeline/processing.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw_cli/pipeline/project.py` & `yet_another_wizz-2.5/src/yaw_cli/pipeline/project.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yaw_cli/pipeline/tasks.py` & `yet_another_wizz-2.5/src/yaw_cli/pipeline/tasks.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.4/src/yet_another_wizz.egg-info/SOURCES.txt` & `yet_another_wizz-2.5/src/yet_another_wizz.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 LICENSE
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
-bin/yaw
 src/yaw/__init__.py
 src/yaw/deprecated.py
 src/yaw/randoms.py
 src/yaw/redshifts.py
 src/yaw/catalogs/__init__.py
 src/yaw/catalogs/catalog.py
 src/yaw/catalogs/factory.py
@@ -43,14 +41,15 @@
 src/yaw/correlation/estimators.py
 src/yaw/correlation/paircounts.py
 src/yaw/examples/__init__.py
 src/yaw/examples/auto_reference.hdf
 src/yaw/examples/auto_unknown_1.hdf
 src/yaw/examples/cross_1.hdf
 src/yaw_cli/__init__.py
+src/yaw_cli/__main__.py
 src/yaw_cli/commandline/__init__.py
 src/yaw_cli/commandline/main.py
 src/yaw_cli/commandline/subcommands.py
 src/yaw_cli/commandline/utils.py
 src/yaw_cli/pipeline/__init__.py
 src/yaw_cli/pipeline/data.py
 src/yaw_cli/pipeline/default_setup.py
@@ -60,9 +59,10 @@
 src/yaw_cli/pipeline/plot.py
 src/yaw_cli/pipeline/processing.py
 src/yaw_cli/pipeline/project.py
 src/yaw_cli/pipeline/tasks.py
 src/yet_another_wizz.egg-info/PKG-INFO
 src/yet_another_wizz.egg-info/SOURCES.txt
 src/yet_another_wizz.egg-info/dependency_links.txt
+src/yet_another_wizz.egg-info/entry_points.txt
 src/yet_another_wizz.egg-info/requires.txt
 src/yet_another_wizz.egg-info/top_level.txt
```

