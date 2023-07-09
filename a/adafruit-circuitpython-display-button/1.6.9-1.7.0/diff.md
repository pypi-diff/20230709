# Comparing `tmp/adafruit-circuitpython-display_button-1.6.9.tar.gz` & `tmp/adafruit-circuitpython-display_button-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-display_button-1.6.9.tar", last modified: Fri May 26 15:54:18 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-display_button-1.7.0.tar", last modified: Sun Jul  9 14:20:48 2023, max compression
```

## Comparing `adafruit-circuitpython-display_button-1.6.9.tar` & `adafruit-circuitpython-display_button-1.7.0.tar`

### file list

```diff
@@ -1,50 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:18.763318 adafruit-circuitpython-display_button-1.6.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:18.747318 adafruit-circuitpython-display_button-1.6.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:18.751318 adafruit-circuitpython-display_button-1.6.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:18.755318 adafruit-circuitpython-display_button-1.6.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:18.755318 adafruit-circuitpython-display_button-1.6.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-26 15:54:18.763318 adafruit-circuitpython-display_button-1.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-05-26 15:54:10.000000 adafruit-circuitpython-display_button-1.6.9/adafruit_button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:18.755318 adafruit-circuitpython-display_button-1.6.9/adafruit_circuitpython_display_button.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-26 15:54:18.000000 adafruit-circuitpython-display_button-1.6.9/adafruit_circuitpython_display_button.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-26 15:54:18.000000 adafruit-circuitpython-display_button-1.6.9/adafruit_circuitpython_display_button.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:54:18.000000 adafruit-circuitpython-display_button-1.6.9/adafruit_circuitpython_display_button.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-26 15:54:18.000000 adafruit-circuitpython-display_button-1.6.9/adafruit_circuitpython_display_button.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 15:54:18.000000 adafruit-circuitpython-display_button-1.6.9/adafruit_circuitpython_display_button.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:18.759318 adafruit-circuitpython-display_button-1.6.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:18.759318 adafruit-circuitpython-display_button-1.6.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:18.763318 adafruit-circuitpython-display_button-1.6.9/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-26 15:54:10.000000 adafruit-circuitpython-display_button-1.6.9/examples/display_button_color_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-26 15:54:10.000000 adafruit-circuitpython-display_button-1.6.9/examples/display_button_customfont.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-26 15:54:10.000000 adafruit-circuitpython-display_button-1.6.9/examples/display_button_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-26 15:54:10.000000 adafruit-circuitpython-display_button-1.6.9/examples/display_button_soundboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-26 15:54:10.000000 adafruit-circuitpython-display_button-1.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-26 15:53:59.000000 adafruit-circuitpython-display_button-1.6.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:54:18.763318 adafruit-circuitpython-display_button-1.6.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:20:48.916102 adafruit-circuitpython-display_button-1.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:20:48.912102 adafruit-circuitpython-display_button-1.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:20:48.912102 adafruit-circuitpython-display_button-1.7.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:20:48.912102 adafruit-circuitpython-display_button-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:20:48.912102 adafruit-circuitpython-display_button-1.7.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-09 14:20:48.916102 adafruit-circuitpython-display_button-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:20:48.912102 adafruit-circuitpython-display_button-1.7.0/adafruit_button/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-09 14:20:41.000000 adafruit-circuitpython-display_button-1.7.0/adafruit_button/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-07-09 14:20:41.000000 adafruit-circuitpython-display_button-1.7.0/adafruit_button/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-09 14:20:41.000000 adafruit-circuitpython-display_button-1.7.0/adafruit_button/button_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-09 14:20:41.000000 adafruit-circuitpython-display_button-1.7.0/adafruit_button/sprite_button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:20:48.916102 adafruit-circuitpython-display_button-1.7.0/adafruit_circuitpython_display_button.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-09 14:20:48.000000 adafruit-circuitpython-display_button-1.7.0/adafruit_circuitpython_display_button.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-09 14:20:48.000000 adafruit-circuitpython-display_button-1.7.0/adafruit_circuitpython_display_button.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:20:48.000000 adafruit-circuitpython-display_button-1.7.0/adafruit_circuitpython_display_button.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-09 14:20:48.000000 adafruit-circuitpython-display_button-1.7.0/adafruit_circuitpython_display_button.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-09 14:20:48.000000 adafruit-circuitpython-display_button-1.7.0/adafruit_circuitpython_display_button.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:20:48.916102 adafruit-circuitpython-display_button-1.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:20:48.916102 adafruit-circuitpython-display_button-1.7.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:20:48.916102 adafruit-circuitpython-display_button-1.7.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:20:48.916102 adafruit-circuitpython-display_button-1.7.0/examples/bmps/
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/examples/bmps/gradient_button_0.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/examples/bmps/gradient_button_0.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/examples/bmps/gradient_button_1.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/examples/bmps/gradient_button_1.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-09 14:20:41.000000 adafruit-circuitpython-display_button-1.7.0/examples/display_button_color_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-09 14:20:41.000000 adafruit-circuitpython-display_button-1.7.0/examples/display_button_customfont.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-09 14:20:41.000000 adafruit-circuitpython-display_button-1.7.0/examples/display_button_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-09 14:20:41.000000 adafruit-circuitpython-display_button-1.7.0/examples/display_button_soundboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-09 14:20:41.000000 adafruit-circuitpython-display_button-1.7.0/examples/display_button_spritebutton_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-09 14:20:41.000000 adafruit-circuitpython-display_button-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-09 14:20:32.000000 adafruit-circuitpython-display_button-1.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:20:48.916102 adafruit-circuitpython-display_button-1.7.0/setup.cfg
```

### Comparing `adafruit-circuitpython-display_button-1.6.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-display_button-1.7.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/.gitignore` & `adafruit-circuitpython-display_button-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/.pre-commit-config.yaml` & `adafruit-circuitpython-display_button-1.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/.pylintrc` & `adafruit-circuitpython-display_button-1.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-display_button-1.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/LICENSE` & `adafruit-circuitpython-display_button-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-display_button-1.7.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/LICENSES/MIT.txt` & `adafruit-circuitpython-display_button-1.7.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-display_button-1.7.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/PKG-INFO` & `adafruit-circuitpython-display_button-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-display_button
-Version: 1.6.9
+Version: 1.7.0
 Summary: UI Buttons for displayio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Display_Button
 Keywords: adafruit,blinka,circuitpython,micropython,display_button,buttons,UI
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-display_button-1.6.9/README.rst` & `adafruit-circuitpython-display_button-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/adafruit_button.py` & `adafruit-circuitpython-display_button-1.7.0/adafruit_button/button.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2019 Limor Fried for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 """
-`adafruit_button`
+`adafruit_button.button`
 ================================================================================
 
 UI Buttons for displayio
 
 
 * Author(s): Limor Fried
 
@@ -18,32 +18,23 @@
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 from micropython import const
-import displayio
-from adafruit_display_text.label import Label
 from adafruit_display_shapes.rect import Rect
 from adafruit_display_shapes.roundrect import RoundRect
+from adafruit_button.button_base import ButtonBase, _check_color
 
-__version__ = "1.6.9"
+__version__ = "1.7.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Button.git"
 
 
-def _check_color(color):
-    # if a tuple is supplied, convert it to a RGB number
-    if isinstance(color, tuple):
-        r, g, b = color
-        return int((r << 16) + (g << 8) + (b & 0xFF))
-    return color
-
-
-class Button(displayio.Group):
+class Button(ButtonBase):
     # pylint: disable=too-many-instance-attributes, too-many-locals
     """Helper class for creating UI buttons for ``displayio``.
 
     :param x: The x position of the button.
     :param y: The y position of the button.
     :param width: The width of the button in pixels.
     :param height: The height of the button in pixels.
