# Comparing `tmp/creativecontrol-circuitpython-ltc166x-1.2.1.tar.gz` & `tmp/creativecontrol-circuitpython-ltc166x-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creativecontrol-circuitpython-ltc166x-1.2.1.tar", last modified: Fri Jul  7 02:37:00 2023, max compression
+gzip compressed data, was "creativecontrol-circuitpython-ltc166x-1.2.2.tar", last modified: Sat Jul  8 23:21:59 2023, max compression
```

## Comparing `creativecontrol-circuitpython-ltc166x-1.2.1.tar` & `creativecontrol-circuitpython-ltc166x-1.2.2.tar`

### file list

```diff
@@ -1,38 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:37:00.722333 creativecontrol-circuitpython-ltc166x-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:37:00.718333 creativecontrol-circuitpython-ltc166x-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:37:00.718333 creativecontrol-circuitpython-ltc166x-1.2.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:37:00.718333 creativecontrol-circuitpython-ltc166x-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:37:00.722333 creativecontrol-circuitpython-ltc166x-1.2.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-07 02:37:00.722333 creativecontrol-circuitpython-ltc166x-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:37:00.722333 creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-07 02:37:00.000000 creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 02:37:00.000000 creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 02:37:00.000000 creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-07 02:37:00.000000 creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 02:37:00.000000 creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-07 02:36:52.000000 creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:37:00.722333 creativecontrol-circuitpython-ltc166x-1.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-07 02:36:52.000000 creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_dac_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-07 02:36:52.000000 creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_dac_list_selective.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-07 02:36:52.000000 creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_dac_value_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-07 02:36:52.000000 creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_single_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-07 02:36:52.000000 creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_single_value_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-07 02:36:52.000000 creativecontrol-circuitpython-ltc166x-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 02:37:00.722333 creativecontrol-circuitpython-ltc166x-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.670340 creativecontrol-circuitpython-ltc166x-1.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.662340 creativecontrol-circuitpython-ltc166x-1.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.666340 creativecontrol-circuitpython-ltc166x-1.2.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.666340 creativecontrol-circuitpython-ltc166x-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.666340 creativecontrol-circuitpython-ltc166x-1.2.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-08 23:21:59.670340 creativecontrol-circuitpython-ltc166x-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.666340 creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-08 23:21:59.000000 creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-08 23:21:59.000000 creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 23:21:59.000000 creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-08 23:21:59.000000 creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 23:21:59.000000 creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-08 23:21:51.000000 creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.666340 creativecontrol-circuitpython-ltc166x-1.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.670340 creativecontrol-circuitpython-ltc166x-1.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.670340 creativecontrol-circuitpython-ltc166x-1.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-08 23:21:51.000000 creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_dac_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-08 23:21:51.000000 creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_dac_list_selective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-08 23:21:51.000000 creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_dac_value_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-08 23:21:51.000000 creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_single_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-08 23:21:51.000000 creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_single_value_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-08 23:21:51.000000 creativecontrol-circuitpython-ltc166x-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 23:21:59.670340 creativecontrol-circuitpython-ltc166x-1.2.2/setup.cfg
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `creativecontrol-circuitpython-ltc166x-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/.github/workflows/release_gh.yml` & `creativecontrol-circuitpython-ltc166x-1.2.2/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/.github/workflows/release_pypi.yml` & `creativecontrol-circuitpython-ltc166x-1.2.2/.github/workflows/release_pypi.yml`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/.gitignore` & `creativecontrol-circuitpython-ltc166x-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/.pre-commit-config.yaml` & `creativecontrol-circuitpython-ltc166x-1.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/.pylintrc` & `creativecontrol-circuitpython-ltc166x-1.2.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/CODE_OF_CONDUCT.md` & `creativecontrol-circuitpython-ltc166x-1.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/LICENSE` & `creativecontrol-circuitpython-ltc166x-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/LICENSES/CC-BY-4.0.txt` & `creativecontrol-circuitpython-ltc166x-1.2.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/LICENSES/MIT.txt` & `creativecontrol-circuitpython-ltc166x-1.2.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/LICENSES/Unlicense.txt` & `creativecontrol-circuitpython-ltc166x-1.2.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/PKG-INFO` & `creativecontrol-circuitpython-ltc166x-1.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creativecontrol-circuitpython-ltc166x
-Version: 1.2.1
+Version: 1.2.2
 Summary: CircuitPython library for control of LTC166X 8-bit and 10-bit DACs.
 Author-email: creativecontrol <t@creativecontrol.cc>
 License: MIT
 Project-URL: Homepage, https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X
 Keywords: adafruit,blinka,circuitpython,micropython,creativecontrol_circuitpython_ltc166x,LTC1660,LTC1665,DAC
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -23,24 +23,26 @@
 
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 
-.. image:: https://github.com/creativecontrol/CircuitPython_creativecontrol_CircuitPython_LTC166X/workflows/Build%20CI/badge.svg
-    :target: https://github.com/creativecontrol/CircuitPython_creativecontrol_CircuitPython_LTC166X/actions
+.. image:: https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X/actions/workflows/build.yml/badge.svg
+    :target: https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X/actions/workflows/build.yml
     :alt: Build Status
 
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-CircuitPython library for control of LTC1665 8-bit and LTC1660 10-bit DACs from Linear Technologies.
+=================================
+
+CircuitPython library for control of LTC1665 8-bit and LTC1660 10-bit 8 channel DACs from Linear Technologies.
 
 `LTC166X datasheet <https://www.analog.com/media/en/technical-documentation/data-sheets/166560fa.pdf>`_
 
 Multiple LTC1665/LTC1660’s can be controlled from a single 3-wire serial port (i.e., SCK, DIN and CS/LD) by
 using the included “daisy-chain” facility. A series of *n* chips is configured by connecting each DOUT (except the
 last) to DIN of the next chip, forming a single 16n-bit shift register. The SCK and CS/LD signals are common
 to all chips in the chain. In use, CS/LD is held low while *n* 16-bit words are clocked to DIN of the first chip; CS/LD
