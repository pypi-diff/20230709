# Comparing `tmp/PyThea-0.7.3.tar.gz` & `tmp/PyThea-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyThea-0.7.3.tar", last modified: Thu Feb 16 04:21:15 2023, max compression
+gzip compressed data, was "PyThea-0.7.4.tar", last modified: Sun Jul  9 12:19:32 2023, max compression
```

## Comparing `PyThea-0.7.3.tar` & `PyThea-0.7.4.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-02-16 04:21:15.514035 PyThea-0.7.3/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)    33872 2023-01-03 18:26:41.000000 PyThea-0.7.3/LICENSE.md
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      381 2023-01-03 18:26:41.000000 PyThea-0.7.3/MANIFEST.in
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     6743 2023-02-16 04:21:15.514294 PyThea-0.7.3/PKG-INFO
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-02-16 04:21:15.500527 PyThea-0.7.3/PyThea/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)    21358 2023-01-25 22:38:03.000000 PyThea-0.7.3/PyThea/PyThea_app.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)       44 2023-01-25 19:20:20.000000 PyThea-0.7.3/PyThea/__init__.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      160 2023-02-16 04:21:15.000000 PyThea-0.7.3/PyThea/_version.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     2856 2023-01-25 22:38:03.000000 PyThea-0.7.3/PyThea/callbacks.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-02-16 04:21:15.504451 PyThea-0.7.3/PyThea/config/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      132 2023-01-25 22:38:03.000000 PyThea-0.7.3/PyThea/config/__init__.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     3211 2023-01-03 18:26:41.000000 PyThea-0.7.3/PyThea/config/app_styles.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     4975 2023-01-03 18:26:41.000000 PyThea-0.7.3/PyThea/config/config_sliders.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      521 2023-01-03 18:26:41.000000 PyThea-0.7.3/PyThea/config/selected_bodies.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     2918 2023-01-25 22:37:49.000000 PyThea-0.7.3/PyThea/config/selected_imagers.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-02-16 04:21:15.505257 PyThea-0.7.3/PyThea/extensions/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     1075 2023-01-25 22:38:03.000000 PyThea-0.7.3/PyThea/extensions/LICENSE_gcs_python.md
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.7.3/PyThea/extensions/__init__.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     2996 2023-01-03 18:26:41.000000 PyThea-0.7.3/PyThea/extensions/buttons.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)    30647 2023-01-25 22:38:03.000000 PyThea-0.7.3/PyThea/geometrical_models.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)    11332 2023-01-25 22:38:03.000000 PyThea-0.7.3/PyThea/modules.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     2360 2023-01-25 22:38:03.000000 PyThea-0.7.3/PyThea/pythea_cli.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-02-16 04:21:15.505527 PyThea-0.7.3/PyThea/sunpy_dev/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-19 20:37:41.000000 PyThea-0.7.3/PyThea/sunpy_dev/__init__.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-02-16 04:21:15.505756 PyThea-0.7.3/PyThea/sunpy_dev/extern/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.7.3/PyThea/sunpy_dev/extern/__init__.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-02-16 04:21:15.505991 PyThea-0.7.3/PyThea/sunpy_dev/extern/sunkit_instruments/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.7.3/PyThea/sunpy_dev/extern/sunkit_instruments/__init__.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-02-16 04:21:15.506499 PyThea-0.7.3/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.7.3/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/__init__.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     3161 2023-01-25 22:38:03.000000 PyThea-0.7.3/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/utils.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-02-16 04:21:15.507075 PyThea-0.7.3/PyThea/sunpy_dev/map/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.7.3/PyThea/sunpy_dev/map/__init__.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     8347 2023-01-25 22:38:03.000000 PyThea-0.7.3/PyThea/sunpy_dev/map/maputils.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-02-16 04:21:15.510612 PyThea-0.7.3/PyThea/test/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      239 2023-01-03 18:26:41.000000 PyThea-0.7.3/PyThea/test/Pythea_test.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.7.3/PyThea/test/__init__.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      439 2023-01-03 18:26:41.000000 PyThea-0.7.3/PyThea/test/conftest.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     4530 2023-01-03 18:26:41.000000 PyThea-0.7.3/PyThea/test/test_geometrical_models.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      554 2023-01-03 18:26:41.000000 PyThea-0.7.3/PyThea/test/test_imports.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      583 2023-01-25 22:30:34.000000 PyThea-0.7.3/PyThea/test/test_remote_clients.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      400 2023-01-25 22:30:34.000000 PyThea-0.7.3/PyThea/test/test_utils.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)    16303 2023-02-16 03:40:58.000000 PyThea-0.7.3/PyThea/utils.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     1000 2023-01-25 22:38:03.000000 PyThea-0.7.3/PyThea/version.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-02-16 04:21:15.502828 PyThea-0.7.3/PyThea.egg-info/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     6743 2023-02-16 04:21:15.000000 PyThea-0.7.3/PyThea.egg-info/PKG-INFO
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     1268 2023-02-16 04:21:15.000000 PyThea-0.7.3/PyThea.egg-info/SOURCES.txt
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        1 2023-02-16 04:21:15.000000 PyThea-0.7.3/PyThea.egg-info/dependency_links.txt
--rw-r--r--   0 kouloa1  (44305931) staff       (20)       50 2023-02-16 04:21:15.000000 PyThea-0.7.3/PyThea.egg-info/entry_points.txt
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        1 2023-01-19 20:30:28.000000 PyThea-0.7.3/PyThea.egg-info/not-zip-safe
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      169 2023-02-16 04:21:15.000000 PyThea-0.7.3/PyThea.egg-info/requires.txt
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        7 2023-02-16 04:21:15.000000 PyThea-0.7.3/PyThea.egg-info/top_level.txt
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     6039 2023-01-25 22:38:03.000000 PyThea-0.7.3/README.md
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     5832 2023-01-25 22:38:03.000000 PyThea-0.7.3/README_pypi.md
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      564 2023-01-25 22:38:03.000000 PyThea-0.7.3/environment.yml
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      107 2023-01-03 18:26:41.000000 PyThea-0.7.3/pyproject.toml
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      169 2023-01-25 22:38:03.000000 PyThea-0.7.3/requirements.txt
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     1018 2023-02-16 04:21:15.515145 PyThea-0.7.3/setup.cfg
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     1837 2023-01-25 22:38:03.000000 PyThea-0.7.3/setup.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-07-09 12:19:32.303557 PyThea-0.7.4/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)    33872 2023-01-03 18:26:41.000000 PyThea-0.7.4/LICENSE.md
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      381 2023-01-03 18:26:41.000000 PyThea-0.7.4/MANIFEST.in
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     6743 2023-07-09 12:19:32.303737 PyThea-0.7.4/PKG-INFO
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-07-09 12:19:32.293683 PyThea-0.7.4/PyThea/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)    21362 2023-07-09 12:04:38.000000 PyThea-0.7.4/PyThea/PyThea_app.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)       44 2023-01-25 19:20:20.000000 PyThea-0.7.4/PyThea/__init__.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      160 2023-07-09 12:19:32.000000 PyThea-0.7.4/PyThea/_version.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     2856 2023-01-25 22:38:03.000000 PyThea-0.7.4/PyThea/callbacks.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-07-09 12:19:32.297479 PyThea-0.7.4/PyThea/config/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      132 2023-01-25 22:38:03.000000 PyThea-0.7.4/PyThea/config/__init__.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     2834 2023-05-31 01:37:57.000000 PyThea-0.7.4/PyThea/config/app_styles.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     4975 2023-01-03 18:26:41.000000 PyThea-0.7.4/PyThea/config/config_sliders.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      521 2023-01-03 18:26:41.000000 PyThea-0.7.4/PyThea/config/selected_bodies.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     2918 2023-05-17 16:42:24.000000 PyThea-0.7.4/PyThea/config/selected_imagers.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-07-09 12:19:32.298343 PyThea-0.7.4/PyThea/extensions/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     1075 2023-01-25 22:38:03.000000 PyThea-0.7.4/PyThea/extensions/LICENSE_gcs_python.md
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.7.4/PyThea/extensions/__init__.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     2996 2023-01-03 18:26:41.000000 PyThea-0.7.4/PyThea/extensions/buttons.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)    30760 2023-07-09 12:04:57.000000 PyThea-0.7.4/PyThea/geometrical_models.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)    11332 2023-05-29 14:53:41.000000 PyThea-0.7.4/PyThea/modules.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     2360 2023-03-28 19:03:30.000000 PyThea-0.7.4/PyThea/pythea_cli.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-07-09 12:19:32.298796 PyThea-0.7.4/PyThea/sunpy_dev/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-19 20:37:41.000000 PyThea-0.7.4/PyThea/sunpy_dev/__init__.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-07-09 12:19:32.299042 PyThea-0.7.4/PyThea/sunpy_dev/extern/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.7.4/PyThea/sunpy_dev/extern/__init__.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-07-09 12:19:32.299283 PyThea-0.7.4/PyThea/sunpy_dev/extern/sunkit_instruments/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.7.4/PyThea/sunpy_dev/extern/sunkit_instruments/__init__.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-07-09 12:19:32.299899 PyThea-0.7.4/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.7.4/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/__init__.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     3161 2023-03-28 20:20:53.000000 PyThea-0.7.4/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/utils.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-07-09 12:19:32.300483 PyThea-0.7.4/PyThea/sunpy_dev/map/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-03-28 18:07:04.000000 PyThea-0.7.4/PyThea/sunpy_dev/map/__init__.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     7825 2023-05-17 16:42:24.000000 PyThea-0.7.4/PyThea/sunpy_dev/map/maputils.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-07-09 12:19:32.303172 PyThea-0.7.4/PyThea/test/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      239 2023-01-03 18:26:41.000000 PyThea-0.7.4/PyThea/test/Pythea_test.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.7.4/PyThea/test/__init__.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      439 2023-01-03 18:26:41.000000 PyThea-0.7.4/PyThea/test/conftest.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     4530 2023-01-03 18:26:41.000000 PyThea-0.7.4/PyThea/test/test_geometrical_models.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      554 2023-01-03 18:26:41.000000 PyThea-0.7.4/PyThea/test/test_imports.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      583 2023-03-28 19:03:30.000000 PyThea-0.7.4/PyThea/test/test_remote_clients.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      400 2023-03-28 19:03:30.000000 PyThea-0.7.4/PyThea/test/test_utils.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)    16317 2023-07-09 12:04:38.000000 PyThea-0.7.4/PyThea/utils.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     1000 2023-01-25 22:38:03.000000 PyThea-0.7.4/PyThea/version.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2023-07-09 12:19:32.296191 PyThea-0.7.4/PyThea.egg-info/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     6148 2023-05-15 13:18:05.000000 PyThea-0.7.4/PyThea.egg-info/.DS_Store
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     6743 2023-07-09 12:19:32.000000 PyThea-0.7.4/PyThea.egg-info/PKG-INFO
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     1294 2023-07-09 12:19:32.000000 PyThea-0.7.4/PyThea.egg-info/SOURCES.txt
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        1 2023-07-09 12:19:32.000000 PyThea-0.7.4/PyThea.egg-info/dependency_links.txt
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)       50 2023-07-09 12:19:32.000000 PyThea-0.7.4/PyThea.egg-info/entry_points.txt
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        1 2023-01-19 20:30:28.000000 PyThea-0.7.4/PyThea.egg-info/not-zip-safe
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      172 2023-07-09 12:19:32.000000 PyThea-0.7.4/PyThea.egg-info/requires.txt
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        7 2023-07-09 12:19:32.000000 PyThea-0.7.4/PyThea.egg-info/top_level.txt
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     6039 2023-01-25 22:38:03.000000 PyThea-0.7.4/README.md
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     5832 2023-01-25 22:38:03.000000 PyThea-0.7.4/README_pypi.md
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      567 2023-07-09 12:11:40.000000 PyThea-0.7.4/environment.yml
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      107 2023-01-03 18:26:41.000000 PyThea-0.7.4/pyproject.toml
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      172 2023-07-09 12:11:40.000000 PyThea-0.7.4/requirements.txt
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     1018 2023-07-09 12:19:32.304406 PyThea-0.7.4/setup.cfg
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     1837 2023-05-29 14:53:41.000000 PyThea-0.7.4/setup.py
```

### Comparing `PyThea-0.7.3/LICENSE.md` & `PyThea-0.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/PKG-INFO` & `PyThea-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyThea
-Version: 0.7.3
+Version: 0.7.4
 Summary: PyThea: A software package to reconstruct the 3D structure of CMEs and shock waves
 Home-page: https://github.com/AthKouloumvakos/PyThea
 Author: Athanasios Kouloumvakos
 Author-email: athkouloumvakos@gmail.com
 License: GPL-3.0
 Keywords: science,solar physics,solar,sun,shock waves
 Platform: any
