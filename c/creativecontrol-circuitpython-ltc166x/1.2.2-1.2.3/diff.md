# Comparing `tmp/creativecontrol-circuitpython-ltc166x-1.2.2.tar.gz` & `tmp/creativecontrol-circuitpython-ltc166x-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creativecontrol-circuitpython-ltc166x-1.2.2.tar", last modified: Sat Jul  8 23:21:59 2023, max compression
+gzip compressed data, was "creativecontrol-circuitpython-ltc166x-1.2.3.tar", last modified: Sun Jul  9 18:30:07 2023, max compression
```

## Comparing `creativecontrol-circuitpython-ltc166x-1.2.2.tar` & `creativecontrol-circuitpython-ltc166x-1.2.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.670340 creativecontrol-circuitpython-ltc166x-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.662340 creativecontrol-circuitpython-ltc166x-1.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.666340 creativecontrol-circuitpython-ltc166x-1.2.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.666340 creativecontrol-circuitpython-ltc166x-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.666340 creativecontrol-circuitpython-ltc166x-1.2.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-08 23:21:59.670340 creativecontrol-circuitpython-ltc166x-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.666340 creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-08 23:21:59.000000 creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-08 23:21:59.000000 creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 23:21:59.000000 creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-08 23:21:59.000000 creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 23:21:59.000000 creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-08 23:21:51.000000 creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.666340 creativecontrol-circuitpython-ltc166x-1.2.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.670340 creativecontrol-circuitpython-ltc166x-1.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:21:59.670340 creativecontrol-circuitpython-ltc166x-1.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-08 23:21:51.000000 creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_dac_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-08 23:21:51.000000 creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_dac_list_selective.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-08 23:21:51.000000 creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_dac_value_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-08 23:21:51.000000 creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_single_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-08 23:21:51.000000 creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_single_value_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-08 23:21:51.000000 creativecontrol-circuitpython-ltc166x-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-08 23:21:42.000000 creativecontrol-circuitpython-ltc166x-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 23:21:59.670340 creativecontrol-circuitpython-ltc166x-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:30:07.432784 creativecontrol-circuitpython-ltc166x-1.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:30:07.428784 creativecontrol-circuitpython-ltc166x-1.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:30:07.428784 creativecontrol-circuitpython-ltc166x-1.2.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:30:07.428784 creativecontrol-circuitpython-ltc166x-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:30:07.432784 creativecontrol-circuitpython-ltc166x-1.2.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-09 18:30:07.432784 creativecontrol-circuitpython-ltc166x-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:30:07.432784 creativecontrol-circuitpython-ltc166x-1.2.3/creativecontrol_circuitpython_ltc166x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-09 18:30:07.000000 creativecontrol-circuitpython-ltc166x-1.2.3/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-09 18:30:07.000000 creativecontrol-circuitpython-ltc166x-1.2.3/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:30:07.000000 creativecontrol-circuitpython-ltc166x-1.2.3/creativecontrol_circuitpython_ltc166x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-09 18:30:07.000000 creativecontrol-circuitpython-ltc166x-1.2.3/creativecontrol_circuitpython_ltc166x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:30:07.000000 creativecontrol-circuitpython-ltc166x-1.2.3/creativecontrol_circuitpython_ltc166x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-09 18:29:58.000000 creativecontrol-circuitpython-ltc166x-1.2.3/creativecontrol_circuitpython_ltc166x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:30:07.432784 creativecontrol-circuitpython-ltc166x-1.2.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:30:07.432784 creativecontrol-circuitpython-ltc166x-1.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:30:07.432784 creativecontrol-circuitpython-ltc166x-1.2.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-09 18:29:58.000000 creativecontrol-circuitpython-ltc166x-1.2.3/examples/ltc166x_dac_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-09 18:29:58.000000 creativecontrol-circuitpython-ltc166x-1.2.3/examples/ltc166x_dac_list_selective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-09 18:29:58.000000 creativecontrol-circuitpython-ltc166x-1.2.3/examples/ltc166x_dac_value_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-09 18:29:58.000000 creativecontrol-circuitpython-ltc166x-1.2.3/examples/ltc166x_single_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-09 18:29:58.000000 creativecontrol-circuitpython-ltc166x-1.2.3/examples/ltc166x_single_value_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-09 18:29:58.000000 creativecontrol-circuitpython-ltc166x-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-09 18:29:47.000000 creativecontrol-circuitpython-ltc166x-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:30:07.432784 creativecontrol-circuitpython-ltc166x-1.2.3/setup.cfg
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `creativecontrol-circuitpython-ltc166x-1.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/.github/workflows/release_gh.yml` & `creativecontrol-circuitpython-ltc166x-1.2.3/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/.github/workflows/release_pypi.yml` & `creativecontrol-circuitpython-ltc166x-1.2.3/.github/workflows/release_pypi.yml`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/.gitignore` & `creativecontrol-circuitpython-ltc166x-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/.pre-commit-config.yaml` & `creativecontrol-circuitpython-ltc166x-1.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/.pylintrc` & `creativecontrol-circuitpython-ltc166x-1.2.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/CODE_OF_CONDUCT.md` & `creativecontrol-circuitpython-ltc166x-1.2.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/LICENSE` & `creativecontrol-circuitpython-ltc166x-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/LICENSES/CC-BY-4.0.txt` & `creativecontrol-circuitpython-ltc166x-1.2.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/LICENSES/MIT.txt` & `creativecontrol-circuitpython-ltc166x-1.2.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/LICENSES/Unlicense.txt` & `creativecontrol-circuitpython-ltc166x-1.2.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/PKG-INFO` & `creativecontrol-circuitpython-ltc166x-1.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creativecontrol-circuitpython-ltc166x
-Version: 1.2.2
+Version: 1.2.3
 Summary: CircuitPython library for control of LTC166X 8-bit and 10-bit DACs.
 Author-email: creativecontrol <t@creativecontrol.cc>
 License: MIT
 Project-URL: Homepage, https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X
 Keywords: adafruit,blinka,circuitpython,micropython,creativecontrol_circuitpython_ltc166x,LTC1660,LTC1665,DAC
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -130,16 +130,23 @@
         print('off')
         ltc1665.write_dac_values([0]*8)
         time.sleep(4)
 
 Documentation
 =============
 