@@ -113,15 +115,15 @@
 
 .. code-block:: shell
 
    import time
    import board
    import creativecontrol_circuitpython_ltc166x
 
-   ltc1665 = creativecontrol_circuitpython_ltc166x.LTC1665(cs=board.GP1, sck=board.GP2, mosi=board.GP3, debug=True)
+   ltc1665 = creativecontrol_circuitpython_ltc166x.LTC1665(csel=board.GP1, sck=board.GP2, mosi=board.GP3, debug=True)
 
    dac_values = [1, 3, 7, 15, 31, 63, 127, 255]
 
    while True:
         print('writing dac values ', time.monotonic())
         ltc1665.write_dac_values(dac_values)
         time.sleep(4)
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/README.rst` & `creativecontrol-circuitpython-ltc166x-1.2.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 
-.. image:: https://github.com/creativecontrol/CircuitPython_creativecontrol_CircuitPython_LTC166X/workflows/Build%20CI/badge.svg
-    :target: https://github.com/creativecontrol/CircuitPython_creativecontrol_CircuitPython_LTC166X/actions
+.. image:: https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X/actions/workflows/build.yml/badge.svg
+    :target: https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X/actions/workflows/build.yml
     :alt: Build Status
 
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-CircuitPython library for control of LTC1665 8-bit and LTC1660 10-bit DACs from Linear Technologies.
+=================================
+
+CircuitPython library for control of LTC1665 8-bit and LTC1660 10-bit 8 channel DACs from Linear Technologies.
 
 `LTC166X datasheet <https://www.analog.com/media/en/technical-documentation/data-sheets/166560fa.pdf>`_
 
 Multiple LTC1665/LTC1660’s can be controlled from a single 3-wire serial port (i.e., SCK, DIN and CS/LD) by
 using the included “daisy-chain” facility. A series of *n* chips is configured by connecting each DOUT (except the
 last) to DIN of the next chip, forming a single 16n-bit shift register. The SCK and CS/LD signals are common
 to all chips in the chain. In use, CS/LD is held low while *n* 16-bit words are clocked to DIN of the first chip; CS/LD
@@ -95,15 +97,15 @@
 
 .. code-block:: shell
 
    import time
    import board
    import creativecontrol_circuitpython_ltc166x
 
-   ltc1665 = creativecontrol_circuitpython_ltc166x.LTC1665(cs=board.GP1, sck=board.GP2, mosi=board.GP3, debug=True)
+   ltc1665 = creativecontrol_circuitpython_ltc166x.LTC1665(csel=board.GP1, sck=board.GP2, mosi=board.GP3, debug=True)
 
    dac_values = [1, 3, 7, 15, 31, 63, 127, 255]
 
    while True:
         print('writing dac values ', time.monotonic())
         ltc1665.write_dac_values(dac_values)
         time.sleep(4)
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO` & `creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creativecontrol-circuitpython-ltc166x
-Version: 1.2.1
+Version: 1.2.2
 Summary: CircuitPython library for control of LTC166X 8-bit and 10-bit DACs.
 Author-email: creativecontrol <t@creativecontrol.cc>
 License: MIT
 Project-URL: Homepage, https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X
 Keywords: adafruit,blinka,circuitpython,micropython,creativecontrol_circuitpython_ltc166x,LTC1660,LTC1665,DAC
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -23,24 +23,26 @@
 
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 
-.. image:: https://github.com/creativecontrol/CircuitPython_creativecontrol_CircuitPython_LTC166X/workflows/Build%20CI/badge.svg
-    :target: https://github.com/creativecontrol/CircuitPython_creativecontrol_CircuitPython_LTC166X/actions
+.. image:: https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X/actions/workflows/build.yml/badge.svg
+    :target: https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X/actions/workflows/build.yml
     :alt: Build Status
 
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-CircuitPython library for control of LTC1665 8-bit and LTC1660 10-bit DACs from Linear Technologies.
+=================================
+
+CircuitPython library for control of LTC1665 8-bit and LTC1660 10-bit 8 channel DACs from Linear Technologies.
 
 `LTC166X datasheet <https://www.analog.com/media/en/technical-documentation/data-sheets/166560fa.pdf>`_
 
 Multiple LTC1665/LTC1660’s can be controlled from a single 3-wire serial port (i.e., SCK, DIN and CS/LD) by
 using the included “daisy-chain” facility. A series of *n* chips is configured by connecting each DOUT (except the
 last) to DIN of the next chip, forming a single 16n-bit shift register. The SCK and CS/LD signals are common
 to all chips in the chain. In use, CS/LD is held low while *n* 16-bit words are clocked to DIN of the first chip; CS/LD
