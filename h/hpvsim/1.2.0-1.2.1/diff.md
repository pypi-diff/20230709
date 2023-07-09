# Comparing `tmp/hpvsim-1.2.0.tar.gz` & `tmp/hpvsim-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpvsim-1.2.0.tar", last modified: Thu Jun  1 02:46:34 2023, max compression
+gzip compressed data, was "hpvsim-1.2.1.tar", last modified: Sun Jul  9 15:08:40 2023, max compression
```

## Comparing `hpvsim-1.2.0.tar` & `hpvsim-1.2.1.tar`

### file list

```diff
@@ -1,79 +1,89 @@
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.346614 hpvsim-1.2.0/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13532 2023-06-01 02:46:05.000000 hpvsim-1.2.0/CHANGELOG.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3501 2022-07-29 04:56:27.000000 hpvsim-1.2.0/CODE_OF_CONDUCT.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1087 2023-01-30 16:47:35.000000 hpvsim-1.2.0/LICENSE
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      205 2022-12-16 01:30:01.000000 hpvsim-1.2.0/MANIFEST.in
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3625 2023-06-01 02:46:34.346614 hpvsim-1.2.0/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2715 2023-02-01 00:00:08.000000 hpvsim-1.2.0/README.rst
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.342615 hpvsim-1.2.0/docs/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.analysis.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.base.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.calibration.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      150 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.data.get_data.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      145 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.data.loaders.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      224 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.data.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.defaults.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.immunity.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.interventions.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.misc.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.parameters.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.people.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.plotting.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.population.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      118 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.run.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.settings.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      118 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.sim.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      124 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.utils.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/hpvsim.version.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      312 2022-12-16 01:30:01.000000 hpvsim-1.2.0/docs/index.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      523 2023-01-31 21:47:37.000000 hpvsim-1.2.0/docs/modules.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       96 2022-08-31 16:50:17.000000 hpvsim-1.2.0/docs/overview.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2022-08-31 16:50:17.000000 hpvsim-1.2.0/docs/requirements.txt
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.342615 hpvsim-1.2.0/docs/tutorials/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      345 2022-12-16 01:30:01.000000 hpvsim-1.2.0/docs/tutorials/README.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      299 2023-02-01 00:00:08.000000 hpvsim-1.2.0/docs/tutorials.rst
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       29 2022-08-31 16:50:17.000000 hpvsim-1.2.0/docs/whats-new.rst
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.342615 hpvsim-1.2.0/hpvsim/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1048 2023-01-30 16:47:35.000000 hpvsim-1.2.0/hpvsim/__init__.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    55482 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/analysis.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    83229 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/base.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    37175 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/calibration.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.346614 hpvsim-1.2.0/hpvsim/data/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       46 2022-08-31 16:50:17.000000 hpvsim-1.2.0/hpvsim/data/__init__.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.346614 hpvsim-1.2.0/hpvsim/data/files/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       87 2022-10-04 15:39:45.000000 hpvsim-1.2.0/hpvsim/data/files/metadata.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7459 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/data/get_data.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    12106 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/data/loaders.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    18870 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/data/products_dx.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1871 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/data/products_tx.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      197 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/data/products_txvx.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      369 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/data/products_vx.csv
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    21237 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/defaults.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22876 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/hiv.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13902 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/immunity.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    67175 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/interventions.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    28482 2022-12-16 01:30:01.000000 hpvsim-1.2.0/hpvsim/misc.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    40694 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/parameters.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    48721 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/people.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    44030 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/plotting.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    17813 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/population.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.346614 hpvsim-1.2.0/hpvsim/regression/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22216 2022-10-12 05:00:20.000000 hpvsim-1.2.0/hpvsim/regression/pars_v0.2.6.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22085 2022-12-16 01:30:01.000000 hpvsim-1.2.0/hpvsim/regression/pars_v0.2.9.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    21901 2022-12-16 01:30:01.000000 hpvsim-1.2.0/hpvsim/regression/pars_v0.3.0.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23231 2022-12-16 01:30:01.000000 hpvsim-1.2.0/hpvsim/regression/pars_v0.3.1.json
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    71932 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/run.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22131 2022-12-16 01:30:01.000000 hpvsim-1.2.0/hpvsim/settings.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    67290 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/sim.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    24398 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/utils.py
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      233 2023-06-01 02:46:05.000000 hpvsim-1.2.0/hpvsim/version.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.342615 hpvsim-1.2.0/hpvsim.egg-info/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3625 2023-06-01 02:46:34.000000 hpvsim-1.2.0/hpvsim.egg-info/PKG-INFO
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1531 2023-06-01 02:46:34.000000 hpvsim-1.2.0/hpvsim.egg-info/SOURCES.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2023-06-01 02:46:34.000000 hpvsim-1.2.0/hpvsim.egg-info/dependency_links.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       66 2023-06-01 02:46:34.000000 hpvsim-1.2.0/hpvsim.egg-info/requires.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        7 2023-06-01 02:46:34.000000 hpvsim-1.2.0/hpvsim.egg-info/top_level.txt
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2023-06-01 02:46:34.346614 hpvsim-1.2.0/setup.cfg
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1566 2023-06-01 02:46:05.000000 hpvsim-1.2.0/setup.py
-drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-06-01 02:46:34.346614 hpvsim-1.2.0/tests/
--rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       50 2023-01-30 16:47:35.000000 hpvsim-1.2.0/tests/requirements.txt
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-07-09 15:08:40.966525 hpvsim-1.2.1/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13532 2023-06-01 02:46:05.000000 hpvsim-1.2.1/CHANGELOG.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3501 2022-07-29 04:56:27.000000 hpvsim-1.2.1/CODE_OF_CONDUCT.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1087 2023-01-30 16:47:35.000000 hpvsim-1.2.1/LICENSE
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      205 2022-12-16 01:30:01.000000 hpvsim-1.2.1/MANIFEST.in
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3625 2023-07-09 15:08:40.966525 hpvsim-1.2.1/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     2715 2023-02-01 00:00:08.000000 hpvsim-1.2.1/README.rst
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-07-09 15:08:40.962526 hpvsim-1.2.1/docs/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.analysis.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.base.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      142 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.calibration.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      157 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.data.downloaders.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      145 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.data.loaders.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      227 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.data.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.defaults.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      118 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.hiv.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.immunity.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      148 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.interventions.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      121 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.misc.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.parameters.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      127 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.people.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.plotting.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      139 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.population.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      118 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.run.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      133 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.settings.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      118 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.sim.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      124 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.utils.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      130 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/hpvsim.version.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      312 2022-12-16 01:30:01.000000 hpvsim-1.2.1/docs/index.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      537 2023-07-09 14:51:24.000000 hpvsim-1.2.1/docs/modules.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       96 2022-08-31 16:50:17.000000 hpvsim-1.2.1/docs/overview.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      104 2022-08-31 16:50:17.000000 hpvsim-1.2.1/docs/requirements.txt
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-07-09 15:08:40.962526 hpvsim-1.2.1/docs/tutorials/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      345 2022-12-16 01:30:01.000000 hpvsim-1.2.1/docs/tutorials/README.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      299 2023-02-01 00:00:08.000000 hpvsim-1.2.1/docs/tutorials.rst
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       29 2022-08-31 16:50:17.000000 hpvsim-1.2.1/docs/whats-new.rst
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-07-09 15:08:40.962526 hpvsim-1.2.1/hpvsim/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1048 2023-01-30 16:47:35.000000 hpvsim-1.2.1/hpvsim/__init__.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    55482 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/analysis.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    83229 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/base.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    37175 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/calibration.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-07-09 15:08:40.962526 hpvsim-1.2.1/hpvsim/data/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       49 2023-07-09 14:51:00.000000 hpvsim-1.2.1/hpvsim/data/__init__.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7615 2023-07-09 14:51:00.000000 hpvsim-1.2.1/hpvsim/data/downloaders.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-07-09 15:08:40.962526 hpvsim-1.2.1/hpvsim/data/files/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       95 2023-07-07 08:30:18.000000 hpvsim-1.2.1/hpvsim/data/files/metadata.json
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    12106 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/data/loaders.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    18870 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/data/products_dx.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1871 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/data/products_tx.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      197 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/data/products_txvx.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      369 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/data/products_vx.csv
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    21237 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/defaults.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22876 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/hiv.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    13902 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/immunity.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    67175 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/interventions.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    28482 2022-12-16 01:30:01.000000 hpvsim-1.2.1/hpvsim/misc.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    40694 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/parameters.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    48721 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/people.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    44030 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/plotting.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    17813 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/population.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-07-09 15:08:40.962526 hpvsim-1.2.1/hpvsim/regression/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22216 2022-10-12 05:00:20.000000 hpvsim-1.2.1/hpvsim/regression/pars_v0.2.6.json
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22085 2022-12-16 01:30:01.000000 hpvsim-1.2.1/hpvsim/regression/pars_v0.2.9.json
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    21901 2022-12-16 01:30:01.000000 hpvsim-1.2.1/hpvsim/regression/pars_v0.3.0.json
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    23231 2022-12-16 01:30:01.000000 hpvsim-1.2.1/hpvsim/regression/pars_v0.3.1.json
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)   414559 2023-07-07 19:07:16.000000 hpvsim-1.2.1/hpvsim/regression/pars_v1.2.0.json
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    71932 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/run.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    22131 2022-12-16 01:30:01.000000 hpvsim-1.2.1/hpvsim/settings.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    67290 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/sim.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    24398 2023-06-01 02:46:05.000000 hpvsim-1.2.1/hpvsim/utils.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      233 2023-07-09 14:51:00.000000 hpvsim-1.2.1/hpvsim/version.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-07-09 15:08:40.962526 hpvsim-1.2.1/hpvsim.egg-info/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     3625 2023-07-09 15:08:40.000000 hpvsim-1.2.1/hpvsim.egg-info/PKG-INFO
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1777 2023-07-09 15:08:40.000000 hpvsim-1.2.1/hpvsim.egg-info/SOURCES.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        1 2023-07-09 15:08:40.000000 hpvsim-1.2.1/hpvsim.egg-info/dependency_links.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       66 2023-07-09 15:08:40.000000 hpvsim-1.2.1/hpvsim.egg-info/requires.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)        7 2023-07-09 15:08:40.000000 hpvsim-1.2.1/hpvsim.egg-info/top_level.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       38 2023-07-09 15:08:40.966525 hpvsim-1.2.1/setup.cfg
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1566 2023-07-09 14:51:00.000000 hpvsim-1.2.1/setup.py
+drwxrwxr-x   0 cliffk    (1000) cliffk    (1000)        0 2023-07-09 15:08:40.966525 hpvsim-1.2.1/tests/
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)       50 2023-01-30 16:47:35.000000 hpvsim-1.2.1/tests/requirements.txt
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6890 2023-06-01 02:46:05.000000 hpvsim-1.2.1/tests/test_analysis.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     6594 2023-03-10 03:16:55.000000 hpvsim-1.2.1/tests/test_baselines.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     4133 2023-06-01 02:46:05.000000 hpvsim-1.2.1/tests/test_calibration.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)      736 2022-12-16 01:30:01.000000 hpvsim-1.2.1/tests/test_data.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     1074 2022-10-12 05:00:03.000000 hpvsim-1.2.1/tests/test_event_schedule.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    20418 2023-01-30 16:47:35.000000 hpvsim-1.2.1/tests/test_interventions.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)     7367 2023-01-30 16:47:35.000000 hpvsim-1.2.1/tests/test_run.py
+-rw-rw-r--   0 cliffk    (1000) cliffk    (1000)    18391 2023-06-01 02:46:05.000000 hpvsim-1.2.1/tests/test_sim.py
```

### Comparing `hpvsim-1.2.0/CHANGELOG.rst` & `hpvsim-1.2.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/CODE_OF_CONDUCT.rst` & `hpvsim-1.2.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/LICENSE` & `hpvsim-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/PKG-INFO` & `hpvsim-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpvsim
-Version: 1.2.0
+Version: 1.2.1
 Summary: HPVsim: Human Papillomavirus Simulator
 Home-page: http://hpvsim.org
 Author: Robyn Stuart, Jamie Cohen, Cliff Kerr, Romesh Abeysuriya, Mariah Boudreau, Daniel Klein, Hao Hu
 Author-email: robyn.stuart@gatesfoundation.org
 Keywords: HPV,agent-based model,simulation
 Platform: OS Independent
 Classifier: Environment :: Console