```

### Comparing `PyThea-0.7.3/PyThea/PyThea_app.py` & `PyThea-0.7.4/PyThea/PyThea_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,18 +277,18 @@
         model = gcs(center, height, alpha, kappa, tilt)
 
     #############################################################
     # Plot main and supplement figure images
     fig, axis = make_figure(running_map, image_mode, clim=clim, clip_model=clip_model)
     if st.session_state.plot_mesh_mode == 'Skeleton':
         model.plot(axis, mode='Skeleton')
-    if st.session_state.plot_mesh_mode == 'Full':
+    elif st.session_state.plot_mesh_mode == 'Full':
         model.plot(axis, mode='Skeleton')
         model.plot(axis, mode='Full')
-    if st.session_state.plot_mesh_mode == 'Surface':
+    elif st.session_state.plot_mesh_mode == 'Surface':
         model.plot(axis, only_surface=True)
 
     if star_field:
         plot_bodies(axis, bodies_list, running_map)
         axis.legend()
     st.pyplot(fig)
```

### Comparing `PyThea-0.7.3/PyThea/callbacks.py` & `PyThea-0.7.4/PyThea/callbacks.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/PyThea/config/app_styles.py` & `PyThea-0.7.4/PyThea/config/app_styles.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 def apply(st):
     # Hide the menu button
     st.markdown(""" <style>
                 #MainMenu {visibility: hidden;}
                 footer {visibility: hidden;}
                 </style> """, unsafe_allow_html=True)
     # Do some css styling tricks here (e.g. remove the padding)
