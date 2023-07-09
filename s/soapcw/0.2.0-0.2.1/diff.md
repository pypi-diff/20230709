# Comparing `tmp/soapcw-0.2.0.tar.gz` & `tmp/soapcw-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soapcw-0.2.0.tar", last modified: Sat Jul  8 21:02:59 2023, max compression
+gzip compressed data, was "soapcw-0.2.1.tar", last modified: Sun Jul  9 20:37:39 2023, max compression
```

## Comparing `soapcw-0.2.0.tar` & `soapcw-0.2.1.tar`

### file list

```diff
@@ -1,96 +1,100 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.685006 soapcw-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-08 21:01:19.000000 soapcw-0.2.0/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     3508 2023-07-08 21:01:19.000000 soapcw-0.2.0/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-08 21:01:19.000000 soapcw-0.2.0/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-08 21:01:19.000000 soapcw-0.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-08 21:01:19.000000 soapcw-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2446 2023-07-08 21:02:59.685006 soapcw-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1377 2023-07-08 21:01:19.000000 soapcw-0.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.677006 soapcw-0.2.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      605 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/authors.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.677006 soapcw-0.2.0/docs/cnn_usage/
--rw-rw-rw-   0 root         (0) root         (0)     5902 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/cnn_usage/data_generation.rst
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/cnn_usage/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5625 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/cnn_usage/train_model.rst
--rwxrwxrwx   0 root         (0) root         (0)     4930 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/history.rst
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.677006 soapcw-0.2.0/docs/pipeline_usage/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/pipeline_usage/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     6633 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/pipeline_usage/run_pipeline.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/readme.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.677006 soapcw-0.2.0/docs/usage/
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-07-08 21:01:19.000000 soapcw-0.2.0/docs/usage/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.678006 soapcw-0.2.0/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.678006 soapcw-0.2.0/pipeline/css/
--rw-rw-rw-   0 root         (0) root         (0)     3163 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/css/general.css
--rwxrwxrwx   0 root         (0) root         (0)     7001 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/make_dag_files_astro.py
--rwxrwxrwx   0 root         (0) root         (0)     6963 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/make_dag_files_lines.py
--rw-rw-rw-   0 root         (0) root         (0)    38283 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/make_html_page.py
--rwxrwxrwx   0 root         (0) root         (0)    37058 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/run_full_soap_astro.py
--rwxrwxrwx   0 root         (0) root         (0)    40172 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/run_full_soap_lines.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.678006 soapcw-0.2.0/pipeline/scripts/
--rw-rw-rw-   0 root         (0) root         (0)    18806 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/scripts/table_scripts.js
--rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-08 21:01:19.000000 soapcw-0.2.0/pipeline/soap_config_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-08 21:02:59.686006 soapcw-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4209 2023-07-08 21:01:19.000000 soapcw-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.681006 soapcw-0.2.0/soapcw/
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.682006 soapcw-0.2.0/soapcw/cnn/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/cnn_data_dag_gen.py
--rwxrwxrwx   0 root         (0) root         (0)    17948 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/cnn_data_gen.py
--rw-rw-rw-   0 root         (0) root         (0)    12490 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/generate_gaussian_train_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11006 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/generate_test_data.py
--rw-rw-rw-   0 root         (0) root         (0)    20005 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/generate_train_data.py
--rwxrwxrwx   0 root         (0) root         (0)     5822 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/narrowband_sfts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.682006 soapcw-0.2.0/soapcw/cnn/pytorch/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/pytorch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4307 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/pytorch/load_models.py
--rw-rw-rw-   0 root         (0) root         (0)    15950 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/pytorch/models.py
--rw-rw-rw-   0 root         (0) root         (0)    14625 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cnn/train_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.683006 soapcw-0.2.0/soapcw/cw/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cw/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    43688 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cw/generate_data.py
--rw-rw-rw-   0 root         (0) root         (0)    19576 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cw/load_sfts.py
--rw-rw-rw-   0 root         (0) root         (0)     8660 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cw/make_sfts.py
--rw-rw-rw-   0 root         (0) root         (0)     9450 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cw/sft.py
--rw-rw-rw-   0 root         (0) root         (0)     8567 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cw/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/cw/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.683006 soapcw-0.2.0/soapcw/line_aware_stat/
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/line_aware_stat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11721 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/line_aware_stat/gen_lookup.pyx
--rw-rw-rw-   0 root         (0) root         (0)    38004 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/line_aware_stat/gen_lookup_python.py
--rwxrwxrwx   0 root         (0) root         (0)     6514 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/line_aware_stat/save_lookup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.684006 soapcw-0.2.0/soapcw/neville/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/neville/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1898 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/neville/load_models.py
--rw-rw-rw-   0 root         (0) root         (0)    23724 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/neville/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4753 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/neville/truncated_gauss.py
--rw-rw-rw-   0 root         (0) root         (0)     4331 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/soap_config_parser.py
--rw-r--r--   0 root         (0) root         (0)  2271838 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw/soapcw.c
--rw-rw-rw-   0 root         (0) root         (0)    65928 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/soapcw.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.684006 soapcw-0.2.0/soapcw/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/tools/plots.py
--rw-rw-rw-   0 root         (0) root         (0)     9044 2023-07-08 21:01:19.000000 soapcw-0.2.0/soapcw/tools/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.681006 soapcw-0.2.0/soapcw.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2446 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1945 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      484 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-08 21:02:59.000000 soapcw-0.2.0/soapcw.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 21:02:59.685006 soapcw-0.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)   445283 2023-07-08 21:01:19.000000 soapcw-0.2.0/tests/SNR_injections.ipynb
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-08 21:01:19.000000 soapcw-0.2.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2023-07-08 21:01:19.000000 soapcw-0.2.0/tests/test_cwload.py
--rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-08 21:01:19.000000 soapcw-0.2.0/tests/test_line_aware_stat.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-07-08 21:01:19.000000 soapcw-0.2.0/tests/test_soap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.945222 soapcw-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-05 17:01:34.000000 soapcw-0.2.1/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3508 2023-07-05 17:01:34.000000 soapcw-0.2.1/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-05 17:01:34.000000 soapcw-0.2.1/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-05 17:01:34.000000 soapcw-0.2.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-05 17:01:34.000000 soapcw-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-07-09 20:37:39.946222 soapcw-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2023-07-09 20:27:29.000000 soapcw-0.2.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.931222 soapcw-0.2.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      605 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/authors.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.932222 soapcw-0.2.1/docs/cnn_usage/
+-rw-rw-rw-   0 root         (0) root         (0)     5901 2023-07-09 19:50:12.000000 soapcw-0.2.1/docs/cnn_usage/data_generation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-07-09 19:50:12.000000 soapcw-0.2.1/docs/cnn_usage/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5625 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/cnn_usage/train_model.rst
+-rwxrwxrwx   0 root         (0) root         (0)     4930 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1237 2023-07-09 19:50:12.000000 soapcw-0.2.1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.933222 soapcw-0.2.1/docs/neville_usage/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-07-09 19:50:12.000000 soapcw-0.2.1/docs/neville_usage/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6072 2023-07-09 19:50:12.000000 soapcw-0.2.1/docs/neville_usage/load_model.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.933222 soapcw-0.2.1/docs/pipeline_usage/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/pipeline_usage/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6633 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/pipeline_usage/run_pipeline.rst
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/readme.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.934222 soapcw-0.2.1/docs/usage/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-07-05 17:01:34.000000 soapcw-0.2.1/docs/usage/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.935222 soapcw-0.2.1/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 20:34:56.000000 soapcw-0.2.1/pipeline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.935222 soapcw-0.2.1/pipeline/css/
+-rw-rw-rw-   0 root         (0) root         (0)     3163 2023-07-05 17:01:34.000000 soapcw-0.2.1/pipeline/css/general.css
+-rwxrwxrwx   0 root         (0) root         (0)     7001 2023-07-05 17:01:34.000000 soapcw-0.2.1/pipeline/make_dag_files_astro.py
+-rwxrwxrwx   0 root         (0) root         (0)     6963 2023-07-05 17:01:34.000000 soapcw-0.2.1/pipeline/make_dag_files_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)    38283 2023-07-05 17:01:34.000000 soapcw-0.2.1/pipeline/make_html_page.py
+-rwxrwxrwx   0 root         (0) root         (0)    37058 2023-07-06 15:04:52.000000 soapcw-0.2.1/pipeline/run_full_soap_astro.py
+-rwxrwxrwx   0 root         (0) root         (0)    40172 2023-07-05 17:01:34.000000 soapcw-0.2.1/pipeline/run_full_soap_lines.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.936222 soapcw-0.2.1/pipeline/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)    18806 2023-07-05 17:01:34.000000 soapcw-0.2.1/pipeline/scripts/table_scripts.js
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-05 17:01:34.000000 soapcw-0.2.1/pipeline/soap_config_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-09 20:37:39.947222 soapcw-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4209 2023-07-05 17:01:34.000000 soapcw-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.939222 soapcw-0.2.1/soapcw/
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-07-09 20:02:12.000000 soapcw-0.2.1/soapcw/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.941222 soapcw-0.2.1/soapcw/cnn/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/cnn_data_dag_gen.py
+-rwxrwxrwx   0 root         (0) root         (0)    17948 2023-07-06 15:04:52.000000 soapcw-0.2.1/soapcw/cnn/cnn_data_gen.py
+-rw-rw-rw-   0 root         (0) root         (0)    12490 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/generate_gaussian_train_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11006 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/generate_test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    20005 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/generate_train_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     5822 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/narrowband_sfts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.941222 soapcw-0.2.1/soapcw/cnn/pytorch/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/pytorch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4307 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/pytorch/load_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    15950 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cnn/pytorch/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    14625 2023-07-06 15:04:52.000000 soapcw-0.2.1/soapcw/cnn/train_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.942222 soapcw-0.2.1/soapcw/cw/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cw/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    43688 2023-07-08 20:43:38.000000 soapcw-0.2.1/soapcw/cw/generate_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    19576 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cw/load_sfts.py
+-rw-rw-rw-   0 root         (0) root         (0)     8660 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cw/make_sfts.py
+-rw-rw-rw-   0 root         (0) root         (0)     9450 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cw/sft.py
+-rw-rw-rw-   0 root         (0) root         (0)     8567 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cw/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/cw/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.943222 soapcw-0.2.1/soapcw/line_aware_stat/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/line_aware_stat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11721 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/line_aware_stat/gen_lookup.pyx
+-rw-rw-rw-   0 root         (0) root         (0)    38004 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/line_aware_stat/gen_lookup_python.py
+-rwxrwxrwx   0 root         (0) root         (0)     6514 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/line_aware_stat/save_lookup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.944222 soapcw-0.2.1/soapcw/neville/
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-07-09 19:50:12.000000 soapcw-0.2.1/soapcw/neville/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-07-08 20:43:38.000000 soapcw-0.2.1/soapcw/neville/load_models.py
+-rw-rw-rw-   0 root         (0) root         (0)    23724 2023-07-08 20:43:38.000000 soapcw-0.2.1/soapcw/neville/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2007 2023-07-09 19:50:12.000000 soapcw-0.2.1/soapcw/neville/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     4753 2023-07-08 20:43:38.000000 soapcw-0.2.1/soapcw/neville/truncated_gauss.py
+-rw-rw-rw-   0 root         (0) root         (0)     4331 2023-07-08 20:43:38.000000 soapcw-0.2.1/soapcw/soap_config_parser.py
+-rw-r--r--   0 root         (0) root         (0)  2271838 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw/soapcw.c
+-rw-rw-rw-   0 root         (0) root         (0)    65928 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/soapcw.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.944222 soapcw-0.2.1/soapcw/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 20:34:56.000000 soapcw-0.2.1/soapcw/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/tools/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     9044 2023-07-05 17:01:34.000000 soapcw-0.2.1/soapcw/tools/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.940222 soapcw-0.2.1/soapcw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      484 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-09 20:37:39.000000 soapcw-0.2.1/soapcw.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 20:37:39.945222 soapcw-0.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   445283 2023-07-05 17:01:34.000000 soapcw-0.2.1/tests/SNR_injections.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-05 17:01:34.000000 soapcw-0.2.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2023-07-05 17:01:34.000000 soapcw-0.2.1/tests/test_cwload.py
+-rw-rw-rw-   0 root         (0) root         (0)     3602 2023-07-05 17:01:34.000000 soapcw-0.2.1/tests/test_line_aware_stat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2023-07-05 17:01:34.000000 soapcw-0.2.1/tests/test_soap.py
```

### Comparing `soapcw-0.2.0/CONTRIBUTING.rst` & `soapcw-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/LICENSE` & `soapcw-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/PKG-INFO` & `soapcw-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soapcw
-Version: 0.2.0
+Version: 0.2.1
 Summary: SOAP is a rapid algorithm to search for continuous sources of gravitational waves, with a wider application to long duration narrowband signals.
 Home-page: https://git.ligo.org/joseph.bayley/soapcw
 Author: Joe Bayley
 Author-email: joseph.bayley@glasgow.ac.uk
 License: MIT license
 Download-URL: https://git.ligo.org/joseph.bayley/soapcw/-/archive/0.1.2/soapcw-0.1.2.tar.gz
 Keywords: soapcw,soap,gravitational waves,pulsars,neutron stars,continuous waves