```

### Comparing `hpvsim-1.2.0/README.rst` & `hpvsim-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/docs/modules.rst` & `hpvsim-1.2.1/docs/modules.rst`

 * *Files 25% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 .. toctree::
    :maxdepth: 4
 
    hpvsim.analysis
    hpvsim.base
    hpvsim.calibration
    hpvsim.defaults
+   hpvsim.hiv
    hpvsim.immunity
    hpvsim.interventions
    hpvsim.misc
    hpvsim.parameters
    hpvsim.people
    hpvsim.plotting
    hpvsim.population
```

### Comparing `hpvsim-1.2.0/hpvsim/__init__.py` & `hpvsim-1.2.1/hpvsim/__init__.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/analysis.py` & `hpvsim-1.2.1/hpvsim/analysis.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/base.py` & `hpvsim-1.2.1/hpvsim/base.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/calibration.py` & `hpvsim-1.2.1/hpvsim/calibration.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/data/get_data.py` & `hpvsim-1.2.1/hpvsim/data/downloaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,28 +15,38 @@
 from urllib import request
 import numpy as np
 import pandas as pd
 import sciris as sc
 from . import loaders
 
 # Set parameters
-data_version = '1.1' # Data version
+data_version = '1.2' # Data version
 data_file = f'hpvsim_data_v{data_version}.zip'
 quick_url = f'https://github.com/amath-idm/hpvsim_data/blob/main/{data_file}?raw=true'
 age_stem = 'WPP2022_Population1JanuaryBySingleAgeSex_Medium_'
 death_stem = 'WPP2022_Life_Table_Abridged_Medium_'
 base_url = 'https://population.un.org/wpp/Download/Files/1_Indicators%20(Standard)/CSV_FILES/'
 years = ['1950-2021', '2022-2100']
 
 