@@ -137,104 +128,58 @@
         label=None,
         label_font=None,
         label_color=0x0,
         selected_fill=None,
         selected_outline=None,
         selected_label=None
     ):
-        super().__init__(x=x, y=y)
-        self.x = x
-        self.y = y
-        self._width = width
-        self._height = height
-        self._font = label_font
-        self._selected = False
-        self.name = name
-        self._label = label
+        super().__init__(
+            x=x,
+            y=y,
+            width=width,
+            height=height,
+            name=name,
+            label=label,
+            label_font=label_font,
+            label_color=label_color,
+            selected_label=selected_label,
+        )
+
         self.body = self.fill = self.shadow = None
         self.style = style
 
         self._fill_color = _check_color(fill_color)
         self._outline_color = _check_color(outline_color)
-        self._label_color = label_color
-        self._label_font = label_font
+
         # Selecting inverts the button colors!
         self._selected_fill = _check_color(selected_fill)
         self._selected_outline = _check_color(selected_outline)
-        self._selected_label = _check_color(selected_label)
 
         if self.selected_fill is None and fill_color is not None:
             self.selected_fill = (~self._fill_color) & 0xFFFFFF
         if self.selected_outline is None and outline_color is not None:
             self.selected_outline = (~self._outline_color) & 0xFFFFFF
 
         self._create_body()
         if self.body:
             self.append(self.body)
 
         self.label = label
 