-    # https://medium.com/ssense-tech/streamlit-tips-tricks-and-hacks-for-data-scientists-d928414e0c16
-    padding = 1
-    st.markdown(f""" <style>
-                .css-12oz5g7{{
-                padding-top: {padding}rem;
-                margin-top: -3.5rem;
-                max-width: 50rem;
-                padding-right: {padding}rem;
-                padding-left: {padding}rem;
-                padding-bottom: {padding}rem;
-                }} </style> """, unsafe_allow_html=True)
-    st.markdown(f""" <style>
-                .css-128j0gw{{
-                margin-top: -3.0rem;
-                }} </style> """, unsafe_allow_html=True)
+    # https://discuss.streamlit.io/t/reduce-white-space-top-of-the-page/21737/3
+    st.markdown("""
+        <style>
+               .block-container {
+                    padding-top: 0rem;
+                }
+        </style>
+        """, unsafe_allow_html=True)
     # Reduce the space in horizontal component
     st.markdown(f""" <style>
                 hr {{
                 margin: 10px 0px;
                 }} </style> """, unsafe_allow_html=True)
     # Custom button appearance
     st.markdown('''
```

### Comparing `PyThea-0.7.3/PyThea/config/config_sliders.py` & `PyThea-0.7.4/PyThea/config/config_sliders.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/PyThea/config/selected_bodies.py` & `PyThea-0.7.4/PyThea/config/selected_bodies.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/PyThea/config/selected_imagers.py` & `PyThea-0.7.4/PyThea/config/selected_imagers.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/PyThea/extensions/LICENSE_gcs_python.md` & `PyThea-0.7.4/PyThea/extensions/LICENSE_gcs_python.md`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/PyThea/extensions/buttons.py` & `PyThea-0.7.4/PyThea/extensions/buttons.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/PyThea/geometrical_models.py` & `PyThea-0.7.4/PyThea/geometrical_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 import operator
 import re
 
 import astropy.units as u
 import numpy as np
 import pandas as pd
+import pyvista as pv
 import seaborn as sns
 from astropy.coordinates import (CartesianRepresentation, Distance, SkyCoord,
                                  SphericalRepresentation, concatenate)
 from numpy.linalg import norm
 from scipy.spatial.transform import Rotation
 from sunpy.coordinates import frames
 
@@ -358,25 +359,25 @@
         self.tilt = tilt
         self.alpha = orthoaxis1 / orthoaxis2
 
     def intersecting_curve(self):
         """
         Returns the coordinates of intersection of the ellipsoid with a unit sphere
          centred at the origin as `~astropy.coordinates.SkyCoord`.
-        We use vedo package for this calculation.
+        We use pyvista package for this calculation.
         """
-        from vedo import Ellipsoid, Sphere
-        sph = Sphere(pos=(0, 0, 0), r=1)
-        ell = Ellipsoid(pos=(self.rcenter.to_value(1*u.R_sun), 0, 0),
-                        axis1=(2*self.radaxis.to_value(1*u.R_sun), 0, 0),
-                        axis2=(0, 2*self.orthoaxis1.to_value(1*u.R_sun), 0),
-                        axis3=(0, 0, 2*self.orthoaxis2.to_value(1*u.R_sun)))
-        sic = sph.intersectWith(ell)
-        poi = sic.points()
-        x, y, z = self.rotate(poi[:, 0]*u.R_sun, poi[:, 1]*u.R_sun, poi[:, 2]*u.R_sun)
+        ellipsoid = pv.ParametricEllipsoid(self.radaxis.to_value(1*u.R_sun),
+                                           self.orthoaxis1.to_value(1*u.R_sun),
+                                           self.orthoaxis2.to_value(1*u.R_sun),
+                                           u_res=20, v_res=20, w_res=20)
+        ellipsoid = ellipsoid.translate((self.rcenter.to_value(1*u.R_sun), 0, 0), inplace=False)
+        sphere = pv.Sphere(radius=1, center=(0, 0, 0))
+        sic, _, _ = sphere.intersection(ellipsoid)
+
+        x, y, z = self.rotate(sic.points[:, 0]*u.R_sun, sic.points[:, 1]*u.R_sun, sic.points[:, 2]*u.R_sun)
 
         return SkyCoord(CartesianRepresentation(x, y, z),
                         frame=frames.HeliographicStonyhurst,
                         observer=self.center.observer,
                         obstime=self.center.obstime)
 
     @property
```

### Comparing `PyThea-0.7.3/PyThea/modules.py` & `PyThea-0.7.4/PyThea/modules.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/PyThea/pythea_cli.py` & `PyThea-0.7.4/PyThea/pythea_cli.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/utils.py` & `PyThea-0.7.4/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/utils.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/PyThea/sunpy_dev/map/maputils.py` & `PyThea-0.7.4/PyThea/sunpy_dev/map/maputils.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,24 +125,14 @@
 
     Returns
     -------
     `~sunpy.map.GenericMap`
         A SunPy map.
 
     '''
-    indices = []
-    # TODO: This has been added because VSO search returns duplicates for WISPR
-    #       so we manualy filter the dublicates until this problem is solved https://github.com/sunpy/sunpy/issues/5481
-    if 'dublicates' in extra:
-        map_sequence.sort(key=attrgetter('date'))
-        for i in range(0, len(map_sequence)-1):
-            if map_sequence[i].date == map_sequence[i+1].date:
-                indices.append(i)
-        for i in sorted(indices, reverse=True):
-            map_sequence.pop(i)
 
     if 'exposure' in extra:
         map_sequence = [tmap for tmap in map_sequence if tmap.exposure_time > extra['exposure']*u.second]
 
     if 'dimensions' in extra:
         map_sequence = [tmap for tmap in map_sequence if (tmap.dimensions[0], tmap.dimensions[1]) == extra['dimensions']]
```

### Comparing `PyThea-0.7.3/PyThea/test/test_geometrical_models.py` & `PyThea-0.7.4/PyThea/test/test_geometrical_models.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/PyThea/test/test_imports.py` & `PyThea-0.7.4/PyThea/test/test_imports.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/PyThea/test/test_remote_clients.py` & `PyThea-0.7.4/PyThea/test/test_remote_clients.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/PyThea/utils.py` & `PyThea-0.7.4/PyThea/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     axis = plt.subplot(projection=map)
     # TODO: For plain images or when EUVIA-B are used, this does not work very well.
     if image_mode == 'Plain':
         map.plot()
     else:
         map.plot(cmap='Greys_r',
                  norm=colors.Normalize(vmin=clim[0], vmax=clim[1]))
-    map.draw_limb()
+    map.draw_limb(resolution=180)
     # map.draw_grid(linewidth=2, color='red') # TODO: This takes too much computation time. Maybe for AIA or EUVI?
     yax = axis.coords[1]
     yax.set_ticklabel(rotation=90)
     if clip_model:
         axis.set_xlim([0, map.data.shape[0]])
         axis.set_ylim([0, map.data.shape[1]])
```

### Comparing `PyThea-0.7.3/PyThea/version.py` & `PyThea-0.7.4/PyThea/version.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/PyThea.egg-info/PKG-INFO` & `PyThea-0.7.4/PyThea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyThea
-Version: 0.7.3
+Version: 0.7.4
 Summary: PyThea: A software package to reconstruct the 3D structure of CMEs and shock waves
 Home-page: https://github.com/AthKouloumvakos/PyThea
 Author: Athanasios Kouloumvakos
 Author-email: athkouloumvakos@gmail.com
 License: GPL-3.0
 Keywords: science,solar physics,solar,sun,shock waves
 Platform: any
```

### Comparing `PyThea-0.7.3/PyThea.egg-info/SOURCES.txt` & `PyThea-0.7.4/PyThea.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 PyThea/_version.py
 PyThea/callbacks.py
 PyThea/geometrical_models.py
 PyThea/modules.py
 PyThea/pythea_cli.py
 PyThea/utils.py
 PyThea/version.py
+PyThea.egg-info/.DS_Store
 PyThea.egg-info/PKG-INFO
 PyThea.egg-info/SOURCES.txt
 PyThea.egg-info/dependency_links.txt
 PyThea.egg-info/entry_points.txt
 PyThea.egg-info/not-zip-safe
 PyThea.egg-info/requires.txt
 PyThea.egg-info/top_level.txt
```

### Comparing `PyThea-0.7.3/README.md` & `PyThea-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/README_pypi.md` & `PyThea-0.7.4/README_pypi.md`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/environment.yml` & `PyThea-0.7.4/environment.yml`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,14 @@
   - astropy
   - astroquery
   - numexpr
   - sunpy=4.1.0
   - parfive==1.5.1 # With parfive>=2.0.0 there is an issue with streamlit and asyncio (see #13)
   - streamlit
   - seaborn
-  - vedo
+  - pyvista
 # - opencv-python-headless > Introdused to solve a libGL library error and no longe needed. https://github.com/AthKouloumvakos/PyThea/commit/24fa8a46fd4c4ee33aa84ee617d6f3e6628ac8e8
   - pytest-astropy
   - pytest-sugar
   - pip
   - pip:
       - stqdm
```

### Comparing `PyThea-0.7.3/setup.cfg` & `PyThea-0.7.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyThea-0.7.3/setup.py` & `PyThea-0.7.4/setup.py`

 * *Files identical despite different names*