-thisdir = sc.path(sc.thisdir())
+thisdir = sc.thispath()
 filesdir = thisdir / 'files'
 
 __all__ = ['get_data', 'quick_download', 'check_downloaded', 'remove_data']
 
+
+def set_filesdir(path):
+    ''' Used to change the file folder '''
+    global filesdir
+    orig = filesdir
+    filesdir = path
+    print(f'Done: filesdir reset from {orig} to {filesdir}')
+    return
+
+
 def get_UN_data(label='', file_stem=None, outfile=None, columns=None, force=None, tidy=None):
     ''' Download data from UN Population Division '''
     if force is None: force = False
     if tidy  is None: tidy  = True
 
     sc.heading(f'Downloading {label} data...')
     T = sc.timer()
@@ -99,15 +109,15 @@
 
 def get_birth_data(start=1960, end=2020):
     ''' Import crude birth rates from WB '''
     sc.heading('Downloading World Bank birth rate data...')
     try:
         import wbgapi as wb
     except Exception as E:
-        errormsg = f'Could not import wbgapi: cannot download raw data'
+        errormsg = 'Could not import wbgapi: cannot download raw data'
         raise ModuleNotFoundError(errormsg) from E
     T = sc.timer()
     birth_rates = wb.data.DataFrame('SP.DYN.CBRT.IN', time=range(start,end), labels=True, skipAggs=True).reset_index()
     d = dict()
     for country in birth_rates['Country'].unique():
         d[country] = birth_rates.loc[(birth_rates['Country']==country)].values[0,2:]
     d['years'] = np.arange(start, end)