```

### Comparing `soapcw-0.2.0/README.rst` & `soapcw-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/docs/Makefile` & `soapcw-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/docs/cnn_usage/data_generation.rst` & `soapcw-0.2.1/docs/cnn_usage/data_generation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .. highlight:: shell
 
 ============
-Pipeline usage
+Creating data
 ============
 
 SOAP is usually run as a pipeline on the LIGO detectors, 
 both searching for astrophysical signals and as a detector characterisation tool.
 
 The machine learning part of this method, mostly using CNNs to reduce the impact of instrumental artefacts, and how to use it is described below.
```

### Comparing `soapcw-0.2.0/docs/cnn_usage/train_model.rst` & `soapcw-0.2.1/docs/cnn_usage/train_model.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/docs/conf.py` & `soapcw-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/docs/index.rst` & `soapcw-0.2.1/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 =============
 
 .. toctree::
     :maxdepth: 2
    
     usage/index
     cnn_usage/index
+    neville_usage/index
     pipeline_usage/index
 
 
 Info
 =========
 
 .. toctree::
```

### Comparing `soapcw-0.2.0/docs/installation.rst` & `soapcw-0.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/docs/make.bat` & `soapcw-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/docs/pipeline_usage/run_pipeline.rst` & `soapcw-0.2.1/docs/pipeline_usage/run_pipeline.rst`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/pipeline/css/general.css` & `soapcw-0.2.1/pipeline/css/general.css`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/pipeline/make_dag_files_astro.py` & `soapcw-0.2.1/pipeline/make_dag_files_astro.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/pipeline/make_dag_files_lines.py` & `soapcw-0.2.1/pipeline/make_dag_files_lines.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/pipeline/make_html_page.py` & `soapcw-0.2.1/pipeline/make_html_page.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/pipeline/run_full_soap_astro.py` & `soapcw-0.2.1/pipeline/run_full_soap_astro.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/pipeline/run_full_soap_lines.py` & `soapcw-0.2.1/pipeline/run_full_soap_lines.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/pipeline/scripts/table_scripts.js` & `soapcw-0.2.1/pipeline/scripts/table_scripts.js`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/pipeline/soap_config_parser.py` & `soapcw-0.2.1/pipeline/soap_config_parser.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/setup.cfg` & `soapcw-0.2.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [bumpversion]
-current_version = 0.1.9
-new_version = 0.2.0
+current_version = 0.2.0
+new_version = 0.2.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
 
@@ -18,15 +18,15 @@
 [flake8]
 exclude = docs
 
 [aliases]
 
 [metadata]
 name = soapcw
-version = 0.2.0
+version = 0.2.1
 
 [options]
 packages = soapcw, pipeline
 
 [options.entry_points]
 console_scripts = 
 	soapcw-make-dag-files-lines = pipeline.make_dag_files_lines:main
```

