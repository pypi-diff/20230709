# Comparing `tmp/msgram-1.2.1.tar.gz` & `tmp/msgram-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgram-1.2.1.tar", last modified: Mon Jun 26 20:35:49 2023, max compression
+gzip compressed data, was "msgram-1.2.2.tar", last modified: Sun Jul  9 03:57:22 2023, max compression
```

## Comparing `msgram-1.2.1.tar` & `msgram-1.2.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.434786 msgram-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-06-26 20:35:17.000000 msgram-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    45026 2023-06-26 20:35:49.434786 msgram-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-26 20:35:17.000000 msgram-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.426786 msgram-1.2.1/msgram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45026 2023-06-26 20:35:49.000000 msgram-1.2.1/msgram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-26 20:35:49.000000 msgram-1.2.1/msgram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:35:49.000000 msgram-1.2.1/msgram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 20:35:49.000000 msgram-1.2.1/msgram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-26 20:35:49.000000 msgram-1.2.1/msgram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 20:35:49.000000 msgram-1.2.1/msgram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-26 20:35:17.000000 msgram-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:35:49.434786 msgram-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.426786 msgram-1.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:17.000000 msgram-1.2.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.426786 msgram-1.2.1/src/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.426786 msgram-1.2.1/src/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/commands/cmd_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/commands/cmd_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/commands/cmd_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.426786 msgram-1.2.1/src/cli/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.426786 msgram-1.2.1/src/cli/jsonReader/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/jsonReader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/jsonReader/jsonReader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.430786 msgram-1.2.1/src/cli/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/resources/characteristic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/resources/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/resources/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/resources/subcharacteristic.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/resources/tsqmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-26 20:35:17.000000 msgram-1.2.1/src/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.430786 msgram-1.2.1/src/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:17.000000 msgram-1.2.1/src/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-26 20:35:17.000000 msgram-1.2.1/src/config/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-26 20:35:17.000000 msgram-1.2.1/src/config/setup_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.430786 msgram-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.430786 msgram-1.2.1/tests/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/system/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/system/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/system/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.434786 msgram-1.2.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:35:49.434786 msgram-1.2.1/tests/unit/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/data/file_reader_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_characteristic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_jsonReader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_subcharacteristic.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-26 20:35:17.000000 msgram-1.2.1/tests/unit/test_tsqmi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:22.625947 msgram-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-07-09 03:57:05.000000 msgram-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    45026 2023-07-09 03:57:22.625947 msgram-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-09 03:57:05.000000 msgram-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:22.621947 msgram-1.2.2/msgram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45026 2023-07-09 03:57:22.000000 msgram-1.2.2/msgram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-09 03:57:22.000000 msgram-1.2.2/msgram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 03:57:22.000000 msgram-1.2.2/msgram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-09 03:57:22.000000 msgram-1.2.2/msgram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-09 03:57:22.000000 msgram-1.2.2/msgram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-09 03:57:22.000000 msgram-1.2.2/msgram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-09 03:57:05.000000 msgram-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 03:57:22.625947 msgram-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:22.621947 msgram-1.2.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:05.000000 msgram-1.2.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:22.621947 msgram-1.2.2/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:22.621947 msgram-1.2.2/src/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/commands/cmd_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/commands/cmd_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/commands/cmd_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:22.621947 msgram-1.2.2/src/cli/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:22.621947 msgram-1.2.2/src/cli/jsonReader/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/jsonReader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/jsonReader/jsonReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:22.621947 msgram-1.2.2/src/cli/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/resources/characteristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/resources/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/resources/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/resources/subcharacteristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/resources/tsqmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-09 03:57:05.000000 msgram-1.2.2/src/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:22.621947 msgram-1.2.2/src/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:05.000000 msgram-1.2.2/src/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-09 03:57:05.000000 msgram-1.2.2/src/config/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-09 03:57:05.000000 msgram-1.2.2/src/config/setup_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:22.625947 msgram-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:05.000000 msgram-1.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:22.625947 msgram-1.2.2/tests/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:05.000000 msgram-1.2.2/tests/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-09 03:57:05.000000 msgram-1.2.2/tests/system/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-09 03:57:05.000000 msgram-1.2.2/tests/system/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-09 03:57:05.000000 msgram-1.2.2/tests/system/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:22.625947 msgram-1.2.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:05.000000 msgram-1.2.2/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:57:22.625947 msgram-1.2.2/tests/unit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-07-09 03:57:05.000000 msgram-1.2.2/tests/unit/data/file_reader_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-07-09 03:57:05.000000 msgram-1.2.2/tests/unit/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-09 03:57:05.000000 msgram-1.2.2/tests/unit/test_characteristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-09 03:57:05.000000 msgram-1.2.2/tests/unit/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-09 03:57:05.000000 msgram-1.2.2/tests/unit/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-07-09 03:57:05.000000 msgram-1.2.2/tests/unit/test_jsonReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-09 03:57:05.000000 msgram-1.2.2/tests/unit/test_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-09 03:57:05.000000 msgram-1.2.2/tests/unit/test_subcharacteristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-09 03:57:05.000000 msgram-1.2.2/tests/unit/test_tsqmi.py
```

### Comparing `msgram-1.2.1/LICENSE` & `msgram-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/PKG-INFO` & `msgram-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram
-Version: 1.2.1
+Version: 1.2.2
 Summary: The msgram CLI is a command-line interface to use MeasureSoftGram software
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-1.2.1/README.md` & `msgram-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/msgram.egg-info/PKG-INFO` & `msgram-1.2.2/msgram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram
-Version: 1.2.1
+Version: 1.2.2
 Summary: The msgram CLI is a command-line interface to use MeasureSoftGram software
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-1.2.1/msgram.egg-info/SOURCES.txt` & `msgram-1.2.2/msgram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/pyproject.toml` & `msgram-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgram"
-version = "1.2.1"
+version = "1.2.2"
 description = "The msgram CLI is a command-line interface to use MeasureSoftGram software"
 readme = "README.md"
 authors = [
     { name = "MeasureSoftGram", email = "measuresoftgram@gmail.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
@@ -28,22 +28,22 @@
         "tabulate==0.8.10",
         "termcolor==1.1.0",
         "pandas~=2.0.0",
         "setuptools~=60.2.0",
         "python-dotenv",
         "rich",
         "validators==0.20.0",
-        "msgram-core==1.3.1",
-        "msgram-parser==0.0.7"
+        "msgram-core==1.3.2",
+        "msgram-parser==0.1.0"
     ]
 
 [project.scripts]
 msgram = "src.cli.cli:main"
 
 [tool.mypy]
 strict = true
 
 [project.optional-dependencies]
 dev = ["pytest", "pytest-cov", "setuptools", "wheel"]
 
 [tool.setuptools.packages]
-find = {}
+find = {}
```

### Comparing `msgram-1.2.1/src/cli/cli.py` & `msgram-1.2.2/src/cli/cli.py`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/src/cli/commands/cmd_calculate.py` & `msgram-1.2.2/src/cli/commands/cmd_calculate.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,35 +78,42 @@
         menssage="> See our docs for more information: \n"
         " https://github.com/fga-eps-mds/2022-2-MeasureSoftGram-CLI",
     )
 
 
 def calculate_all(json_data, file_name, config):
     data_measures, _ = calculate_measures(json_data, config)
-
     data_subcharacteristics, _ = calculate_subcharacteristics(
         config, data_measures["measures"]
     )
-
-    data_characteristics, _ = calculate_characteristics(
-        config, data_subcharacteristics["subcharacteristics"]
+    data_characteristics, _ = (
+        calculate_characteristics(config, data_subcharacteristics["subcharacteristics"])
+        if data_subcharacteristics["subcharacteristics"]
+        else ([], [])
+    )
+    data_tsqmi, _ = (
+        calculate_tsqmi(config, data_characteristics["characteristics"])
+        if data_characteristics
+        else ([], [])
     )
-
-    data_tsqmi, _ = calculate_tsqmi(config, data_characteristics["characteristics"])
 
     version = re.search(r"\d{1,2}-\d{1,2}-\d{4}-\d{1,2}-\d{1,2}", file_name)[0]
     repository = file_name.split(version)[0][:-1]
 
     return {
         "repository": [{"key": "repository", "value": repository}],
-        "version": [{"key": "version", "value": version}],
-        "measures": data_measures["measures"],
-        "subcharacteristics": data_subcharacteristics["subcharacteristics"],
-        "characteristics": data_characteristics["characteristics"],
-        "tsqmi": data_tsqmi["tsqmi"],
+        "version": [{"key": "version", "value": version}] if version else [],
+        "measures": data_measures["measures"] if data_measures else [],
+        "subcharacteristics": data_subcharacteristics["subcharacteristics"]
+        if data_subcharacteristics
+        else [],
+        "characteristics": data_characteristics["characteristics"]
+        if data_characteristics
+        else [],
+        "tsqmi": data_tsqmi["tsqmi"] if data_tsqmi else [],
     }
 
 
 def show_results(output_format, data_calculated, config_path):
     if output_format == "tabular":
         show_tabulate(data_calculated)
```

### Comparing `msgram-1.2.1/src/cli/commands/cmd_init.py` & `msgram-1.2.2/src/cli/commands/cmd_init.py`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/src/cli/exceptions/exceptions.py` & `msgram-1.2.2/src/cli/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/src/cli/jsonReader/jsonReader.py` & `msgram-1.2.2/src/cli/jsonReader/jsonReader.py`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/src/cli/parsers.py` & `msgram-1.2.2/src/cli/parsers.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,23 +45,22 @@
     parser_extract.add_argument(
         "-o",
         "--output_origin",
         required=True,
         type=str,
         choices=(AVAILABLE_IMPORTS),
         help=(
-            "Import a metrics files from some origin. Valid values are: "
+            "Import a metrics files/repository from some origin. Valid values are: "
             + ", ".join(AVAILABLE_IMPORTS)
         ),
     )
 
     parser_extract.add_argument(
         "-dp",
         "--data_path",
-        required=True,
         type=lambda p: Path(p).absolute(),
         help="Path to analysis data directory",
     )
 
     parser_extract.add_argument(
         "-ep",
         "--extracted_path",
@@ -73,14 +72,22 @@
     parser_extract.add_argument(
         "-le",
         "--language_extension",
         type=str,
         help="The source code language extension",
         default="py",
     )
+
+    parser_extract.add_argument(
+        "-rep",
+        "--repository_path",
+        type=str,
+        help="Path to analysis git repository",
+    )
+
     parser_extract.set_defaults(func=command_extract)  # function command extract
 
     # =====================================< COMMAND calculate >=====================================
     parser_calculate = subparsers.add_parser(
         "calculate",
         help="Calculates all entities",
     )
```

### Comparing `msgram-1.2.1/src/cli/resources/characteristic.py` & `msgram-1.2.2/src/cli/resources/characteristic.py`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/src/cli/resources/measure.py` & `msgram-1.2.2/src/cli/resources/measure.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,21 @@
 
     calculate_infos = []
     for measures in SUPPORTED_MEASURES:
         calculate_infos.append(
             {
                 "key": list(measures.keys())[0],
                 "parameters": {
-                    metric: extracted[metric]
+                    metric: extracted[metric] if extracted.get(metric) else None
                     for metric in list(measures.values())[0]["metrics"]
                 },
             }
         )
+        new_metrics = []
+        for measure in calculate_infos:
+            if measure.get("parameters", None) and all(measure["parameters"].values()):
+                new_metrics.append(measure)
+
+        calculate_infos = new_metrics
 
     headers = ["Id", "Name", "Description", "Value", "Created at"]
     return core_calculate({"measures": calculate_infos}, config), headers
```

### Comparing `msgram-1.2.1/src/cli/resources/metrics.py` & `msgram-1.2.2/src/cli/resources/metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,25 +13,21 @@
 
     # Métricas que o parâmetro é extraido do UTS
     uts_values = ["test_execution_time", "tests"]
     response_data = {}
 
     # Para todos os arquivos extraidos
     for path_readed in extracted.values():
-        qualifier = path_readed["qualifier"]
-        measures = path_readed["measures"]
-
         # Para cada métrica dentro das medidas
-        for metric in measures:
+        for metric in path_readed:
             metric_name = metric["metric"]
             metric_value = metric["value"]
 
             # Se ela for "agregada", olho apenas arquivos FIL,
             # se não, salvo somente a última.
-            if metric_name in listed_values and qualifier == "FIL":
-                response_data.setdefault(metric_name, []).append(metric_value)
-            elif metric_name in uts_values and qualifier == "UTS":
+            all_value_list = listed_values + uts_values
+            if metric_name in all_value_list:
                 response_data.setdefault(metric_name, []).append(metric_value)
-            elif metric_name not in (listed_values + uts_values) and qualifier == "TRK":
+            else:
                 response_data[metric_name] = metric_value
 
     return response_data
```

### Comparing `msgram-1.2.1/src/cli/resources/subcharacteristic.py` & `msgram-1.2.2/src/cli/resources/subcharacteristic.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,29 +7,35 @@
     subchar_calculated = []
     for subchar in char:
         subchar_key = subchar["key"]
 
         subchar_calculated.append(
             {
                 "key": subchar_key,
-                "value": {m["key"]: m["value"] for m in subchars}[subchar_key],
+                "value": {m["key"]: m["value"] for m in subchars}.get(
+                    subchar_key, None
+                ),
                 "weight": subchar["weight"],
             }
         )
 
     return subchar_calculated
 
 
 def calculate_subcharacteristics(config, measures):
     subchars = [sc["subcharacteristics"] for sc in config["characteristics"]]
     calculate_infos = []
 
-    for subchar in subchars:
-        calculate_infos.append(
+    calculate_infos = [
+        (
             {
                 "key": subchar[0]["key"],
                 "measures": get_measure_value(measures, subchar[0]["measures"]),
             }
         )
-
+        if measures
+        else None
+        for subchar in subchars
+    ]
+    calculate_infos = list(filter(None, calculate_infos))
     headers = ["Id", "Name", "Description", "Value", "Created at"]
     return core_calculate({"subcharacteristics": calculate_infos}), headers
```

### Comparing `msgram-1.2.1/src/cli/utils.py` & `msgram-1.2.2/src/cli/utils.py`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/src/config/settings.py` & `msgram-1.2.2/src/config/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ]
 
 SUPPORTED_FORMATS = [
     "json",
     "tabular",
 ]
 
-AVAILABLE_IMPORTS = ["sonarqube"]
+AVAILABLE_IMPORTS = ["sonarqube", "github"]
 
 AVAILABLE_GEN_FORMATS = ["csv", "json"]
 
 SUPPORTED_MEASURES = [
     {
         "passed_tests": {
             "metrics": [
```

### Comparing `msgram-1.2.1/src/config/setup_log.py` & `msgram-1.2.2/src/config/setup_log.py`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/tests/system/test_extract.py` & `msgram-1.2.2/tests/system/test_extract.py`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/tests/system/test_help.py` & `msgram-1.2.2/tests/system/test_help.py`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/tests/system/test_init.py` & `msgram-1.2.2/tests/system/test_init.py`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/tests/unit/data/file_reader_response.py` & `msgram-1.2.2/tests/unit/data/file_reader_response.py`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/tests/unit/test_calculate.py` & `msgram-1.2.2/tests/unit/test_calculate.py`

 * *Files 23% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     args = {
         "output_format": output_format,
         "config_path": Path(config_dirpath),
         "extracted_path": Path(
             extract_dirpath + (f"/{extracted_file_name}" if not mult_file else "")
         ),
     }
-
     if not mult_file:
         calculate_patch = patch("builtins.input", return_value=output_format)
         calculate_patch.start()
 
     command_calculate(args)
 
     assert len(os.listdir(config_dirpath)) == 2 if mult_file else 1
@@ -83,68 +82,103 @@
 
 
 def test_calculate_all_dict():
     file_name = "fga-eps-mds-2022-2-MeasureSoftGram-CLI-01-05-2023-21-40-30-develop-extracted.msgram"
     json_data = open_json_file(Path(f"tests/unit/data/{file_name}"))
     config = open_json_file(Path("tests/unit/data/msgram.json"))
 
-    calculated = calculate_all(json_data, file_name, config)
-    print(calculated)
-    assert calculated == {
+    calculated_result = calculate_all(json_data, file_name, config)
+    calculate_expected = {
         "repository": [
             {"key": "repository", "value": "fga-eps-mds-2022-2-MeasureSoftGram-CLI"}
         ],
         "version": [{"key": "version", "value": "01-05-2023-21-40"}],
         "measures": [
             {"key": "passed_tests", "value": 1.0},
             {
                 "key": "test_builds",
-                "value": pytest.approx(0.9996969618055556, 0.00000000000001),
+                "value": 0.9996066627522133,
             },
             {
                 "key": "test_coverage",
-                "value": pytest.approx(0.4707692307692307, 0.00000000000001),
+                "value": 0.40234848484848484,
             },
             {
                 "key": "non_complex_file_density",
-                "value": pytest.approx(0.3789488966318234, 0.00000000000001),
+                "value": 0.44347274991556906,
             },
             {
                 "key": "commented_file_density",
-                "value": pytest.approx(0.029230769230769227, 0.00000000000001),
+                "value": 0.04318181818181818,
             },
             {"key": "duplication_absense", "value": 1.0},
         ],
         "subcharacteristics": [
             {
                 "key": "testing_status",
-                "value": pytest.approx(0.8543507067377631, 0.00000000000001),
+                "value": 0.8421061048464034,
             },
             {
                 "key": "modifiability",
-                "value": pytest.approx(0.6276266582884098, 0.00000000000001),
+                "value": 0.6415437113263573,
             },
         ],
         "characteristics": [
             {
                 "key": "reliability",
-                "value": pytest.approx(0.8543507067377631, 0.00000000000001),
+                "value": 0.8421061048464034,
             },
             {
                 "key": "maintainability",
-                "value": pytest.approx(0.6276266582884098, 0.00000000000001),
+                "value": 0.6415437113263573,
             },
         ],
         "tsqmi": [
             {
                 "key": "tsqmi",
-                "value": pytest.approx(0.7496100160408716, 0.00000000000001),
+                "value": 0.7485723162667646,
             }
         ],
     }
+    assert calculated_result.get("repository") == calculate_expected.get("repository")
+    assert calculated_result.get("version") == calculate_expected.get("version")
+    measures_result = calculated_result.get("measures")
+    measures_expected = calculate_expected.get("measures")
+    for measure_result, measure_expected in zip(measures_result, measures_expected):
+        assert measure_result.get("key") == measure_expected.get("key")
+        assert pytest.approx(measure_result.get("value")) == measure_expected.get(
+            "value"
+        )
+
+    subcharacteristics_result = calculated_result.get("subcharacteristics")
+    subcharacteristics_expected = calculate_expected.get("subcharacteristics")
+    for subcharacteristic_result, subcharacteristic_expected in zip(
+        subcharacteristics_result, subcharacteristics_expected
+    ):
+        assert subcharacteristic_result.get("key") == subcharacteristic_expected.get(
+            "key"
+        )
+        assert pytest.approx(
+            subcharacteristic_result.get("value")
+        ) == subcharacteristic_expected.get("value")
+
+    characteristics_result = calculated_result.get("characteristics")
+    characteristics_expected = calculate_expected.get("characteristics")
+    for characteristic_result, characteristic_expected in zip(
+        characteristics_result, characteristics_expected
+    ):
+        assert characteristic_result.get("key") == characteristic_expected.get("key")
+        assert pytest.approx(
+            characteristic_result.get("value")
+        ) == characteristic_expected.get("value")
+
+    tsqmi_result = calculated_result.get("tsqmi")[0]
+    tsqmi_expected = calculate_expected.get("tsqmi")[0]
+    assert tsqmi_result.get("key") == tsqmi_expected.get("key")
+    assert pytest.approx(tsqmi_result.get("value")) == tsqmi_expected.get("value")
 
 
 def test_calculate_invalid_config_file():
     captured_output = StringIO()
     sys.stdout = captured_output
 
     config_dirpath = tempfile.mkdtemp()
```

### Comparing `msgram-1.2.1/tests/unit/test_characteristic.py` & `msgram-1.2.2/tests/unit/test_characteristic.py`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/tests/unit/test_extract.py` & `msgram-1.2.2/tests/unit/test_extract.py`

 * *Files 16% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     shutil.rmtree(config_dirpath)
     shutil.rmtree(extract_dirpath)
 
 
 @pytest.mark.parametrize(
     "extract_arg",
-    ["output_origin", "extracted_path", "data_path", "language_extension"],
+    ["output_origin", "extracted_path", "language_extension"],
 )
 def test_extract_invalid_args(extract_arg):
     captured_output = StringIO()
     sys.stdout = captured_output
 
     args = copy.deepcopy(EXTRACT_ARGS)
     del args[extract_arg]
@@ -89,19 +89,44 @@
     sys.stdout = sys.__stdout__
     assert (
         f"KeyError: args['{extract_arg}'] - non-existent parameters"
         in captured_output.getvalue()
     )
 
 
-def test_command_extract_extracted_path_is_not_a_dir():
+def test_extract_fail_no_dp_or_rep():
+    extract_dirpath = tempfile.mkdtemp()
+    args = {
+        "output_origin": "sonarqube",
+        "language_extension": "py",
+        "extracted_path": Path(extract_dirpath),
+    }
+
     captured_output = StringIO()
     sys.stdout = captured_output
+    with pytest.raises(SystemExit):
+        command_extract(args)
 
-    args = copy.deepcopy(EXTRACT_ARGS)
-    args["extracted_path"] = Path("inexistent")
+    sys.stdout = sys.__stdout__
+
+    assert (
+        "It is necessary to pass the data_path or repository_path parameters"
+        in captured_output.getvalue()
+    )
+
+
+def test_extract_directory_not_exist():
+    args = {
+        "output_origin": "sonarqube",
+        "language_extension": "py",
+        "extracted_path": Path("tests/directory_not_exist"),
+        "data_path": Path("tests/directory_not_exist"),
+    }
 
+    captured_output = StringIO()
+    sys.stdout = captured_output
     with pytest.raises(SystemExit):
         command_extract(args)
 
     sys.stdout = sys.__stdout__
+
     assert "FileNotFoundError: extract directory" in captured_output.getvalue()
```

### Comparing `msgram-1.2.1/tests/unit/test_init.py` & `msgram-1.2.2/tests/unit/test_init.py`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/tests/unit/test_jsonReader.py` & `msgram-1.2.2/tests/unit/test_jsonReader.py`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/tests/unit/test_measures.py` & `msgram-1.2.2/tests/unit/test_measures.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,18 @@
     infos, headers = calculate_measures(json_data)
     assert headers == ["Id", "Name", "Description", "Value", "Created at"]
     assert "measures" in infos
 
     measure_result = infos.get("measures")
     measure_expected = [
         {"key": "passed_tests", "value": 1.0},
-        {"key": "test_builds", "value": 0.9996969618055556},
-        {"key": "test_coverage", "value": 0.4707692307692307},
-        {"key": "non_complex_file_density", "value": 0.3789488966318234},
-        {"key": "commented_file_density", "value": 0.029230769230769227},
+        {"key": "test_builds", "value": 0.9996066627522133},
+        {"key": "test_coverage", "value": 0.40234848484848484},
+        {"key": "non_complex_file_density", "value": 0.44347274991556906},
+        {"key": "commented_file_density", "value": 0.04318181818181818},
         {"key": "duplication_absense", "value": 1.0},
     ]
     for measure_result, measure_expected in zip(measure_result, measure_expected):
         assert measure_result.get("key") == measure_expected.get("key")
         assert pytest.approx(measure_result.get("value")) == measure_expected.get(
             "value"
         )
```

### Comparing `msgram-1.2.1/tests/unit/test_subcharacteristic.py` & `msgram-1.2.2/tests/unit/test_subcharacteristic.py`

 * *Files identical despite different names*

### Comparing `msgram-1.2.1/tests/unit/test_tsqmi.py` & `msgram-1.2.2/tests/unit/test_tsqmi.py`

 * *Files identical despite different names*