+API documentation for this library can be found on `Read the Docs <https://creativecontrol-circuitpython-ltc166x.readthedocs.io/>`_.
+
 For information on building library documentation, please check out
 `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
 
+Tutorial
+=============
+
+A tutorial on controlling daisy-chained LTC166X DACs can be found on my website `creativecontrol <https://www.creativecontrol.cc/blog/2023/7/7/circuitpython-ltc166x-dac-control-of-daisy-chained-dacs>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/creativecontrol/CircuitPython_creativecontrol_CircuitPython_LTC166X/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/README.rst` & `creativecontrol-circuitpython-ltc166x-1.2.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -112,16 +112,23 @@
         print('off')
         ltc1665.write_dac_values([0]*8)
         time.sleep(4)
 
 Documentation
 =============
 
+API documentation for this library can be found on `Read the Docs <https://creativecontrol-circuitpython-ltc166x.readthedocs.io/>`_.
+
 For information on building library documentation, please check out
 `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
 
+Tutorial
+=============
+
+A tutorial on controlling daisy-chained LTC166X DACs can be found on my website `creativecontrol <https://www.creativecontrol.cc/blog/2023/7/7/circuitpython-ltc166x-dac-control-of-daisy-chained-dacs>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/creativecontrol/CircuitPython_creativecontrol_CircuitPython_LTC166X/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO` & `creativecontrol-circuitpython-ltc166x-1.2.3/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creativecontrol-circuitpython-ltc166x
-Version: 1.2.2
+Version: 1.2.3
 Summary: CircuitPython library for control of LTC166X 8-bit and 10-bit DACs.
 Author-email: creativecontrol <t@creativecontrol.cc>
 License: MIT
 Project-URL: Homepage, https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X
 Keywords: adafruit,blinka,circuitpython,micropython,creativecontrol_circuitpython_ltc166x,LTC1660,LTC1665,DAC
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -130,16 +130,23 @@
         print('off')
         ltc1665.write_dac_values([0]*8)
         time.sleep(4)
 
 Documentation
 =============
 
+API documentation for this library can be found on `Read the Docs <https://creativecontrol-circuitpython-ltc166x.readthedocs.io/>`_.
+
 For information on building library documentation, please check out
 `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
 
+Tutorial
+=============
+
+A tutorial on controlling daisy-chained LTC166X DACs can be found on my website `creativecontrol <https://www.creativecontrol.cc/blog/2023/7/7/circuitpython-ltc166x-dac-control-of-daisy-chained-dacs>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/creativecontrol/CircuitPython_creativecontrol_CircuitPython_LTC166X/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt` & `creativecontrol-circuitpython-ltc166x-1.2.3/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/creativecontrol_circuitpython_ltc166x.py` & `creativecontrol-circuitpython-ltc166x-1.2.3/creativecontrol_circuitpython_ltc166x.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 """
 
 import microcontroller
 from busio import SPI
 import digitalio
 from adafruit_bus_device.spi_device import SPIDevice
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 __repo__ = (
     "https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X.git"
 )
 
 
 class LTC166X:
     """
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/docs/_static/favicon.ico` & `creativecontrol-circuitpython-ltc166x-1.2.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/docs/conf.py` & `creativecontrol-circuitpython-ltc166x-1.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/docs/examples.rst` & `creativecontrol-circuitpython-ltc166x-1.2.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/docs/index.rst` & `creativecontrol-circuitpython-ltc166x-1.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_dac_chain.py` & `creativecontrol-circuitpython-ltc166x-1.2.3/examples/ltc166x_dac_chain.py`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_dac_list_selective.py` & `creativecontrol-circuitpython-ltc166x-1.2.3/examples/ltc166x_dac_list_selective.py`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_dac_value_list.py` & `creativecontrol-circuitpython-ltc166x-1.2.3/examples/ltc166x_dac_value_list.py`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_single_value.py` & `creativecontrol-circuitpython-ltc166x-1.2.3/examples/ltc166x_single_value.py`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/examples/ltc166x_single_value_sweep.py` & `creativecontrol-circuitpython-ltc166x-1.2.3/examples/ltc166x_single_value_sweep.py`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.2.2/pyproject.toml` & `creativecontrol-circuitpython-ltc166x-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "creativecontrol-circuitpython-ltc166x"
 description = "CircuitPython library for control of LTC166X 8-bit and 10-bit DACs."
-version = "1.2.2"
+version = "1.2.3"
 readme = "README.rst"
 authors = [
     {name = "creativecontrol", email = "t@creativecontrol.cc"}
 ]
 urls = {Homepage = "https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X"}
 keywords = [
     "adafruit",
```