-    @property
-    def label(self):
-        """The text label of the button"""
-        return self._label.text
-
-    @label.setter
-    def label(self, newtext):
-        if self._label and self and (self[-1] == self._label):
-            self.pop()
-
-        self._label = None
-        if not newtext or (self._label_color is None):  # no new text
-            return  # nothing to do!
-
-        if not self._label_font:
-            raise RuntimeError("Please provide label font")
-        self._label = Label(self._label_font, text=newtext)
-        dims = self._label.bounding_box
-        if dims[2] >= self.width or dims[3] >= self.height:
-            while len(self._label.text) > 1 and (
-                dims[2] >= self.width or dims[3] >= self.height
-            ):
-                self._label.text = "{}.".format(self._label.text[:-2])
-                dims = self._label.bounding_box
-            if len(self._label.text) <= 1:
-                raise RuntimeError("Button not large enough for label")
-        self._label.x = (self.width - dims[2]) // 2
-        self._label.y = self.height // 2
-        self._label.color = self._label_color
-        self.append(self._label)
-
-        if (self.selected_label is None) and (self._label_color is not None):
-            self.selected_label = (~self._label_color) & 0xFFFFFF
-
-    @property
-    def selected(self):
-        """Selected inverts the colors."""
-        return self._selected
-
-    @selected.setter
-    def selected(self, value):
-        if value == self._selected:
-            return  # bail now, nothing more to do
-        self._selected = value
+    def _subclass_selected_behavior(self, value):
         if self._selected:
             new_fill = self.selected_fill
             new_out = self.selected_outline
-            new_label = self.selected_label
         else:
             new_fill = self._fill_color
             new_out = self._outline_color
-            new_label = self._label_color
         # update all relevant colors!
         if self.body is not None:
             self.body.fill = new_fill
             self.body.outline = new_out