@@ -126,15 +136,15 @@
         get_death_data()
     if which in ['life_expectancy', 'ex']:
         get_ex_data()
     return
 
 
 def get_data():
-    ''' Download data '''
+    ''' Download data in parallel '''
     sc.heading('Downloading HPVsim data, please be patient...')
     T = sc.timer()
 
     if len(sys.argv) > 1:
         which = sys.argv[1]
         if which not in ['all', 'age', 'ages', 'birth', 'births', 'death', 'deaths']:
             errormsg = f'Invalid selection "{which}": must be all, ages, births, or deaths'
@@ -205,11 +215,8 @@
 
 def remove_data(verbose=True, **kwargs):
     ''' Remove downloaded data; arguments passed to sc.rmpath() '''
     if verbose: sc.heading('Removing HPVsim data files')
     for key,fn in loaders.files.items():
         sc.rmpath(fn, verbose=verbose, **kwargs)
     if verbose: print('Data files removed.')
-    return
-
-if __name__ == '__main__':
-    quick_download()
+    return
```

### Comparing `hpvsim-1.2.0/hpvsim/data/loaders.py` & `hpvsim-1.2.1/hpvsim/data/loaders.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/data/products_dx.csv` & `hpvsim-1.2.1/hpvsim/data/products_dx.csv`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/data/products_tx.csv` & `hpvsim-1.2.1/hpvsim/data/products_tx.csv`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/defaults.py` & `hpvsim-1.2.1/hpvsim/defaults.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/hiv.py` & `hpvsim-1.2.1/hpvsim/hiv.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/immunity.py` & `hpvsim-1.2.1/hpvsim/immunity.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/interventions.py` & `hpvsim-1.2.1/hpvsim/interventions.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/misc.py` & `hpvsim-1.2.1/hpvsim/misc.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/parameters.py` & `hpvsim-1.2.1/hpvsim/parameters.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/people.py` & `hpvsim-1.2.1/hpvsim/people.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/plotting.py` & `hpvsim-1.2.1/hpvsim/plotting.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/population.py` & `hpvsim-1.2.1/hpvsim/population.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/regression/pars_v0.2.6.json` & `hpvsim-1.2.1/hpvsim/regression/pars_v0.2.6.json`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/regression/pars_v0.2.9.json` & `hpvsim-1.2.1/hpvsim/regression/pars_v0.2.9.json`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/regression/pars_v0.3.0.json` & `hpvsim-1.2.1/hpvsim/regression/pars_v0.3.0.json`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/regression/pars_v0.3.1.json` & `hpvsim-1.2.1/hpvsim/regression/pars_v0.3.1.json`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/run.py` & `hpvsim-1.2.1/hpvsim/run.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/settings.py` & `hpvsim-1.2.1/hpvsim/settings.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/sim.py` & `hpvsim-1.2.1/hpvsim/sim.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim/utils.py` & `hpvsim-1.2.1/hpvsim/utils.py`

 * *Files identical despite different names*

### Comparing `hpvsim-1.2.0/hpvsim.egg-info/PKG-INFO` & `hpvsim-1.2.1/hpvsim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpvsim
-Version: 1.2.0
+Version: 1.2.1
 Summary: HPVsim: Human Papillomavirus Simulator
 Home-page: http://hpvsim.org
 Author: Robyn Stuart, Jamie Cohen, Cliff Kerr, Romesh Abeysuriya, Mariah Boudreau, Daniel Klein, Hao Hu
 Author-email: robyn.stuart@gatesfoundation.org
 Keywords: HPV,agent-based model,simulation
 Platform: OS Independent
 Classifier: Environment :: Console
