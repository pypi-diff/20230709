# Comparing `tmp/pwforecast-1.1.0.tar.gz` & `tmp/pwforecast-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwforecast-1.1.0.tar", last modified: Sun Jul  9 02:40:10 2023, max compression
+gzip compressed data, was "pwforecast-1.1.1.tar", last modified: Sun Jul  9 03:07:36 2023, max compression
```

## Comparing `pwforecast-1.1.0.tar` & `pwforecast-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:40:10.443442 pwforecast-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-09 02:39:57.000000 pwforecast-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-09 02:40:10.443442 pwforecast-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-09 02:39:57.000000 pwforecast-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:40:10.443442 pwforecast-1.1.0/pwforecast/
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-07-09 02:39:57.000000 pwforecast-1.1.0/pwforecast/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:40:10.443442 pwforecast-1.1.0/pwforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-09 02:40:10.000000 pwforecast-1.1.0/pwforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-09 02:40:10.000000 pwforecast-1.1.0/pwforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 02:40:10.000000 pwforecast-1.1.0/pwforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-09 02:40:10.000000 pwforecast-1.1.0/pwforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 02:40:10.000000 pwforecast-1.1.0/pwforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 02:40:10.443442 pwforecast-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-09 02:39:57.000000 pwforecast-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:07:36.719890 pwforecast-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-09 03:07:24.000000 pwforecast-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-09 03:07:36.719890 pwforecast-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-09 03:07:24.000000 pwforecast-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:07:36.719890 pwforecast-1.1.1/pwforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-07-09 03:07:24.000000 pwforecast-1.1.1/pwforecast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:07:36.719890 pwforecast-1.1.1/pwforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-09 03:07:36.000000 pwforecast-1.1.1/pwforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-09 03:07:36.000000 pwforecast-1.1.1/pwforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 03:07:36.000000 pwforecast-1.1.1/pwforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-09 03:07:36.000000 pwforecast-1.1.1/pwforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 03:07:36.000000 pwforecast-1.1.1/pwforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 03:07:36.719890 pwforecast-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-09 03:07:24.000000 pwforecast-1.1.1/setup.py
```

### Comparing `pwforecast-1.1.0/LICENSE` & `pwforecast-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pwforecast-1.1.0/PKG-INFO` & `pwforecast-1.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: pwforecast
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.
 Home-page: https://github.com/timhawker/pwforecast
 Author: Tim Hawker
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PwForecast
 
 A Python module to charge/discharge Powerwall based on solar forecast and peak/off-peak tariffs. 
 