### Comparing `soapcw-0.2.0/setup.py` & `soapcw-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/__init__.py` & `soapcw-0.2.1/soapcw/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import
 """Top-level package for soapcw."""
 
 __author__ = """Joe Bayley"""
 __email__ = 'joseph.bayley@glasgow.ac.uk'
-__version__ = '0.1.9'
+__version__ = '0.2.1'
 from .soapcw import single_detector, two_detector, three_detector, single_detector_gaps
 from .tools import tools, plots
 from .cnn import __init__
 from .neville import __init__
 from .line_aware_stat import __init__
 from .cw import __init__
 from . import soap_config_parser
```

### Comparing `soapcw-0.2.0/soapcw/cnn/cnn_data_dag_gen.py` & `soapcw-0.2.1/soapcw/cnn/cnn_data_dag_gen.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/cnn/cnn_data_gen.py` & `soapcw-0.2.1/soapcw/cnn/cnn_data_gen.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/cnn/generate_gaussian_train_data.py` & `soapcw-0.2.1/soapcw/cnn/generate_gaussian_train_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/cnn/generate_test_data.py` & `soapcw-0.2.1/soapcw/cnn/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/cnn/generate_train_data.py` & `soapcw-0.2.1/soapcw/cnn/generate_train_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/cnn/narrowband_sfts.py` & `soapcw-0.2.1/soapcw/cnn/narrowband_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/cnn/pytorch/load_models.py` & `soapcw-0.2.1/soapcw/cnn/pytorch/load_models.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/cnn/pytorch/models.py` & `soapcw-0.2.1/soapcw/cnn/pytorch/models.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/cnn/train_model.py` & `soapcw-0.2.1/soapcw/cnn/train_model.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/cw/generate_data.py` & `soapcw-0.2.1/soapcw/cw/generate_data.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/cw/load_sfts.py` & `soapcw-0.2.1/soapcw/cw/load_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/cw/make_sfts.py` & `soapcw-0.2.1/soapcw/cw/make_sfts.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/cw/sft.py` & `soapcw-0.2.1/soapcw/cw/sft.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/cw/timeseries.py` & `soapcw-0.2.1/soapcw/cw/timeseries.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/cw/tools.py` & `soapcw-0.2.1/soapcw/cw/tools.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/line_aware_stat/gen_lookup.pyx` & `soapcw-0.2.1/soapcw/line_aware_stat/gen_lookup.pyx`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/line_aware_stat/gen_lookup_python.py` & `soapcw-0.2.1/soapcw/line_aware_stat/gen_lookup_python.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/line_aware_stat/save_lookup.py` & `soapcw-0.2.1/soapcw/line_aware_stat/save_lookup.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/neville/load_models.py` & `soapcw-0.2.1/soapcw/neville/load_models.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/neville/models.py` & `soapcw-0.2.1/soapcw/neville/models.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/neville/truncated_gauss.py` & `soapcw-0.2.1/soapcw/neville/truncated_gauss.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/soap_config_parser.py` & `soapcw-0.2.1/soapcw/soap_config_parser.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/soapcw.c` & `soapcw-0.2.1/soapcw/soapcw.c`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/soapcw.pyx` & `soapcw-0.2.1/soapcw/soapcw.pyx`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/tools/plots.py` & `soapcw-0.2.1/soapcw/tools/plots.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw/tools/tools.py` & `soapcw-0.2.1/soapcw/tools/tools.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/soapcw.egg-info/PKG-INFO` & `soapcw-0.2.1/soapcw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soapcw
-Version: 0.2.0
+Version: 0.2.1
 Summary: SOAP is a rapid algorithm to search for continuous sources of gravitational waves, with a wider application to long duration narrowband signals.
 Home-page: https://git.ligo.org/joseph.bayley/soapcw
 Author: Joe Bayley
 Author-email: joseph.bayley@glasgow.ac.uk
 License: MIT license
 Download-URL: https://git.ligo.org/joseph.bayley/soapcw/-/archive/0.1.2/soapcw-0.1.2.tar.gz
 Keywords: soapcw,soap,gravitational waves,pulsars,neutron stars,continuous waves
```