-        if self._label is not None:
-            self._label.color = new_label
 
     @property
     def group(self):
         """Return self for compatibility with old API."""
         print(
             "Warning: The group property is being deprecated. "
             "User code should be updated to add the Button directly to the "
@@ -292,33 +237,14 @@
     @selected_outline.setter
     def selected_outline(self, new_color):
         self._selected_outline = _check_color(new_color)
         if self.selected:
             self.body.outline = self._selected_outline
 
     @property
-    def selected_label(self):
-        """The font color of the button when selected"""
-        return self._selected_label
-
-    @selected_label.setter
-    def selected_label(self, new_color):
-        self._selected_label = _check_color(new_color)
-
-    @property
-    def label_color(self):
-        """The font color of the button"""
-        return self._label_color
-
-    @label_color.setter
-    def label_color(self, new_color):
-        self._label_color = _check_color(new_color)
-        self._label.color = self._label_color
-
-    @property
     def width(self):
         """The width of the button"""
         return self._width
 
     @width.setter
     def width(self, new_width):
         self._width = new_width
```

### Comparing `adafruit-circuitpython-display_button-1.6.9/adafruit_circuitpython_display_button.egg-info/PKG-INFO` & `adafruit-circuitpython-display_button-1.7.0/adafruit_circuitpython_display_button.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-display-button
-Version: 1.6.9
+Version: 1.7.0
 Summary: UI Buttons for displayio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Display_Button
 Keywords: adafruit,blinka,circuitpython,micropython,display_button,buttons,UI
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-display_button-1.6.9/adafruit_circuitpython_display_button.egg-info/SOURCES.txt` & `adafruit-circuitpython-display_button-1.7.0/adafruit_circuitpython_display_button.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,26 +2,29 @@
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
-adafruit_button.py
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
 .github/workflows/release_gh.yml
 .github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
+adafruit_button/__init__.py
+adafruit_button/button.py
+adafruit_button/button_base.py
+adafruit_button/sprite_button.py
 adafruit_circuitpython_display_button.egg-info/PKG-INFO
 adafruit_circuitpython_display_button.egg-info/SOURCES.txt
 adafruit_circuitpython_display_button.egg-info/dependency_links.txt
 adafruit_circuitpython_display_button.egg-info/requires.txt
 adafruit_circuitpython_display_button.egg-info/top_level.txt
 docs/api.rst
 docs/api.rst.license
@@ -32,8 +35,13 @@
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/display_button_color_properties.py
 examples/display_button_customfont.py
 examples/display_button_simpletest.py
-examples/display_button_soundboard.py
+examples/display_button_soundboard.py
+examples/display_button_spritebutton_simpletest.py
+examples/bmps/gradient_button_0.bmp
+examples/bmps/gradient_button_0.bmp.license
+examples/bmps/gradient_button_1.bmp
+examples/bmps/gradient_button_1.bmp.license
```

### Comparing `adafruit-circuitpython-display_button-1.6.9/docs/_static/favicon.ico` & `adafruit-circuitpython-display_button-1.7.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/docs/conf.py` & `adafruit-circuitpython-display_button-1.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/docs/examples.rst` & `adafruit-circuitpython-display_button-1.7.0/docs/examples.rst`

 * *Files 13% similar despite different names*

```diff
@@ -29,7 +29,16 @@
 ----------
 
 A soundboard made with buttons
 
 .. literalinclude:: ../examples/display_button_soundboard.py
     :caption: examples/display_button_soundboard.py
     :linenos:
+
+Sprite Button
+-------------
+
+Custom sprite button
+
+.. literalinclude:: ../examples/display_button_spritebutton_simpletest.py
+    :caption: examples/display_button_spritebutton_simpletest.py
+    :linenos:
```

### Comparing `adafruit-circuitpython-display_button-1.6.9/docs/index.rst` & `adafruit-circuitpython-display_button-1.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/examples/display_button_color_properties.py` & `adafruit-circuitpython-display_button-1.7.0/examples/display_button_color_properties.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/examples/display_button_customfont.py` & `adafruit-circuitpython-display_button-1.7.0/examples/display_button_customfont.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/examples/display_button_simpletest.py` & `adafruit-circuitpython-display_button-1.7.0/examples/display_button_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/examples/display_button_soundboard.py` & `adafruit-circuitpython-display_button-1.7.0/examples/display_button_soundboard.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_button-1.6.9/pyproject.toml` & `adafruit-circuitpython-display_button-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-display_button"
 description = "UI Buttons for displayio"
-version = "1.6.9"
+version = "1.7.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Button"}
 keywords = [
     "adafruit",
@@ -35,12 +35,12 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["adafruit_button"]
+packages = ["adafruit_button"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 optional-dependencies = {optional = {file = ["optional_requirements.txt"]}}
```

