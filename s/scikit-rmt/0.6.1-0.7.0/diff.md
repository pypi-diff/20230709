# Comparing `tmp/scikit-rmt-0.6.1.tar.gz` & `tmp/scikit-rmt-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-rmt-0.6.1.tar", last modified: Sat Jul  8 21:07:00 2023, max compression
+gzip compressed data, was "dist/scikit-rmt-0.7.0.tar", last modified: Sat Jul  8 22:53:00 2023, max compression
```

## Comparing `scikit-rmt-0.6.1.tar` & `scikit-rmt-0.7.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.387165 scikit-rmt-0.6.1/
--rw-r--r--   0 santorum   (501) staff       (20)      337 2021-05-02 17:28:24.000000 scikit-rmt-0.6.1/.coveragerc
--rw-r--r--   0 santorum   (501) staff       (20)      278 2023-03-09 19:40:44.000000 scikit-rmt-0.6.1/.travis.yml
--rw-r--r--   0 santorum   (501) staff       (20)      382 2023-01-27 19:58:20.000000 scikit-rmt-0.6.1/CITATION.cff
--rw-r--r--   0 santorum   (501) staff       (20)     1563 2021-04-26 20:56:17.000000 scikit-rmt-0.6.1/LICENSE
--rw-r--r--   0 santorum   (501) staff       (20)      346 2023-01-27 19:52:49.000000 scikit-rmt-0.6.1/MANIFEST.in
--rw-r--r--   0 santorum   (501) staff       (20)     2569 2021-05-05 17:08:35.000000 scikit-rmt-0.6.1/Makefile
--rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-07-08 21:07:00.387626 scikit-rmt-0.6.1/PKG-INFO
--rw-r--r--   0 santorum   (501) staff       (20)    19268 2023-06-21 14:56:22.000000 scikit-rmt-0.6.1/README.md
--rw-r--r--   0 santorum   (501) staff       (20)     3189 2023-01-27 19:40:29.000000 scikit-rmt-0.6.1/conf.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.340109 scikit-rmt-0.6.1/docs/
--rw-r--r--   0 santorum   (501) staff       (20)       52 2022-10-04 14:32:13.000000 scikit-rmt-0.6.1/docs/modules.rst
--rw-r--r--   0 santorum   (501) staff       (20)       54 2021-05-08 23:10:40.000000 scikit-rmt-0.6.1/docs/readthedocs-requirements.txt
--rw-r--r--   0 santorum   (501) staff       (20)      522 2022-10-04 14:32:13.000000 scikit-rmt-0.6.1/docs/skrmt.covariance.rst
--rw-r--r--   0 santorum   (501) staff       (20)     1114 2023-06-21 14:56:22.000000 scikit-rmt-0.6.1/docs/skrmt.ensemble.rst
--rw-r--r--   0 santorum   (501) staff       (20)      232 2022-10-04 14:32:13.000000 scikit-rmt-0.6.1/docs/skrmt.rst
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.345620 scikit-rmt-0.6.1/examples/
--rw-r--r--   0 santorum   (501) staff       (20)       70 2021-05-08 16:13:31.000000 scikit-rmt-0.6.1/examples/README.txt
--rw-r--r--   0 santorum   (501) staff       (20)     2155 2023-07-08 20:47:44.000000 scikit-rmt-0.6.1/examples/plot_boosting_density_representation.py
--rw-r--r--   0 santorum   (501) staff       (20)     2559 2021-05-10 19:22:01.000000 scikit-rmt-0.6.1/examples/plot_circular_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     1385 2022-10-04 14:35:07.000000 scikit-rmt-0.6.1/examples/plot_complex_histograms.py
--rw-r--r--   0 santorum   (501) staff       (20)     2651 2021-05-10 18:16:25.000000 scikit-rmt-0.6.1/examples/plot_gaussian_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     3200 2021-05-10 19:13:42.000000 scikit-rmt-0.6.1/examples/plot_manova_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     2417 2021-05-10 19:07:13.000000 scikit-rmt-0.6.1/examples/plot_wishart_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)     2293 2021-05-14 20:07:04.000000 scikit-rmt-0.6.1/index.rst
--rw-r--r--   0 santorum   (501) staff       (20)      506 2023-05-06 11:49:55.000000 scikit-rmt-0.6.1/readthedocs.yml
--rw-r--r--   0 santorum   (501) staff       (20)       66 2023-06-21 14:56:22.000000 scikit-rmt-0.6.1/requirements.txt
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.350303 scikit-rmt-0.6.1/scikit_rmt.egg-info/
--rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-07-08 21:07:00.000000 scikit-rmt-0.6.1/scikit_rmt.egg-info/PKG-INFO
--rw-r--r--   0 santorum   (501) staff       (20)     1718 2023-07-08 21:07:00.000000 scikit-rmt-0.6.1/scikit_rmt.egg-info/SOURCES.txt
--rw-r--r--   0 santorum   (501) staff       (20)        1 2023-07-08 21:07:00.000000 scikit-rmt-0.6.1/scikit_rmt.egg-info/dependency_links.txt
--rw-r--r--   0 santorum   (501) staff       (20)       67 2023-07-08 21:07:00.000000 scikit-rmt-0.6.1/scikit_rmt.egg-info/requires.txt
--rw-r--r--   0 santorum   (501) staff       (20)        6 2023-07-08 21:07:00.000000 scikit-rmt-0.6.1/scikit_rmt.egg-info/top_level.txt
--rw-r--r--   0 santorum   (501) staff       (20)       38 2023-07-08 21:07:00.388242 scikit-rmt-0.6.1/setup.cfg
--rw-r--r--   0 santorum   (501) staff       (20)     2239 2023-05-06 11:35:01.000000 scikit-rmt-0.6.1/setup.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.351812 scikit-rmt-0.6.1/skrmt/
--rw-r--r--   0 santorum   (501) staff       (20)       95 2023-01-27 19:00:33.000000 scikit-rmt-0.6.1/skrmt/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)       49 2023-07-06 19:32:53.000000 scikit-rmt-0.6.1/skrmt/_version.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.354789 scikit-rmt-0.6.1/skrmt/covariance/
--rw-r--r--   0 santorum   (501) staff       (20)      734 2021-04-28 22:17:52.000000 scikit-rmt-0.6.1/skrmt/covariance/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)    10347 2021-05-04 14:06:35.000000 scikit-rmt-0.6.1/skrmt/covariance/estimator.py
--rw-r--r--   0 santorum   (501) staff       (20)     3144 2021-04-28 17:36:36.000000 scikit-rmt-0.6.1/skrmt/covariance/metrics.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.357234 scikit-rmt-0.6.1/skrmt/covariance/tests/
--rw-r--r--   0 santorum   (501) staff       (20)        0 2021-04-13 20:20:47.000000 scikit-rmt-0.6.1/skrmt/covariance/tests/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)     6356 2021-04-28 22:13:28.000000 scikit-rmt-0.6.1/skrmt/covariance/tests/test_estimator.py
--rw-r--r--   0 santorum   (501) staff       (20)     3823 2021-05-02 17:01:05.000000 scikit-rmt-0.6.1/skrmt/covariance/tests/test_metrics.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.368282 scikit-rmt-0.6.1/skrmt/ensemble/
--rw-r--r--   0 santorum   (501) staff       (20)     1021 2023-06-21 14:56:22.000000 scikit-rmt-0.6.1/skrmt/ensemble/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)     9693 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/_base_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    13737 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/circular_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    14984 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/gaussian_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    13881 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/manova_ensemble.py
--rw-r--r--   0 santorum   (501) staff       (20)    56082 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/spectral_law.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.383580 scikit-rmt-0.6.1/skrmt/ensemble/tests/
--rw-r--r--   0 santorum   (501) staff       (20)        0 2021-03-30 20:39:25.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/__init__.py
--rw-r--r--   0 santorum   (501) staff       (20)      287 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_base_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)     5714 2023-06-21 14:56:22.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_circular_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    11926 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_gaussian_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)     5058 2023-06-21 14:56:22.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_manova_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    42454 2023-07-06 19:27:12.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_spectral_law.py
--rw-r--r--   0 santorum   (501) staff       (20)     1611 2023-01-05 15:04:32.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_tracy_widom_approx.py
--rw-r--r--   0 santorum   (501) staff       (20)     1200 2021-05-04 14:00:53.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_tridiagonalization.py
--rw-r--r--   0 santorum   (501) staff       (20)    14668 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/tests/test_wishart_ens.py
--rw-r--r--   0 santorum   (501) staff       (20)    33083 2023-05-06 11:35:01.000000 scikit-rmt-0.6.1/skrmt/ensemble/tracy_widom_approximator.py
--rw-r--r--   0 santorum   (501) staff       (20)     6028 2023-05-06 11:35:01.000000 scikit-rmt-0.6.1/skrmt/ensemble/tridiagonal_utils.py
--rw-r--r--   0 santorum   (501) staff       (20)    16537 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/skrmt/ensemble/wishart_ensemble.py
-drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 21:07:00.386580 scikit-rmt-0.6.1/tutorial/
--rw-r--r--   0 santorum   (501) staff       (20)       64 2021-05-09 15:49:23.000000 scikit-rmt-0.6.1/tutorial/README.txt
--rw-r--r--   0 santorum   (501) staff       (20)     2706 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/tutorial/plot_0_introduction.py
--rw-r--r--   0 santorum   (501) staff       (20)    10272 2023-06-21 14:56:22.000000 scikit-rmt-0.6.1/tutorial/plot_1_spectral_laws.py
--rw-r--r--   0 santorum   (501) staff       (20)     9176 2023-07-08 21:05:42.000000 scikit-rmt-0.6.1/tutorial/plot_2_plot_spectral_laws.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.380699 scikit-rmt-0.7.0/
+-rw-r--r--   0 santorum   (501) staff       (20)      337 2021-05-02 17:28:24.000000 scikit-rmt-0.7.0/.coveragerc
+-rw-r--r--   0 santorum   (501) staff       (20)      278 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/.travis.yml
+-rw-r--r--   0 santorum   (501) staff       (20)      382 2023-01-27 19:58:20.000000 scikit-rmt-0.7.0/CITATION.cff
+-rw-r--r--   0 santorum   (501) staff       (20)     1563 2021-04-26 20:56:17.000000 scikit-rmt-0.7.0/LICENSE
+-rw-r--r--   0 santorum   (501) staff       (20)      346 2023-01-27 19:52:49.000000 scikit-rmt-0.7.0/MANIFEST.in
+-rw-r--r--   0 santorum   (501) staff       (20)     2569 2023-07-08 22:52:37.000000 scikit-rmt-0.7.0/Makefile
+-rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-07-08 22:53:00.381033 scikit-rmt-0.7.0/PKG-INFO
+-rw-r--r--   0 santorum   (501) staff       (20)    19268 2023-06-21 14:56:22.000000 scikit-rmt-0.7.0/README.md
+-rw-r--r--   0 santorum   (501) staff       (20)     3189 2023-01-27 19:40:29.000000 scikit-rmt-0.7.0/conf.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.339736 scikit-rmt-0.7.0/docs/
+-rw-r--r--   0 santorum   (501) staff       (20)       52 2022-10-04 14:32:13.000000 scikit-rmt-0.7.0/docs/modules.rst
+-rw-r--r--   0 santorum   (501) staff       (20)       54 2021-05-08 23:10:40.000000 scikit-rmt-0.7.0/docs/readthedocs-requirements.txt
+-rw-r--r--   0 santorum   (501) staff       (20)      522 2022-10-04 14:32:13.000000 scikit-rmt-0.7.0/docs/skrmt.covariance.rst
+-rw-r--r--   0 santorum   (501) staff       (20)     1114 2023-06-21 14:56:22.000000 scikit-rmt-0.7.0/docs/skrmt.ensemble.rst
+-rw-r--r--   0 santorum   (501) staff       (20)      232 2022-10-04 14:32:13.000000 scikit-rmt-0.7.0/docs/skrmt.rst
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.347457 scikit-rmt-0.7.0/examples/
+-rw-r--r--   0 santorum   (501) staff       (20)       70 2021-05-08 16:13:31.000000 scikit-rmt-0.7.0/examples/README.txt
+-rw-r--r--   0 santorum   (501) staff       (20)     2155 2023-07-08 20:47:44.000000 scikit-rmt-0.7.0/examples/plot_boosting_density_representation.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2559 2021-05-10 19:22:01.000000 scikit-rmt-0.7.0/examples/plot_circular_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1385 2022-10-04 14:35:07.000000 scikit-rmt-0.7.0/examples/plot_complex_histograms.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2651 2021-05-10 18:16:25.000000 scikit-rmt-0.7.0/examples/plot_gaussian_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3200 2021-05-10 19:13:42.000000 scikit-rmt-0.7.0/examples/plot_manova_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2417 2021-05-10 19:07:13.000000 scikit-rmt-0.7.0/examples/plot_wishart_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)     2293 2021-05-14 20:07:04.000000 scikit-rmt-0.7.0/index.rst
+-rw-r--r--   0 santorum   (501) staff       (20)      506 2023-05-06 11:49:55.000000 scikit-rmt-0.7.0/readthedocs.yml
+-rw-r--r--   0 santorum   (501) staff       (20)       65 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/requirements.txt
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.350678 scikit-rmt-0.7.0/scikit_rmt.egg-info/
+-rw-r--r--   0 santorum   (501) staff       (20)    23760 2023-07-08 22:53:00.000000 scikit-rmt-0.7.0/scikit_rmt.egg-info/PKG-INFO
+-rw-r--r--   0 santorum   (501) staff       (20)     1718 2023-07-08 22:53:00.000000 scikit-rmt-0.7.0/scikit_rmt.egg-info/SOURCES.txt
+-rw-r--r--   0 santorum   (501) staff       (20)        1 2023-07-08 22:53:00.000000 scikit-rmt-0.7.0/scikit_rmt.egg-info/dependency_links.txt
+-rw-r--r--   0 santorum   (501) staff       (20)       66 2023-07-08 22:53:00.000000 scikit-rmt-0.7.0/scikit_rmt.egg-info/requires.txt
+-rw-r--r--   0 santorum   (501) staff       (20)        6 2023-07-08 22:53:00.000000 scikit-rmt-0.7.0/scikit_rmt.egg-info/top_level.txt
+-rw-r--r--   0 santorum   (501) staff       (20)       38 2023-07-08 22:53:00.381638 scikit-rmt-0.7.0/setup.cfg
+-rw-r--r--   0 santorum   (501) staff       (20)     2239 2023-05-06 11:35:01.000000 scikit-rmt-0.7.0/setup.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.352389 scikit-rmt-0.7.0/skrmt/
+-rw-r--r--   0 santorum   (501) staff       (20)       95 2023-01-27 19:00:33.000000 scikit-rmt-0.7.0/skrmt/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)       49 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/_version.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.357121 scikit-rmt-0.7.0/skrmt/covariance/
+-rw-r--r--   0 santorum   (501) staff       (20)      734 2021-04-28 22:17:52.000000 scikit-rmt-0.7.0/skrmt/covariance/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)    10347 2021-05-04 14:06:35.000000 scikit-rmt-0.7.0/skrmt/covariance/estimator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3144 2021-04-28 17:36:36.000000 scikit-rmt-0.7.0/skrmt/covariance/metrics.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.359991 scikit-rmt-0.7.0/skrmt/covariance/tests/
+-rw-r--r--   0 santorum   (501) staff       (20)        0 2021-04-13 20:20:47.000000 scikit-rmt-0.7.0/skrmt/covariance/tests/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)     6356 2021-04-28 22:13:28.000000 scikit-rmt-0.7.0/skrmt/covariance/tests/test_estimator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     3823 2021-05-02 17:01:05.000000 scikit-rmt-0.7.0/skrmt/covariance/tests/test_metrics.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.366985 scikit-rmt-0.7.0/skrmt/ensemble/
+-rw-r--r--   0 santorum   (501) staff       (20)     1021 2023-06-21 14:56:22.000000 scikit-rmt-0.7.0/skrmt/ensemble/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)    10728 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/_base_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    13872 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/circular_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    15308 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/gaussian_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    14125 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/manova_ensemble.py
+-rw-r--r--   0 santorum   (501) staff       (20)    56446 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/spectral_law.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.376211 scikit-rmt-0.7.0/skrmt/ensemble/tests/
+-rw-r--r--   0 santorum   (501) staff       (20)        0 2021-03-30 20:39:25.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/__init__.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1936 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_base_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)     5714 2023-06-21 14:56:22.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_circular_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    12191 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_gaussian_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)     5058 2023-06-21 14:56:22.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_manova_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    42454 2023-07-06 19:27:12.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_spectral_law.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1611 2023-01-05 15:04:32.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_tracy_widom_approx.py
+-rw-r--r--   0 santorum   (501) staff       (20)     1200 2021-05-04 14:00:53.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_tridiagonalization.py
+-rw-r--r--   0 santorum   (501) staff       (20)    14730 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/tests/test_wishart_ens.py
+-rw-r--r--   0 santorum   (501) staff       (20)    33083 2023-05-06 11:35:01.000000 scikit-rmt-0.7.0/skrmt/ensemble/tracy_widom_approximator.py
+-rw-r--r--   0 santorum   (501) staff       (20)     6028 2023-05-06 11:35:01.000000 scikit-rmt-0.7.0/skrmt/ensemble/tridiagonal_utils.py
+-rw-r--r--   0 santorum   (501) staff       (20)    17113 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/skrmt/ensemble/wishart_ensemble.py
+drwxr-xr-x   0 santorum   (501) staff       (20)        0 2023-07-08 22:53:00.380142 scikit-rmt-0.7.0/tutorial/
+-rw-r--r--   0 santorum   (501) staff       (20)       64 2021-05-09 15:49:23.000000 scikit-rmt-0.7.0/tutorial/README.txt
+-rw-r--r--   0 santorum   (501) staff       (20)     2689 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/tutorial/plot_0_introduction.py
+-rw-r--r--   0 santorum   (501) staff       (20)    10272 2023-06-21 14:56:22.000000 scikit-rmt-0.7.0/tutorial/plot_1_spectral_laws.py
+-rw-r--r--   0 santorum   (501) staff       (20)     9183 2023-07-08 22:32:18.000000 scikit-rmt-0.7.0/tutorial/plot_2_plot_spectral_laws.py
```

### Comparing `scikit-rmt-0.6.1/LICENSE` & `scikit-rmt-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/Makefile` & `scikit-rmt-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/PKG-INFO` & `scikit-rmt-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scikit-rmt
-Version: 0.6.1
+Version: 0.7.0
 Summary: Random Matrix Theory Python package
 Home-page: https://github.com/AlejandroSantorum/scikit-rmt
 Author: Alejandro Santorum Varela
 Author-email: alejandro.santorum@gmail.com
 License: BSD
-Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.6.1.tar.gz
+Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.7.0.tar.gz
 Description: ![scikit-rmt logo](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scikit-rmt_logo_bigger.png)
         
         
         [![PyPI](https://img.shields.io/pypi/v/scikit-rmt?color=g)](https://pypi.org/project/scikit-rmt/)
         [![Documentation Status](https://readthedocs.org/projects/scikit-rmt/badge/?version=latest)](https://scikit-rmt.readthedocs.io/en/latest/?badge=latest)
         [![Build Status](https://travis-ci.com/AlejandroSantorum/scikit-rmt.svg?branch=main)](https://travis-ci.com/AlejandroSantorum/scikit-rmt)
         [![codecov](https://codecov.io/gh/AlejandroSantorum/scikit-rmt/branch/main/graph/badge.svg?token=56TNEASPJK)](https://codecov.io/gh/AlejandroSantorum/scikit-rmt)
```

### Comparing `scikit-rmt-0.6.1/README.md` & `scikit-rmt-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/conf.py` & `scikit-rmt-0.7.0/conf.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/docs/skrmt.covariance.rst` & `scikit-rmt-0.7.0/docs/skrmt.covariance.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/docs/skrmt.ensemble.rst` & `scikit-rmt-0.7.0/docs/skrmt.ensemble.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/examples/plot_boosting_density_representation.py` & `scikit-rmt-0.7.0/examples/plot_boosting_density_representation.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/examples/plot_circular_ensemble.py` & `scikit-rmt-0.7.0/examples/plot_circular_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/examples/plot_complex_histograms.py` & `scikit-rmt-0.7.0/examples/plot_complex_histograms.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/examples/plot_gaussian_ensemble.py` & `scikit-rmt-0.7.0/examples/plot_gaussian_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/examples/plot_manova_ensemble.py` & `scikit-rmt-0.7.0/examples/plot_manova_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/examples/plot_wishart_ensemble.py` & `scikit-rmt-0.7.0/examples/plot_wishart_ensemble.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/index.rst` & `scikit-rmt-0.7.0/index.rst`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/scikit_rmt.egg-info/PKG-INFO` & `scikit-rmt-0.7.0/scikit_rmt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scikit-rmt
-Version: 0.6.1
+Version: 0.7.0
 Summary: Random Matrix Theory Python package
 Home-page: https://github.com/AlejandroSantorum/scikit-rmt
 Author: Alejandro Santorum Varela
 Author-email: alejandro.santorum@gmail.com
 License: BSD
-Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.6.1.tar.gz
+Download-URL: https://github.com/AlejandroSantorum/scikit-rmt/archive/refs/tags/v0.7.0.tar.gz
 Description: ![scikit-rmt logo](https://raw.githubusercontent.com/AlejandroSantorum/scikit-rmt/main/imgs/scikit-rmt_logo_bigger.png)
         
         
         [![PyPI](https://img.shields.io/pypi/v/scikit-rmt?color=g)](https://pypi.org/project/scikit-rmt/)
         [![Documentation Status](https://readthedocs.org/projects/scikit-rmt/badge/?version=latest)](https://scikit-rmt.readthedocs.io/en/latest/?badge=latest)
         [![Build Status](https://travis-ci.com/AlejandroSantorum/scikit-rmt.svg?branch=main)](https://travis-ci.com/AlejandroSantorum/scikit-rmt)
         [![codecov](https://codecov.io/gh/AlejandroSantorum/scikit-rmt/branch/main/graph/badge.svg?token=56TNEASPJK)](https://codecov.io/gh/AlejandroSantorum/scikit-rmt)
```

### Comparing `scikit-rmt-0.6.1/scikit_rmt.egg-info/SOURCES.txt` & `scikit-rmt-0.7.0/scikit_rmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/setup.py` & `scikit-rmt-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/skrmt/covariance/__init__.py` & `scikit-rmt-0.7.0/skrmt/covariance/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/skrmt/covariance/estimator.py` & `scikit-rmt-0.7.0/skrmt/covariance/estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/skrmt/covariance/metrics.py` & `scikit-rmt-0.7.0/skrmt/covariance/metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/skrmt/covariance/tests/test_estimator.py` & `scikit-rmt-0.7.0/skrmt/covariance/tests/test_estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/skrmt/covariance/tests/test_metrics.py` & `scikit-rmt-0.7.0/skrmt/covariance/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/__init__.py` & `scikit-rmt-0.7.0/skrmt/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/_base_ensemble.py` & `scikit-rmt-0.7.0/skrmt/ensemble/_base_ensemble.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,20 +27,27 @@
         matrix (numpy array): instance of the random matrix ensemble
             of size n times n.
         _eigvals (numpy array): array of computed eigenvalues. This array
             is None until the method `eigvals` is called. The computed
             eigenvalues are cached in the attribute _eigvals to avoid
             re-computing them. The eigenvalues are re-calculated again
             if the matrix sample changes.
+        eigval_norm_cost (float): constant that is used to normalize the
+            eigenvalues so their support is always the same independently
+            of the sample size. This is really useful for plotting, since
+            the representation interval will always be the same no matter
+            how many eigenvalues are sampled.
     """
 
     @abstractmethod
     def __init__(self):
         self.matrix = None
         self._eigvals = None
+        # default eigenvalue normalization constant
+        self.eigval_norm_const = 1.0
 
     @abstractmethod
     def sample(self):
         """Samples new random matrix.
 
         The sampling algorithm depends on the inherited classes, so it should be
         specified by them.
@@ -54,29 +61,49 @@
     @abstractmethod
     def set_size(self):
         # pylint: disable=unnecessary-pass
         # pylint: disable=missing-function-docstring
         # this will be commented at inherited classes
         pass
 
+    def set_eigval_norm_const(self, eigval_norm_const):
+        """Sets a custom eigenvalue normalization constant.
+
+        This updates the normalization constant applied to the computed eigenvalues.
+        Eigenvalue normalization is useful because normalized eigenvalues always have
+        the same support independently of the sample size.
+
+        Args:
+            eigval_norm_const (float): new eigenvalue normalization constant.
+        """
+        # pylint: disable=unnecessary-pass
+        self.eigval_norm_const = eigval_norm_const
+
     @abstractmethod
-    def eigvals(self):
+    def eigvals(self, normalize=False):
         # pylint: disable=unnecessary-pass
         # pylint: disable=missing-function-docstring
         # this will be commented at inherited classes
         pass
 
     @abstractmethod
     def joint_eigval_pdf(self):
         # pylint: disable=unnecessary-pass
         # pylint: disable=missing-function-docstring
         # this will be commented at inherited classes
         pass
 
-    def eigval_hist(self, bins, interval=None, density=False, norm_const=None, avoid_img=False):
+    def eigval_hist(
+        self,
+        bins,
+        interval=None,
+        density=False,
+        normalize=True,
+        avoid_img=False
+    ):
         """Calculates the histogram of the matrix eigenvalues.
 
         Calculates the histogram of the current sampled matrix eigenvalues. Some ensembles
         like Gaussian (Hermite) ensemble or Wishart (Laguerre) ensemble might have
         improved routines to avoid calculating the eigenvalues, so instead the histogram
         is built using certain techniques to boost efficiency.
         It is important to underline that this function works with real eigenvalues,
@@ -90,18 +117,18 @@
             interval (tuple): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
-            norm_const (float, default=None): Eigenvalue normalization constant. By default,
-                it is set to None, so eigenvalues are not normalized. However, it is advisable
-                to specify a normalization constant to observe eigenvalue spectrum, e.g.
-                1/sqrt(n/2) if you want to analyze Wigner's Semicircular Law.
+            normalize (bool, default=True): Whether to normalize the computed eigenvalues
+                by the default normalization constant (see references). Defaults to True, i.e.,
+                the eigenvalues are normalized. Normalization makes the eigenvalues to be in the
+                same support independently of the sample size.
             avoid_img (bool, default=False): If True, eigenvalue imaginary part is ignored.
                 This should be used when the eigenvalue compatation is expected to generate
                 complex eigenvalues with really small imaginary part because of computing
                 rounding errors. E.g.: MANOVA Ensemble eigenvalues.
 
         Returns:
             (tuple) tuple containing:
@@ -125,28 +152,33 @@
 
         """
         if interval is not None:
             if not isinstance(interval, tuple):
                 raise ValueError("interval argument must be a tuple")
 
         # calculating eigenvalues using standard algorithm
-        eigvals = self.eigvals()
+        eigvals = self.eigvals(normalize=normalize)
         # ignoring imaginary part because of computing rounding errors
         if avoid_img:
             eigvals = eigvals.real
 
-        if norm_const:
-            eigvals = norm_const*eigvals
-
         # using numpy to obtain histogram in the given interval and no. of bins
         observed, bins = np.histogram(eigvals, bins=bins, range=interval, density=density)
         return observed, bins
 
 
-    def plot_eigval_hist(self, bins, interval=None, density=False, norm_const=None, fig_path=None, avoid_img=False):
+    def plot_eigval_hist(
+        self,
+        bins,
+        interval=None,
+        density=False,
+        normalize=True,
+        fig_path=None,
+        avoid_img=False
+    ):
         """Computes and plots the histogram of the matrix eigenvalues.
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
         Some ensembles like Gaussian (Hermite) ensemble or Wishart (Laguerre) ensemble
         have improved routines to avoid calculating the eigenvalues, so the histogram
         is built using certain techniques to boost efficiency. It is important to
         underline that this function works with real and complex eigenvalues: if the
@@ -161,18 +193,18 @@
             interval (tuple): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
-            norm_const (float, default=None): Eigenvalue normalization constant. By default,
-                it is set to None, so eigenvalues are not normalized. However, it is advisable
-                to specify a normalization constant to observe eigenvalue spectrum, e.g.
-                1/sqrt(n/2) if you want to analyze Wigner's Semicircular Law.
+            normalize (bool, default=True): Whether to normalize the computed eigenvalues
+                by the default normalization constant (see references). Defaults to True, i.e.,
+                the eigenvalues are normalized. Normalization makes the eigenvalues to be in the
+                same support independently of the sample size.
             avoid_img (bool, default=False): If True, eigenvalue imaginary part is ignored.
                 This should be used when the eigenvalue compatation is expected to generate
                 complex eigenvalues with really small imaginary part because of computing
                 rounding errors. E.g.: MANOVA Ensemble eigenvalues.
             fig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
 
@@ -186,19 +218,19 @@
 
         """
         # pylint: disable=too-many-arguments
         if not isinstance(interval, tuple):
             raise ValueError("interval argument must be a tuple")
 
         observed, bins = self.eigval_hist(bins=bins, interval=interval, density=density,
-                                          norm_const=norm_const, avoid_img=avoid_img)
+                                          normalize=normalize, avoid_img=avoid_img)
         width = bins[1]-bins[0]
         plt.bar(bins[:-1], observed, width=width, align='edge')
 
-        plt.title("Eigenvalue density histogram", fontweight="bold")
+        plt.title("Eigenvalue histogram", fontweight="bold")
         plt.xlabel("x")
         plt.ylabel("density")
 
         # Saving plot or showing it
         if fig_path:
             plt.savefig(fig_path, dpi=1200)
         else:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/circular_ensemble.py` & `scikit-rmt-0.7.0/skrmt/ensemble/circular_ensemble.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,14 +88,15 @@
                 and CSE are of size 2n times 2n.
 
         """
         super().__init__()
         # pylint: disable=invalid-name
         self.n = n
         self.beta = beta
+        self._eigvals = None
         self.matrix = self.sample()
 
     def set_size(self, n, resample_mtx=False):
         # pylint: disable=arguments-differ
         """Setter of matrix size.
 
         Sets the matrix size. Useful if it has been initialized with a different value.
@@ -195,37 +196,38 @@
         inds = np.arange(size-1)
         # selecting upper-diagonal indices
         j_mtx[inds, inds+1] = -1
         # selecting lower-diagonal indices
         j_mtx[inds+1, inds] = 1
         return j_mtx
 
-    def eigvals(self):
+    def eigvals(self, normalize=False):
         """Calculates the random matrix eigenvalues.
 
         Calculates the random matrix eigenvalues using numpy standard procedure.
         If the matrix ensemble is symmetric, a faster algorithm is used.
 
         Returns:
             numpy array with the calculated eigenvalues.
 
         """
+        norm_const = self.eigval_norm_const if normalize else 1.0
         if self._eigvals is not None:
-            return self._eigvals
+            return norm_const * self._eigvals
 
         if self.beta == 1:
             # using eigvalsh because it's known all eigenvalues are real
             self._eigvals = np.linalg.eigvalsh(self.matrix)
         else:
             # using eigvals since some eigenvalues could be imaginary
             self._eigvals = np.linalg.eigvals(self.matrix)
 
-        return self._eigvals
+        return norm_const * self._eigvals
 
-    def plot_eigval_hist(self, bins, interval=None, density=False, norm_const=None, fig_path=None):
+    def plot_eigval_hist(self, bins, interval=None, density=False, normalize=True, fig_path=None):
         """Computes and plots the histogram of the matrix eigenvalues.
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
         It is important to underline that this function works with real and complex
         eigenvalues: if the matrix eigenvalues are complex, they are plotted in the
         complex plane next to a heap map to study eigenvalue density.
 
@@ -237,32 +239,34 @@
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
-            norm_const (float, default=None): Eigenvalue normalization constant. By default,
-                it is set to None, so eigenvalues are not normalized. However, it is advisable
-                to specify a normalization constant to observe eigenvalue spectrum, e.g.
-                1/sqrt(n/2) if you want to analyze Wigner's Semicircular Law.
+            normalize (bool, default=True): Whether to normalize the computed eigenvalues
+                by the default normalization constant (see references). Defaults to True, i.e.,
+                the eigenvalues are normalized. Normalization makes the eigenvalues to be in the
+                same support independently of the sample size.
             fig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
 
         References:
             - Killip, R. and Zozhan, R.
                 Matrix Models and Eigenvalue Statistics for Truncations of
                 Classical Ensembles of Random Unitary Matrices.
                 Communications in Mathematical Physics. 349 (2017): 991-1027.
 
         """
         # pylint: disable=too-many-arguments
         # pylint: disable=too-many-locals
         if self.beta == 1:
-            return super().plot_eigval_hist(bins, interval, density, norm_const, fig_path)
+            return super().plot_eigval_hist(
+                bins=bins, interval=interval, density=density, normalize=normalize, fig_path=fig_path
+            )
 
         if (interval is not None) and not isinstance(interval, tuple):
             raise ValueError("interval argument must be a tuple (or None)")
 
         eigvals = self.eigvals()
         xvals = eigvals.real
         yvals = eigvals.imag
@@ -279,29 +283,28 @@
         fig.set_figheight(5)
         fig.set_figwidth(13)
         fig.subplots_adjust(hspace=.5)
 
         axes[0].set_xlim(rang[0][0], rang[0][1])
         axes[0].set_ylim(rang[1][0], rang[1][1])
         axes[0].plot(xvals, yvals, 'o')
-        axes[0].set_title('Eigenvalue plot')
+        axes[0].set_title('Complex plane')
         axes[0].set_xlabel('real')
         axes[0].set_ylabel('imaginary')
 
         h2d,_,_,img = axes[1].hist2d(xvals, yvals, range=rang,
                                    cmap=plt.cm.get_cmap('nipy_spectral'))
         fig.colorbar(img, ax=axes[1])
         axes[1].cla()
         axes[1].imshow(h2d.transpose(), origin='lower', interpolation="bilinear", extent=extent)
-        axes[1].set_title('Heatmap eigenvalue plot')
+        axes[1].set_title('Eigenvalue heatmap')
         axes[1].set_xlabel('real')
         axes[1].set_ylabel('imaginary')
 
-        plt.suptitle("matrix size: "+\
-                      str(len(self.matrix))+"x"+str(len(self.matrix)), fontweight="bold")
+        plt.suptitle("Complex eigenvalues histogram", fontweight="bold")
 
         # Saving plot or showing it
         if fig_path:
             plt.savefig(fig_path, dpi=600)
         else:
             plt.show()
```

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/gaussian_ensemble.py` & `scikit-rmt-0.7.0/skrmt/ensemble/gaussian_ensemble.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,16 +83,23 @@
 
         super().__init__()
         # pylint: disable=invalid-name
         self.n = n
         self.beta = beta
         self.use_tridiagonal = use_tridiagonal
         self.sigma = sigma
+        self._eigvals = None
         self.matrix = self.sample()
 
+        # default eigenvalue normalization constant
+        if self.use_tridiagonal:
+            self.eigval_norm_const = 1/np.sqrt(self.n) if self.beta==4 else 1/np.sqrt(self.n/2)
+        else:
+            self.eigval_norm_const = 1/np.sqrt(self.n)
+
 
     def set_size(self, n, resample_mtx=True):
         # pylint: disable=arguments-differ
         """Setter of matrix size.
 
         Sets the matrix size. Useful if it has been initialized with a different value.
 
@@ -206,41 +213,48 @@
         mtx = sparse.diags(diagonals, [-1, 0, 1])
         # converting to numpy array
         self.matrix = mtx.toarray()
         # setting array of eigenvalues to None to force re-computing them
         self._eigvals = None
         return self.matrix
 
-    def eigvals(self):
+    def eigvals(self, normalize=False):
         """Computes the random matrix eigenvalues.
 
         Calculates the random matrix eigenvalues using numpy standard procedure.
         If the matrix ensemble is symmetric, a faster algorithm is used.
 
         Returns:
             numpy array with the calculated eigenvalues.
 
         """
+        norm_const = self.eigval_norm_const if normalize else 1.0
+
         if self._eigvals is not None:
-            return self._eigvals
+            return norm_const * self._eigvals
 
+        # always storing non-normalized eigenvalues
         self._eigvals = np.linalg.eigvalsh(self.matrix)
-        return self._eigvals
+        return norm_const * self._eigvals
 
-    def eigval_hist(self, bins, interval=None, density=False, norm_const=None, avoid_img=False):
+    def eigval_hist(self, bins, interval=None, density=False, normalize=True, avoid_img=False):
         if self.use_tridiagonal:
-            if norm_const:
-                return tridiag_eigval_hist(self.matrix*norm_const, bins=bins,
-                                           interval=interval, density=density)
+            if normalize:
+                return tridiag_eigval_hist(
+                    self.eigval_norm_const * self.matrix,
+                    bins=bins,
+                    interval=interval,
+                    density=density,
+                )
             return tridiag_eigval_hist(self.matrix, bins=bins, interval=interval, density=density)
 
         return super().eigval_hist(bins, interval=interval, density=density,
-                                   norm_const=norm_const, avoid_img=avoid_img)
+                                   normalize=normalize, avoid_img=avoid_img)
 
-    def plot_eigval_hist(self, bins=100, interval=None, density=False, norm_const=None, fig_path=None):
+    def plot_eigval_hist(self, bins=100, interval=None, density=False, normalize=True, fig_path=None):
         """Computes and plots the histogram of the matrix eigenvalues.
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
         Gaussian (Hermite) ensemble and Wishart (Laguerre) ensemble have improved
         routines to avoid calculating the eigenvalues, so the histogram
         is built using certain techniques to boost efficiency.
 
@@ -252,18 +266,18 @@
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
-            norm_const (float, default=None): Eigenvalue normalization constant. By default,
-                it is set to None, so eigenvalues are not normalized. However, it is advisable
-                to specify a normalization constant to observe eigenvalue spectrum, e.g.
-                1/sqrt(n/2) if you want to analyze Wigner's Semicircular Law.
+            normalize (bool, default=True): Whether to normalize the computed eigenvalues
+                by the default normalization constant (see references). Defaults to True, i.e.,
+                the eigenvalues are normalized. Normalization makes the eigenvalues to be in the
+                same support independently of the sample size.
             fig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
 
         References:
             - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
@@ -271,38 +285,41 @@
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
         if interval is None:
             wsl_radius = 2*np.sqrt(self.beta)*self.sigma
             interval = (-wsl_radius, wsl_radius)
+
         if self.use_tridiagonal:
             # pylint: disable=too-many-arguments
-            if norm_const is None:
-                norm_const = 1/np.sqrt(self.n) if self.beta==4 else 1/np.sqrt(self.n/2)
+            observed, bins = self.eigval_hist(
+                bins=bins, interval=interval, density=density, normalize=normalize
+            )
 
-            observed, bins = tridiag_eigval_hist(self.matrix*norm_const, bins=bins,
-                                                 interval=interval, density=density)
             width = bins[1]-bins[0]
             plt.bar(bins[:-1], observed, width=width, align='edge')
-            plt.title("Eigenvalue density histogram", fontweight="bold")
+            plt.title("Eigenvalue histogram", fontweight="bold")
             plt.xlabel("x")
             plt.ylabel("density")
             # Saving plot or showing it
             if fig_path:
                 plt.savefig(fig_path, dpi=1000)
             else:
                 plt.show()
 
         else:
             # pylint: disable=too-many-arguments
-            if norm_const is None:
-                norm_const = 1/np.sqrt(self.n)
-            super().plot_eigval_hist(bins, interval=interval, density=density,
-                                     norm_const=norm_const, fig_path=fig_path)
+            super().plot_eigval_hist(
+                bins=bins,
+                interval=interval,
+                density=density,
+                normalize=normalize,
+                fig_path=fig_path,
+            )
 
     def joint_eigval_pdf(self, eigvals=None):
         '''Computes joint eigenvalue pdf.
 
         Calculates joint eigenvalue probability density function given an array of
         eigenvalues. If the array of eigenvalues is not provided, the current random
         matrix sample (so its eigenvalues) is used. This function depends on beta,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/manova_ensemble.py` & `scikit-rmt-0.7.0/skrmt/ensemble/manova_ensemble.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         """
         super().__init__()
         # pylint: disable=invalid-name
         self.m = m
         self.n1 = n1
         self.n2 = n2
         self.beta = beta
+        self._eigvals = None
         self.matrix = self.sample()
 
     def set_size(self, m, n1, n2, resample_mtx=True):
         # pylint: disable=arguments-differ
         """Setter of matrix size.
 
         Sets the matrix size. Useful if it has been initialized with a different value.
@@ -202,31 +203,34 @@
         a2_mtx = a1_mtx + np.matmul(y_mtx, y_mtx.transpose().conj())
         # A = (X * X') / (X * X' + Y * Y') = (X * X') * (X * X' + Y * Y')^(-1)
         self.matrix = np.matmul(a1_mtx, np.linalg.inv(a2_mtx))
         # setting array of eigenvalues to None to force re-computing them
         self._eigvals = None
         return self.matrix
 
-    def eigvals(self):
+    def eigvals(self, normalize=False):
         """Computes the random matrix eigenvalues.
 
         Calculates the random matrix eigenvalues using numpy standard procedure.
         If the matrix ensemble is symmetric, a faster algorithm is used.
 
         Returns:
             numpy array with the calculated eigenvalues.
 
         """
+        norm_const = self.eigval_norm_const if normalize else 1.0
+
         if self._eigvals is not None:
-            return self._eigvals
+            return norm_const * self._eigvals
 
+        # always storing non-normalized eigenvalues
         self._eigvals = np.linalg.eigvals(self.matrix)
-        return self._eigvals
+        return norm_const * self._eigvals
 
-    def plot_eigval_hist(self, bins, interval=(0,1), density=False, norm_const=None, fig_path=None):
+    def plot_eigval_hist(self, bins, interval=(0,1), density=False, normalize=True, fig_path=None):
         """Computes and plots the histogram of the matrix eigenvalues
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
 
         Args:
             bins (int or sequence): If bins is an integer, it defines the number of
                 equal-width bins in the range. If bins is a sequence, it defines the
@@ -235,33 +239,39 @@
             interval (tuple, default=(0,1)): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
-            norm_const (float, default=None): Eigenvalue normalization constant. By default,
-                it is set to None, so eigenvalues are not normalized. However, it is advisable
-                to specify a normalization constant to observe eigenvalue spectrum, e.g.
-                1/sqrt(n/2) if you want to analyze Wigner's Semicircular Law.
+            normalize (bool, default=True): Whether to normalize the computed eigenvalues
+                by the default normalization constant (see references). Defaults to True, i.e.,
+                the eigenvalues are normalized. Normalization makes the eigenvalues to be in the
+                same support independently of the sample size.
             fig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
 
         References:
             - Erdos, L. and Farrell, B.
                 "Local Eigenvalue Density for General MANOVA Matrices".
                 Journal of Statistical Physics. 152.6 (2013): 1003-1032.
             - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
         # pylint: disable=too-many-arguments
-        return super().plot_eigval_hist(bins, interval, density,
-                                        norm_const=norm_const, avoid_img=True, fig_path=fig_path)
+        return super().plot_eigval_hist(
+            bins=bins,
+            interval=interval,
+            density=density,
+            normalize=normalize,
+            fig_path=fig_path,
+            avoid_img=True,
+        )
 
     def joint_eigval_pdf(self, eigvals=None):
         '''Computes joint eigenvalue pdf.
 
         Calculates joint eigenvalue probability density function given an array of
         eigenvalues. If the array of eigenvalues is not provided, the current random
         matrix sample (so its eigenvalues) is used. This function depends on beta,
```

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/spectral_law.py` & `scikit-rmt-0.7.0/skrmt/ensemble/spectral_law.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,15 +248,15 @@
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
             interval = (self.center - self.radius - 0.1, self.center + self.radius + 0.1)
         
         _plot_func(
-            interval, func=self.pdf, bins=bins, 
+            interval, func=self.pdf, bins=bins, plot_title="Wigner Semicircle law PDF", 
             plot_ylabel="probability density", savefig_path=savefig_path
         )
     
     def plot_cdf(self, interval=None, bins=1000, savefig_path=None):
         """Plots the CDF of the Wigner Semicircle Law.
 
         Args:
@@ -268,20 +268,20 @@
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
             interval = (self.center - self.radius - 0.1, self.center + self.radius + 0.1)
         
         _plot_func(
-            interval, func=self.cdf, bins=bins, 
+            interval, func=self.cdf, bins=bins, plot_title="Wigner Semicircle law CDF",
             plot_ylabel="cumulative distribution", savefig_path=savefig_path
         )
     
 
-    def plot_empirical_pdf(self, n_size=1000, bins=100, interval=None, density=False,
+    def plot_empirical_pdf(self, n_size=10000, bins=100, interval=None, density=False,
                            plot_law_pdf=False, savefig_path=None):
         """Computes and plots Wigner's semicircle empirical law.
 
         Calculates and plots Wigner's semicircle empirical law using random samples generated
         using the relationship between the Wigner Semicircle law and the Beta distribution:
         the Wigner's Semicircle distribution it is a scaled Beta distribution with parameters
         :math:`\alpha = \beta = 3/2`.
@@ -314,14 +314,17 @@
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
         # pylint: disable=too-many-arguments
         if n_size<1:
             raise ValueError("matrix size must be positive")
+        
+        if interval is None:
+            interval = (-self.radius, self.radius)
 
         random_samples = self.rvs(size=n_size)
         observed, bins = np.histogram(random_samples, bins=bins, range=interval, density=density)
 
         width = bins[1]-bins[0]
         plt.bar(bins[:-1], observed, width=width, align='edge')
 
@@ -419,19 +422,18 @@
         
         _n = int(np.round(size / self.ratio))
 
         if not self._wishart_ens:
             self._wishart_ens = WishartEnsemble(beta=self.beta, p=size, n=_n, use_tridiagonal=False, sigma=self.sigma)
         else:
             self._wishart_ens.set_size(p=size, n=_n, resample_mtx=True)
-        
-        _eigval_norm_const = 1/_n 
+
         if self.beta == 4:
-            return _eigval_norm_const * self._wishart_ens.eigvals()[::2]
-        return _eigval_norm_const * self._wishart_ens.eigvals()
+            return self._wishart_ens.eigvals(normalize=True)[::2]
+        return self._wishart_ens.eigvals(normalize=True)
 
     def pdf(self, x):
         """Computes PDF of the Marchenko-Pastur Law.
 
         Args:
             x (float or ndarray): value or (numpy) array of values in which compute the PDF.
         
@@ -500,15 +502,15 @@
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
             interval = (self.lambda_minus, self.lambda_plus)
         
         _plot_func(
-            interval, func=self.pdf, bins=bins, 
+            interval, func=self.pdf, bins=bins, plot_title="Marchenko-Pastur law PDF",
             plot_ylabel="probability density", savefig_path=savefig_path
         )
     
     def plot_cdf(self, interval=None, bins=1000, savefig_path=None):
         """Plots the CDF of the Marchenko-Pastur Law.
 
         Args:
@@ -520,15 +522,15 @@
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
             interval = (self.lambda_minus, self.lambda_plus)
         
         _plot_func(
-            interval, func=self.cdf, bins=bins, 
+            interval, func=self.cdf, bins=bins, plot_title="Marchenko-Pastur law CDF",
             plot_ylabel="cumulative distribution", savefig_path=savefig_path
         )
 
     def plot_empirical_pdf(self, n_size=3000, p_size=None, bins=100, interval=None,
                            density=False, plot_law_pdf=False, savefig_path=None):
         """Computes and plots Marchenko-Pastur empirical law using Wishart Ensemble random matrices.
 
@@ -614,31 +616,28 @@
             print(f"Warning: The given scale is not the standard (sigma = {self.sigma}).\n"
                 "\t Tridiagonal histogramming is deactivated.\n"
                 "\t It is adviced to set sigma=1.0 to optimize and boost histogramming.")
 
         ens = WishartEnsemble(beta=self.beta, p=p_size, n=n_size, sigma=self.sigma,
                             use_tridiagonal=(use_tridiag_ratio and use_tridiag_sigma))
 
-        # Wigner eigenvalue normalization constant
-        norm_const = 1/n_size 
+        observed, bins = ens.eigval_hist(bins=bins, interval=interval, density=density, normalize=True)
 
-        observed, bins = ens.eigval_hist(bins=bins, interval=interval,
-                                         density=density, norm_const=norm_const)
         width = bins[1]-bins[0]
         plt.bar(bins[:-1], observed, width=width, align='edge')
 
         # Plotting theoretical graphic
         if plot_law_pdf and density:
             centers = np.array(_get_bins_centers_and_contour(bins))
             # creating new instance with the approximated ratio depending on the given matrix sizes
             mpd = MarchenkoPasturDistribution(beta=self.beta, ratio=approx_ratio, sigma=self.sigma)
             pdf = mpd.pdf(centers)
             plt.plot(centers, pdf, color='red', linewidth=2)
 
-        plt.title("Marchenko-Pastur Law - Empirical density histogram", fontweight="bold")
+        plt.title("Marchenko-Pastur Law - Eigenvalue histogram", fontweight="bold")
         plt.xlabel("x")
         plt.ylabel("probability density")
         if approx_ratio > 1:
             if plot_law_pdf and density:
                 ylim_vals = pdf
             else:
                 ylim_vals = observed
@@ -725,15 +724,15 @@
         if mtx_size <= 0:
             raise ValueError(f"Error: invalid matrix size. It has to be positive. Provided matrix size = {mtx_size}.")
 
         self._gaussian_ens = GaussianEnsemble(beta=self.beta, n=mtx_size, use_tridiagonal=False)
 
         max_eigvals = []
         for _ in range(size):
-            max_eigvals.append(self._gaussian_ens.eigvals().max())
+            max_eigvals.append(self._gaussian_ens.eigvals(normalize=False).max())
             self._gaussian_ens.sample()
         max_eigvals = np.asarray(max_eigvals)
 
         # Tracy-Widom eigenvalue distr. normalization constants
         eigval_scale = 1.0
         size_scale = 1.0
         if self.beta == 2:
@@ -781,15 +780,15 @@
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
             interval = (-5, 4-self.beta)
         
         _plot_func(
-            interval, func=self.pdf, bins=bins, 
+            interval, func=self.pdf, bins=bins, plot_title="Tracy-Widom law PDF",
             plot_ylabel="probability density", savefig_path=savefig_path
         )
     
     def plot_cdf(self, interval=None, bins=1000, savefig_path=None):
         """Plots the PDF of the Tracy-Widom Law.
 
         Args:
@@ -801,15 +800,15 @@
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
             interval = (-5, 4-self.beta)
         
         _plot_func(
-            interval, func=self.cdf, bins=bins, 
+            interval, func=self.cdf, bins=bins, plot_title="Tracy-Widom law CDF",
             plot_ylabel="cumulative distribution", savefig_path=savefig_path
         )
 
     def plot_empirical_pdf(self, n_size=100, times=1000, bins=100, interval=None,
                            density=False, plot_law_pdf=False, savefig_path=None):
         """Computes and plots Tracy-Widom empirical law using Gaussian Ensemble.
 
@@ -851,15 +850,15 @@
         if n_size<1 or times<1:
             raise ValueError("matrix size or number of repetitions must be positive")
 
         ens = GaussianEnsemble(beta=self.beta, n=n_size, use_tridiagonal=False)
 
         eigvals = []
         for _ in range(times):
-            eigvals.append(ens.eigvals().max())
+            eigvals.append(ens.eigvals(normalize=False).max())
             ens.sample()
         eigvals = np.asarray(eigvals)
 
         # Tracy-Widom eigenvalue distr. normalization constants
         eigval_scale = 1.0
         size_scale = 1.0
         if self.beta == 2:
@@ -881,15 +880,15 @@
 
         # Plotting theoretical graphic
         if plot_law_pdf and density:
             centers = _get_bins_centers_and_contour(bins)
             pdf = self.pdf(centers)
             plt.plot(centers, pdf, color='red', linewidth=2)
 
-        plt.title("Tracy-Widom Law - Empirical density histogram", fontweight="bold")
+        plt.title("Tracy-Widom Law - Eigenvalue histogram", fontweight="bold")
         plt.xlabel("x")
         plt.ylabel("probability density")
 
         # Saving plot or showing it
         if savefig_path:
             plt.savefig(savefig_path, dpi=1200)
         else:
@@ -981,19 +980,19 @@
         _n1 = int(np.round(size * self.a))
         _n2 = int(np.round(size * self.b))
 
         if not self._manova_ens:
             self._manova_ens = ManovaEnsemble(beta=self.beta, m=size, n1=_n1, n2=_n2)
         else:
             self._manova_ens.set_size(m=size, n1=_n1, n2=_n2, resample_mtx=True)
-        
-        # Here, _eigval_norm_const = 1.0
+
+        # normalization here is not crucial since the default normalization const. of Manova is 1.0
         if self.beta == 4:
-            return self._manova_ens.eigvals()[::2].real
-        return self._manova_ens.eigvals().real
+            return self._manova_ens.eigvals(normalize=True)[::2].real
+        return self._manova_ens.eigvals(normalize=True).real
     
     def pdf(self, x):
         """Computes PDF of the Manova Spectrum distribution.
 
         Args:
             x (float or ndarray): value or (numpy) array of values in which compute the PDF.
         
@@ -1048,15 +1047,15 @@
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
             interval = (self.lambda_minus, self.lambda_plus)
         
         _plot_func(
-            interval, func=self.pdf, bins=bins, 
+            interval, func=self.pdf, bins=bins, plot_title="Manova spectrum PDF",
             plot_ylabel="probability density", savefig_path=savefig_path
         )
 
     def plot_cdf(self, interval=None, bins=1000, savefig_path=None):
         """Plots the CDF of the Manova Spectrum distribution.
 
         Args:
@@ -1068,15 +1067,15 @@
                 provided, the plot is shown at the end of the routine.
         
         """
         if interval is None:
             interval = (self.lambda_minus, self.lambda_plus)
 
         _plot_func(
-            interval, func=self.cdf, bins=bins, 
+            interval, func=self.cdf, bins=bins, plot_title="Manova spectrum CDF",
             plot_ylabel="cumulative distribution", savefig_path=savefig_path
         )
 
     def plot_empirical_pdf(self, m_size=1000, n1_size=None, n2_size=None, bins=100, interval=None,
                            density=False, plot_law_pdf=False, savefig_path=None):
         """Computes and plots Manova spectrum empirical pdf and analytical distribution.
 
@@ -1159,28 +1158,34 @@
             interval = [lambda_minus, lambda_plus]
             if approx_a <= 1:
                 interval[0] = min(-0.05, lambda_minus)
             if approx_b <= 1:
                 interval[1] = max(lambda_plus, 1.05)
             interval = tuple(interval)
 
-        observed, bins = ens.eigval_hist(bins=bins, interval=interval, density=density, avoid_img=True)
+        observed, bins = ens.eigval_hist(
+            bins=bins,
+            interval=interval,
+            density=density,
+            normalize=True,
+            avoid_img=True
+        )
 
         width = bins[1]-bins[0]
         plt.bar(bins[:-1], observed, width=width, align='edge')
 
         # Plotting theoretical graphic
         if plot_law_pdf and density:
             centers = np.array(_get_bins_centers_and_contour(bins))
             # creating new instance with the approximated ratios depending on the given matrix sizes
             msd = ManovaSpectrumDistribution(beta=self.beta, a=approx_a, b=approx_b)
             pdf = msd.pdf(centers)
             plt.plot(centers, pdf, color='red', linewidth=2)
 
-        plt.title("Manova Spectrum - Empirical density histogram", fontweight="bold")
+        plt.title("Manova Spectrum - Eigenvalue histogram", fontweight="bold")
         plt.xlabel("x")
         plt.ylabel("probability density")
         if approx_a <= 1 or approx_b <= 1:
             if plot_law_pdf and density:
                 ylim_vals = pdf
             else:
                 ylim_vals = observed
```

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/tests/test_circular_ens.py` & `scikit-rmt-0.7.0/skrmt/ensemble/tests/test_circular_ens.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/tests/test_gaussian_ens.py` & `scikit-rmt-0.7.0/skrmt/ensemble/tests/test_gaussian_ens.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,42 +116,42 @@
     goe1 = GaussianEnsemble(beta=1, n=n_size, use_tridiagonal=False)
     goe2 = GaussianEnsemble(beta=1, n=n_size, use_tridiagonal=True)
 
     goe1.matrix = goe2.matrix
 
     nbins = 10
     interval = (-2,2)
-    to_norm = False # without normalization
+    to_norm = False # without density normalization
     # calculating histogram using standard naive procedure
     hist_nottridiag, bins_nottridiag = goe1.eigval_hist(bins=nbins, interval=interval,
-                                                        density=to_norm)
+                                                        density=to_norm, normalize=False)
     # calculating histogram using tridiagonal procedure
     hist_tridiag, bins_tridiag = goe2.eigval_hist(bins=nbins, interval=interval,
-                                                  density=to_norm)
+                                                  density=to_norm, normalize=False)
     assert_array_equal(bins_nottridiag, bins_tridiag)
     assert_array_equal(hist_nottridiag, hist_tridiag)
 
-    to_norm = True # normalization
+    to_norm = True # density normalization
     # calculating histogram using standard naive procedure
     hist_nottridiag, bins_nottridiag = goe1.eigval_hist(bins=nbins, interval=interval,
-                                                        density=to_norm)
+                                                        density=to_norm, normalize=False)
     # calculating histogram using tridiagonal procedure
     hist_tridiag, bins_tridiag = goe2.eigval_hist(bins=nbins, interval=interval,
-                                                  density=to_norm)
+                                                  density=to_norm, normalize=False)
 
     assert_array_equal(bins_nottridiag, bins_tridiag)
     assert_array_equal(hist_nottridiag, hist_tridiag)
 
-    const = 1/np.sqrt(n_size/2)
+    to_norm = False # no density normalization
     # calculating histogram using standard naive procedure
     hist_nottridiag, bins_nottridiag = goe1.eigval_hist(bins=nbins, interval=interval,
-                                                        density=to_norm, norm_const=const)
+                                                        density=to_norm, normalize=False)
     # calculating histogram using tridiagonal procedure
     hist_tridiag, bins_tridiag = goe2.eigval_hist(bins=nbins, interval=interval,
-                                                  density=to_norm, norm_const=const)
+                                                  density=to_norm, normalize=False)
 
     assert_array_equal(bins_nottridiag, bins_tridiag)
     assert_array_equal(hist_nottridiag, hist_tridiag)
 
 
 
 ##########################################
@@ -235,31 +235,31 @@
     gue1 = GaussianEnsemble(beta=2, n=n_size, use_tridiagonal=False)
     gue2 = GaussianEnsemble(beta=2, n=n_size, use_tridiagonal=True)
 
     gue1.matrix = gue2.matrix
 
     nbins = 10
     interval = (-2,2)
-    to_norm = False # without normalization
+    to_norm = False # without density normalization
     # calculating histogram using standard naive procedure
     hist_nottridiag, bins_nottridiag = gue1.eigval_hist(bins=nbins, interval=interval,
-                                                        density=to_norm)
+                                                        density=to_norm, normalize=False)
     # calculating histogram using tridiagonal procedure
     hist_tridiag, bins_tridiag = gue2.eigval_hist(bins=nbins, interval=interval,
-                                                  density=to_norm)
+                                                  density=to_norm, normalize=False)
     assert_array_equal(bins_nottridiag, bins_tridiag)
     assert_array_equal(hist_nottridiag, hist_tridiag)
 
-    to_norm = True # normalization
+    to_norm = True # density normalization
     # calculating histogram using standard naive procedure
     hist_nottridiag, bins_nottridiag = gue1.eigval_hist(bins=nbins, interval=interval,
-                                                        density=to_norm)
+                                                        density=to_norm, normalize=False)
     # calculating histogram using tridiagonal procedure
     hist_tridiag, bins_tridiag = gue2.eigval_hist(bins=nbins, interval=interval,
-                                                  density=to_norm)
+                                                  density=to_norm, normalize=False)
     assert_array_equal(bins_nottridiag, bins_tridiag)
     assert_array_equal(hist_nottridiag, hist_tridiag)
 
 
 ##########################################
 ### Gaussian Symplectic Ensemble = GSE
 
@@ -343,26 +343,26 @@
     gse1 = GaussianEnsemble(beta=4, n=n_size, use_tridiagonal=False)
     gse2 = GaussianEnsemble(beta=4, n=n_size, use_tridiagonal=True)
 
     gse1.matrix = gse2.matrix
 
     nbins = 10
     interval = (-2,2)
-    to_norm = False # without normalization
+    to_norm = False # without density normalization
     # calculating histogram using standard naive procedure
     hist_nottridiag, bins_nottridiag = gse1.eigval_hist(bins=nbins, interval=interval,
-                                                        density=to_norm)
+                                                        density=to_norm, normalize=False)
     # calculating histogram using tridiagonal procedure
     hist_tridiag, bins_tridiag = gse2.eigval_hist(bins=nbins, interval=interval,
-                                                  density=to_norm)
+                                                  density=to_norm, normalize=False)
     assert_array_equal(bins_nottridiag, bins_tridiag)
     assert_array_equal(hist_nottridiag, hist_tridiag)
 
-    to_norm = True # normalization
+    to_norm = True # density normalization
     # calculating histogram using standard naive procedure
     hist_nottridiag, bins_nottridiag = gse1.eigval_hist(bins=nbins, interval=interval,
-                                                        density=to_norm)
+                                                        density=to_norm, normalize=False)
     # calculating histogram using tridiagonal procedure
     hist_tridiag, bins_tridiag = gse2.eigval_hist(bins=nbins, interval=interval,
-                                                  density=to_norm)
+                                                  density=to_norm, normalize=False)
     assert_array_equal(bins_nottridiag, bins_tridiag)
     assert_array_equal(hist_nottridiag, hist_tridiag)
```

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/tests/test_manova_ens.py` & `scikit-rmt-0.7.0/skrmt/ensemble/tests/test_manova_ens.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/tests/test_spectral_law.py` & `scikit-rmt-0.7.0/skrmt/ensemble/tests/test_spectral_law.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/tests/test_tracy_widom_approx.py` & `scikit-rmt-0.7.0/skrmt/ensemble/tests/test_tracy_widom_approx.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/tests/test_tridiagonalization.py` & `scikit-rmt-0.7.0/skrmt/ensemble/tests/test_tridiagonalization.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/tests/test_wishart_ens.py` & `scikit-rmt-0.7.0/skrmt/ensemble/tests/test_wishart_ens.py`

 * *Files 5% similar despite different names*

```diff
@@ -149,32 +149,32 @@
     # calculating histogram using tridiagonal procedure
     hist_tridiag, bins_tridiag = wre2.eigval_hist(bins=nbins, interval=interval,
                                                   density=to_norm)
 
     assert_array_equal(bins_nottridiag, bins_tridiag)
     assert_array_equal(hist_nottridiag, hist_tridiag)
 
-    to_norm = True # normalization
+    to_norm = True # density normalization
     # calculating histogram using standard naive procedure
     hist_nottridiag, bins_nottridiag = wre1.eigval_hist(bins=nbins, interval=interval,
-                                                        density=to_norm)
+                                                        density=to_norm, normalize=True)
     # calculating histogram using tridiagonal procedure
     hist_tridiag, bins_tridiag = wre2.eigval_hist(bins=nbins, interval=interval,
-                                                  density=to_norm)
+                                                  density=to_norm, normalize=True)
 
     assert_array_equal(bins_nottridiag, bins_tridiag)
     assert_almost_equal(hist_nottridiag, hist_tridiag, decimal=7)
 
-    const = 1/n_size
+    to_norm = False # no density normalization
     # calculating histogram using standard naive procedure
     hist_nottridiag, bins_nottridiag = wre1.eigval_hist(bins=nbins, interval=interval,
-                                                        density=to_norm, norm_const=const)
+                                                        density=to_norm, normalize=True)
     # calculating histogram using tridiagonal procedure
     hist_tridiag, bins_tridiag = wre2.eigval_hist(bins=nbins, interval=interval,
-                                                  density=to_norm, norm_const=const)
+                                                  density=to_norm, normalize=True)
 
     assert_array_equal(bins_nottridiag, bins_tridiag)
     assert_array_equal(hist_nottridiag, hist_tridiag)
 
 
 ##########################################
 ### Wishart Complex Ensemble = WCE
```

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/tracy_widom_approximator.py` & `scikit-rmt-0.7.0/skrmt/ensemble/tracy_widom_approximator.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/tridiagonal_utils.py` & `scikit-rmt-0.7.0/skrmt/ensemble/tridiagonal_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/skrmt/ensemble/wishart_ensemble.py` & `scikit-rmt-0.7.0/skrmt/ensemble/wishart_ensemble.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,15 +92,18 @@
         super().__init__()
         # pylint: disable=invalid-name
         self.p = p
         self.n = n
         self.beta = beta
         self.use_tridiagonal = use_tridiagonal
         self.sigma = sigma
+        self._eigvals = None
         self.matrix = self.sample()
+        # default eigenvalue normalization constant
+        self.eigval_norm_const = 1/self.n
 
     def set_size(self, p, n, resample_mtx=True):
         # pylint: disable=arguments-differ
         """Setter of matrix size.
 
         Sets the matrix size. Useful if it has been initialized with a different value.
 
@@ -230,40 +233,48 @@
         # converting to numpy array
         self.matrix = mtx.toarray()
         # setting array of eigenvalues to None to force re-computing them
         self._eigvals = None
         return self.matrix
 
 
-    def eigvals(self):
+    def eigvals(self, normalize=False):
         """Computes the random matrix eigenvalues.
 
         Calculates the random matrix eigenvalues using numpy standard procedure.
         If the matrix ensemble is symmetric, a faster algorithm is used.
 
         Returns:
             numpy array with the calculated eigenvalues.
 
         """
+        norm_const = self.eigval_norm_const if normalize else 1.0
+
         if self._eigvals is not None:
-            return self._eigvals
+            return norm_const * self._eigvals
 
+        # always storing non-normalized eigenvalues
         self._eigvals = np.linalg.eigvalsh(self.matrix)
-        return self._eigvals
+        return norm_const * self._eigvals
 
-    def eigval_hist(self, bins, interval=None, density=False, norm_const=None, avoid_img=False):
+    def eigval_hist(self, bins, interval=None, density=False, normalize=True, avoid_img=False):
         if self.use_tridiagonal:
-            if norm_const:
-                return tridiag_eigval_hist(self.matrix*norm_const, bins=bins,
-                                           interval=interval, density=density)
+            if normalize:
+                return tridiag_eigval_hist(
+                    self.eigval_norm_const * self.matrix,
+                    bins=bins,
+                    interval=interval,
+                    density=density,
+                )
             return tridiag_eigval_hist(self.matrix, bins=bins, interval=interval, density=density)
 
-        return super().eigval_hist(bins, interval, density, norm_const, avoid_img=avoid_img)
+        return super().eigval_hist(bins, interval=interval, density=density,
+                                   normalize=normalize, avoid_img=avoid_img)
 
-    def plot_eigval_hist(self, bins=100, interval=None, density=False, norm_const=None, fig_path=None):
+    def plot_eigval_hist(self, bins=100, interval=None, density=False, normalize=True, fig_path=None):
         """Computes and plots the histogram of the matrix eigenvalues.
 
         Calculates and plots the histogram of the current sampled matrix eigenvalues.
         Gaussian (Hermite) ensemble and Wishart (Laguerre) ensemble have improved
         routines to avoid calculating the eigenvalues, so the histogram
         is built using certain techniques to boost efficiency.
 
@@ -275,56 +286,65 @@
             interval (tuple, default=None): Delimiters (xmin, xmax) of the histogram.
                 The lower and upper range of the bins. Lower and upper outliers are ignored.
             density (bool, default=False): If True, draw and return a probability
                 density: each bin will display the bin's raw count divided by the total
                 number of counts and the bin width, so that the area under the histogram
                 integrates to 1. If set to False, the absolute frequencies of the eigenvalues
                 are returned.
-            norm_const (float, default=None): Eigenvalue normalization constant. By default,
-                it is set to None, so eigenvalues are not normalized. However, it is advisable
-                to specify a normalization constant to observe eigenvalue spectrum, e.g.
-                1/sqrt(n/2) if you want to analyze Wigner's Semicircular Law.
+            normalize (bool, default=True): Whether to normalize the computed eigenvalues
+                by the default normalization constant (see references). Defaults to True, i.e.,
+                the eigenvalues are normalized. Normalization makes the eigenvalues to be in the
+                same support independently of the sample size.
             fig_path (string, default=None): path to save the created figure. If it is not
                 provided, the plot is shown at the end of the routine.
 
         References:
             - Albrecht, J. and Chan, C.P. and Edelman, A.
                 "Sturm sequences and random eigenvalue distributions".
                 Foundations of Computational Mathematics. 9.4 (2008): 461-483.
             - Dumitriu, I. and Edelman, A.
                 "Matrix Models for Beta Ensembles".
                 Journal of Mathematical Physics. 43.11 (2002): 5830-5847.
 
         """
+        if not normalize:
+            print("Warning: setting normalize=False may cause normal instability and/or rounding errors.")
+
         # pylint: disable=too-many-arguments
-        if norm_const is None:
-            norm_const = 1/self.n 
         if interval is None:
             # calculating constants depending on matrix sizes
             ratio = self.p/self.n
             lambda_plus = self.beta * self.sigma**2 * (1 + np.sqrt(ratio))**2
             lambda_minus = self.beta * self.sigma**2 * (1 - np.sqrt(ratio))**2
             interval = (lambda_minus, lambda_plus)
 
         if self.use_tridiagonal:
-            observed, bins = tridiag_eigval_hist(self.matrix*norm_const, bins=bins,
-                                                 interval=interval, density=density)
+            observed, bins = self.eigval_hist(
+                bins=bins, interval=interval, density=density, normalize=normalize
+            )
+
             width = bins[1]-bins[0]
             plt.bar(bins[:-1], observed, width=width, align='edge')
-            plt.title("Eigenvalue density histogram", fontweight="bold")
+            plt.title("Eigenvalue histogram", fontweight="bold")
             plt.xlabel("x")
             plt.ylabel("density")
             # Saving plot or showing it
             if fig_path:
                 plt.savefig(fig_path, dpi=1000)
             else:
                 plt.show()
 
         else:
-            super().plot_eigval_hist(bins, interval, density, norm_const, fig_path)
+            super().plot_eigval_hist(
+                bins=bins,
+                interval=interval,
+                density=density,
+                normalize=normalize,
+                fig_path=fig_path,
+            )
 
     def joint_eigval_pdf(self, eigvals=None):
         '''Computes joint eigenvalue pdf.
 
         Calculates joint eigenvalue probability density function given an array of
         eigenvalues. If the array of eigenvalues is not provided, the current random
         matrix sample (so its eigenvalues) is used. This function depends on beta,
```

### Comparing `scikit-rmt-0.6.1/tutorial/plot_0_introduction.py` & `scikit-rmt-0.7.0/tutorial/plot_0_introduction.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,8 +57,8 @@
 
 ##############################################################################
 # To study its eigenvalue spectrum, its size should be a little bit larger.
 
 from skrmt.ensemble import GaussianEnsemble
 
 goe = GaussianEnsemble(beta=1, n=1000)
-goe.plot_eigval_hist(bins=60, interval=(-2,2))
+goe.plot_eigval_hist(bins=80)
```

### Comparing `scikit-rmt-0.6.1/tutorial/plot_1_spectral_laws.py` & `scikit-rmt-0.7.0/tutorial/plot_1_spectral_laws.py`

 * *Files identical despite different names*

### Comparing `scikit-rmt-0.6.1/tutorial/plot_2_plot_spectral_laws.py` & `scikit-rmt-0.7.0/tutorial/plot_2_plot_spectral_laws.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,48 +28,49 @@
 ##############################################################################
 # As an example, we can try to plot the spectral density of the Gaussian
 # Orthogonal Ensemble (GOE) in the interval (-10, 10).
 
 from skrmt.ensemble import GaussianEnsemble
 
 goe = GaussianEnsemble(beta=1, n=1000)
-goe.plot_eigval_hist(bins=80, interval=(-10, 10), norm_const=1)
+goe.plot_eigval_hist(bins=80, interval=(-10, 10), normalize=False)
 
 ##############################################################################
 # As we can see, the histogram does not explain barely anything about
 # the ensemble. That is because we are not using correctly the theory
 # behind the model.
 #
 # Most of the ensembles need their eigenvalues to be normalized by a
 # certain constant in order to perceive their limiting density properly.
 # By default, the scikit-rmt is implemented to normalize eigenvalues
 # with the more suitable constant depending on the ensemble.
 
 ##############################################################################
 # In the former example, GOE matrices of size :math:`n \times n` should be
-# normalized by :math:`1/\sqrt{n}`. 
+# normalized by :math:`1/\sqrt{n}`, which is done by default or by setting
+# `normalize=True`. 
 
 import numpy as np
 from skrmt.ensemble import GaussianEnsemble
 
 n=1000
 goe = GaussianEnsemble(beta=1, n=n)
-goe.plot_eigval_hist(bins=80, interval=(-10, 10), norm_const=1/np.sqrt(n))
+goe.plot_eigval_hist(bins=80, interval=(-10, 10), normalize=True)
 
 ##############################################################################
 # Additionally, we can control the plotting interval to get a better picture
 # of the spectral density. In the GOE case, the spectral distribution is
 # concentrated in the (-2,2) interval.
 
 import numpy as np
 from skrmt.ensemble import GaussianEnsemble
 
 n=1000
 goe = GaussianEnsemble(beta=1, n=n)
-goe.plot_eigval_hist(bins=80, interval=(-2, 2), norm_const=1/np.sqrt(n))
+goe.plot_eigval_hist(bins=80, interval=(-2, 2), normalize=True)
 
 ##############################################################################
 # This example would be equivalent for Gaussian Unitary Ensemble (GUE) and
 # Gaussian Symplectic Ensemble (GSE).
 
 ##############################################################################
 # Another example would be using the Wishart Ensemble. In the following
@@ -78,22 +79,22 @@
 from skrmt.ensemble import WishartEnsemble
 
 p, n = 1000, 3000
 wre = WishartEnsemble(beta=1, p=p, n=n)
 wre.plot_eigval_hist(bins=80, interval=(-5,5))
 
 ##############################################################################
-# By not specifying the normalization constant, the library has taken charge
-# of it by itself. The plotting interval still can be improved.
+# By default, scikit-rmt takes charge of using the most suitable plotting
+# interval and eigenvalue normalization constant.
 
 from skrmt.ensemble import WishartEnsemble
 
 p, n = 1000, 3000
 wre = WishartEnsemble(beta=1, p=p, n=n)
-wre.plot_eigval_hist(bins=80, interval=(0.2, 2.2))
+wre.plot_eigval_hist(bins=80)
 
 ##############################################################################
 # This example would be equivalent for Wishart Complex Ensemble (WCE) and
 # Wishart Quaternion Ensemble (WQE), with the detail of controlling its
 # representation interval.
 
 ##############################################################################
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