### Comparing `soapcw-0.2.0/soapcw.egg-info/SOURCES.txt` & `soapcw-0.2.1/soapcw.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/cnn_usage/data_generation.rst
 docs/cnn_usage/index.rst
 docs/cnn_usage/train_model.rst
+docs/neville_usage/index.rst
+docs/neville_usage/load_model.rst
 docs/pipeline_usage/index.rst
 docs/pipeline_usage/run_pipeline.rst
 docs/usage/index.rst
 pipeline/__init__.py
 pipeline/make_dag_files_astro.py
 pipeline/make_dag_files_lines.py
 pipeline/make_html_page.py
@@ -63,14 +65,15 @@
 soapcw/line_aware_stat/__init__.py
 soapcw/line_aware_stat/gen_lookup.pyx
 soapcw/line_aware_stat/gen_lookup_python.py
 soapcw/line_aware_stat/save_lookup.py
 soapcw/neville/__init__.py
 soapcw/neville/load_models.py
 soapcw/neville/models.py
+soapcw/neville/tools.py
 soapcw/neville/truncated_gauss.py
 soapcw/tools/__init__.py
 soapcw/tools/plots.py
 soapcw/tools/tools.py
 tests/SNR_injections.ipynb
 tests/__init__.py
 tests/test_cwload.py
```

### Comparing `soapcw-0.2.0/tests/SNR_injections.ipynb` & `soapcw-0.2.1/tests/SNR_injections.ipynb`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/tests/test_cwload.py` & `soapcw-0.2.1/tests/test_cwload.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/tests/test_line_aware_stat.py` & `soapcw-0.2.1/tests/test_line_aware_stat.py`

 * *Files identical despite different names*

### Comparing `soapcw-0.2.0/tests/test_soap.py` & `soapcw-0.2.1/tests/test_soap.py`

 * *Files identical despite different names*