-Utilises the excellent [TeslaPy](https://tesla-api.timdorr.com/) by Tim Dorssers.
+Utilises the excellent [TeslaPy](https://github.com/tdorssers/TeslaPy) by Tim Dorssers.
 
 PwForecast is primarily designed for those with dual rate tariffs. If there is interest in expanding this to provide
 more flexible control for those with more complex tariffs, please let me know.
 
 [![Version](https://img.shields.io/pypi/v/pwforecast)](https://pypi.org/project/pwforecast)
 
 
 ## Getting Started
 
 PwForecast requires a Solcast API key and Site ID. You can sign up for a 
 [free Hobbyist account](https://toolkit.solcast.com.au/register) which allows up to two sites and 50 API calls per day. 
 
-[TeslaPy](https://tesla-api.timdorr.com/) has great documentation on getting started. It even works with two-factor
+[TeslaPy](https://github.com/tdorssers/TeslaPy) has great documentation on getting started. It even works with two-factor
 authentication enabled.
 
-Rather than inherit [TeslaPy](https://tesla-api.timdorr.com/), PwForecast requires an instance of a Tesla class passed 
-to it. This allows you to configure the object based on your credentials before passing to PwForecast.  
+Rather than inherit, PwForecast requires an instance of a [TeslaPy](https://github.com/tdorssers/TeslaPy) Tesla class 
+passed to it. This allows you to configure the object based on your credentials before passing to PwForecast.  
 
 When using PwForecast, Self Powered mode is recommended. Time Based Control could be used if you need to charge
 faster than 1.7kW per Powerwall, but results may be unpredictable. 
 
 
 ## Overview
```

### Comparing `pwforecast-1.1.0/README.md` & `pwforecast-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 ## PwForecast
 
 A Python module to charge/discharge Powerwall based on solar forecast and peak/off-peak tariffs. 
 
-Utilises the excellent [TeslaPy](https://tesla-api.timdorr.com/) by Tim Dorssers.
+Utilises the excellent [TeslaPy](https://github.com/tdorssers/TeslaPy) by Tim Dorssers.
 
 PwForecast is primarily designed for those with dual rate tariffs. If there is interest in expanding this to provide
 more flexible control for those with more complex tariffs, please let me know.
 
 [![Version](https://img.shields.io/pypi/v/pwforecast)](https://pypi.org/project/pwforecast)
 
 
 ## Getting Started
 
 PwForecast requires a Solcast API key and Site ID. You can sign up for a 
 [free Hobbyist account](https://toolkit.solcast.com.au/register) which allows up to two sites and 50 API calls per day. 
 
-[TeslaPy](https://tesla-api.timdorr.com/) has great documentation on getting started. It even works with two-factor
+[TeslaPy](https://github.com/tdorssers/TeslaPy) has great documentation on getting started. It even works with two-factor
 authentication enabled.
 
-Rather than inherit [TeslaPy](https://tesla-api.timdorr.com/), PwForecast requires an instance of a Tesla class passed 
-to it. This allows you to configure the object based on your credentials before passing to PwForecast.  
+Rather than inherit, PwForecast requires an instance of a [TeslaPy](https://github.com/tdorssers/TeslaPy) Tesla class 
+passed to it. This allows you to configure the object based on your credentials before passing to PwForecast.  
 
 When using PwForecast, Self Powered mode is recommended. Time Based Control could be used if you need to charge
 faster than 1.7kW per Powerwall, but results may be unpredictable. 
 
 
 ## Overview
```

### Comparing `pwforecast-1.1.0/pwforecast/__init__.py` & `pwforecast-1.1.1/pwforecast/__init__.py`

 * *Files identical despite different names*

### Comparing `pwforecast-1.1.0/pwforecast.egg-info/PKG-INFO` & `pwforecast-1.1.1/pwforecast.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: pwforecast
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.
 Home-page: https://github.com/timhawker/pwforecast
 Author: Tim Hawker
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PwForecast
 
 A Python module to charge/discharge Powerwall based on solar forecast and peak/off-peak tariffs. 
 
-Utilises the excellent [TeslaPy](https://tesla-api.timdorr.com/) by Tim Dorssers.
+Utilises the excellent [TeslaPy](https://github.com/tdorssers/TeslaPy) by Tim Dorssers.
 
 PwForecast is primarily designed for those with dual rate tariffs. If there is interest in expanding this to provide
 more flexible control for those with more complex tariffs, please let me know.
 
 [![Version](https://img.shields.io/pypi/v/pwforecast)](https://pypi.org/project/pwforecast)
 
 
 ## Getting Started
 
 PwForecast requires a Solcast API key and Site ID. You can sign up for a 
 [free Hobbyist account](https://toolkit.solcast.com.au/register) which allows up to two sites and 50 API calls per day. 
 
-[TeslaPy](https://tesla-api.timdorr.com/) has great documentation on getting started. It even works with two-factor
+[TeslaPy](https://github.com/tdorssers/TeslaPy) has great documentation on getting started. It even works with two-factor
 authentication enabled.
 
-Rather than inherit [TeslaPy](https://tesla-api.timdorr.com/), PwForecast requires an instance of a Tesla class passed 
-to it. This allows you to configure the object based on your credentials before passing to PwForecast.  
+Rather than inherit, PwForecast requires an instance of a [TeslaPy](https://github.com/tdorssers/TeslaPy) Tesla class 
+passed to it. This allows you to configure the object based on your credentials before passing to PwForecast.  
 
 When using PwForecast, Self Powered mode is recommended. Time Based Control could be used if you need to charge
 faster than 1.7kW per Powerwall, but results may be unpredictable. 
 
 
 ## Overview
```

### Comparing `pwforecast-1.1.0/setup.py` & `pwforecast-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 
 # read the contents of README file
 readme = (this_directory / 'README.md').read_text()
 
 setuptools.setup(
     name='pwforecast',
-    version='1.1.0',
+    version='1.1.1',
     author='Tim Hawker',
     description='A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.',
     url='https://github.com/timhawker/pwforecast',
     long_description_content_type='text/markdown',
     long_description=readme,
     packages=['pwforecast'],
     install_requires=['tzlocal', 'requests', 'python-dateutil', 'TeslaPy']
```