```

### Comparing `hpvsim-1.2.0/hpvsim.egg-info/SOURCES.txt` & `hpvsim-1.2.1/hpvsim.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
 docs/hpvsim.analysis.rst
 docs/hpvsim.base.rst
 docs/hpvsim.calibration.rst
-docs/hpvsim.data.get_data.rst
+docs/hpvsim.data.downloaders.rst
 docs/hpvsim.data.loaders.rst
 docs/hpvsim.data.rst
 docs/hpvsim.defaults.rst
+docs/hpvsim.hiv.rst
 docs/hpvsim.immunity.rst
 docs/hpvsim.interventions.rst
 docs/hpvsim.misc.rst
 docs/hpvsim.parameters.rst
 docs/hpvsim.people.rst
 docs/hpvsim.plotting.rst
 docs/hpvsim.population.rst
@@ -50,19 +51,28 @@
 hpvsim/version.py
 hpvsim.egg-info/PKG-INFO
 hpvsim.egg-info/SOURCES.txt
 hpvsim.egg-info/dependency_links.txt
 hpvsim.egg-info/requires.txt
 hpvsim.egg-info/top_level.txt
 hpvsim/data/__init__.py
-hpvsim/data/get_data.py
+hpvsim/data/downloaders.py
 hpvsim/data/loaders.py
 hpvsim/data/products_dx.csv
 hpvsim/data/products_tx.csv
 hpvsim/data/products_txvx.csv
 hpvsim/data/products_vx.csv
 hpvsim/data/files/metadata.json
 hpvsim/regression/pars_v0.2.6.json
 hpvsim/regression/pars_v0.2.9.json
 hpvsim/regression/pars_v0.3.0.json
 hpvsim/regression/pars_v0.3.1.json
-tests/requirements.txt
+hpvsim/regression/pars_v1.2.0.json
+tests/requirements.txt
+tests/test_analysis.py
+tests/test_baselines.py
+tests/test_calibration.py
+tests/test_data.py
+tests/test_event_schedule.py
+tests/test_interventions.py
+tests/test_run.py
+tests/test_sim.py
```

### Comparing `hpvsim-1.2.0/setup.py` & `hpvsim-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,14 @@
     platforms=["OS Independent"],
     classifiers=CLASSIFIERS,
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'numpy',
         'scipy',
-        'pandas>=1.4.0', 
+        'pandas>=2.0.0', 
         'sciris>=3.0.0',
         'matplotlib',
         'seaborn',
         'optuna',
     ],
 )
```