@@ -113,15 +115,15 @@
 
 .. code-block:: shell
 
    import time
    import board
    import creativecontrol_circuitpython_ltc166x
 
-   ltc1665 = creativecontrol_circuitpython_ltc166x.LTC1665(cs=board.GP1, sck=board.GP2, mosi=board.GP3, debug=True)
+   ltc1665 = creativecontrol_circuitpython_ltc166x.LTC1665(csel=board.GP1, sck=board.GP2, mosi=board.GP3, debug=True)
 
    dac_values = [1, 3, 7, 15, 31, 63, 127, 255]
 
    while True:
         print('writing dac values ', time.monotonic())
         ltc1665.write_dac_values(dac_values)
         time.sleep(4)
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.py` & `creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 CircuitPython library for control of LTC166X 8-bit and 10-bit DACs.
 
 
 * Author(s): Thadeus Frazier-Reed
 
 Implementation Notes
 --------------------
+The library provides options for storing all DAC values in a list
+or a list of lists for DAC daisy-chains.
+A channel may be marked for no update using a negative number (i.e. -1)
+This value will be skipped or a no change message will be sent in the case of a daisy-change.
 
 **TODO:**
 
 * Add Sleep and Wake control
-* Add example for multiple chained DACs
-
 
 * Influenced by
   http://www.kerrywong.com/2010/05/02/a-library-for-ltc1665ltc1660/
 
 **Hardware:**
 
 * Linear Technologies LTC166X datasheet:
@@ -47,15 +49,15 @@
 """
 
 import microcontroller
 from busio import SPI
 import digitalio
 from adafruit_bus_device.spi_device import SPIDevice
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 __repo__ = (
     "https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X.git"
 )
 
 
 class LTC166X:
     """
@@ -123,24 +125,28 @@
     def write_chained_dac_values(self, dac_values: list):
         """
         Write list of values to a chain of DACs. All lists should be the same length.
         Do not update if value is < 0. This allows for comparison of
         update frames and only updating if value has changed.
 
         :param list dac_values: list of lists of values from 0 to device range.
-        Each list represents a DAC.
 
+        Each list represents a DAC's channel values.
         [[DAC 1], [DAC 2], [DAC 3], etc.]
         """
-        for index, _ in enumerate(dac_values[0]):
-            dac_chain_list = [dac[index] for dac in dac_values]
+        for dac_index, _ in enumerate(dac_values[0]):
+            dac_chain_list = [dac[dac_index] for dac in dac_values]
+            # DAC chain is reversed because of the way the shift register works.
+            dac_chain_list.reverse()
             with self._device as spi:
-                for chain_index, chain_value in enumerate(dac_chain_list):
+                for chain_value in dac_chain_list:
                     if chain_value >= 0:
-                        self.write_value_to_spi(spi, chain_value, chain_index + 1)
+                        self.write_value_to_spi(spi, chain_value, dac_index + 1)
+                    else:
+                        self.write_value_to_spi(spi, 0, 0)
 
     def write_chained_dac_value(self, value: list, address: int, chain_length: int):
         """
         Write a single DAC value to a chain.
 
         :param list value: DAC value from 0 to device range.
         :param int address: DAC address DAC A = 1 ... DAC H = 8 ... ALL DACs = 15.
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_dac_chain.py` & `creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_dac_chain.py`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_dac_list_selective.py` & `creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_dac_list_selective.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 # SPDX-FileCopyrightText: Copyright (c) 2023 Thadeus Frazier-Reed for creativecontrol
 #
 # SPDX-License-Identifier: Unlicense
 
 """
-Only update value if it has changed.
+Write random values to all DAC channels from a list. Only update value if it has changed.
 """
 
 import random
 import time
 import board
 import creativecontrol_circuitpython_ltc166x
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_dac_value_list.py` & `creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_dac_value_list.py`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_single_value.py` & `creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_single_value.py`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_single_value_sweep.py` & `creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_single_value_sweep.py`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.1/pyproject.toml` & `creativecontrol-circuitpython-ltc166x-1.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "creativecontrol-circuitpython-ltc166x"
 description = "CircuitPython library for control of LTC166X 8-bit and 10-bit DACs."
-version = "1.2.1"
+version = "1.2.2"
 readme = "README.rst"
 authors = [
     {name = "creativecontrol", email = "t@creativecontrol.cc"}
 ]
 urls = {Homepage = "https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X"}
 keywords = [
     "adafruit",
```

