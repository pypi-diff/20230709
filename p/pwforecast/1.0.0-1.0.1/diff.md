# Comparing `tmp/pwforecast-1.0.0.tar.gz` & `tmp/pwforecast-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwforecast-1.0.0.tar", last modified: Sat Jul  8 21:34:40 2023, max compression
+gzip compressed data, was "pwforecast-1.0.1.tar", last modified: Sat Jul  8 22:53:50 2023, max compression
```

## Comparing `pwforecast-1.0.0.tar` & `pwforecast-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:34:40.954244 pwforecast-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-08 21:34:29.000000 pwforecast-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-07-08 21:34:40.954244 pwforecast-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-08 21:34:29.000000 pwforecast-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:34:40.954244 pwforecast-1.0.0/pwforecast/
--rw-r--r--   0 runner    (1001) docker     (123)    15974 2023-07-08 21:34:29.000000 pwforecast-1.0.0/pwforecast/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:34:40.954244 pwforecast-1.0.0/pwforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-07-08 21:34:40.000000 pwforecast-1.0.0/pwforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-08 21:34:40.000000 pwforecast-1.0.0/pwforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:34:40.000000 pwforecast-1.0.0/pwforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-08 21:34:40.000000 pwforecast-1.0.0/pwforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 21:34:40.000000 pwforecast-1.0.0/pwforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:34:40.954244 pwforecast-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-08 21:34:29.000000 pwforecast-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:50.978203 pwforecast-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-08 22:53:41.000000 pwforecast-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-08 22:53:50.978203 pwforecast-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-08 22:53:41.000000 pwforecast-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:50.978203 pwforecast-1.0.1/pwforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-07-08 22:53:41.000000 pwforecast-1.0.1/pwforecast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:50.978203 pwforecast-1.0.1/pwforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-08 22:53:50.000000 pwforecast-1.0.1/pwforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-08 22:53:50.000000 pwforecast-1.0.1/pwforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:53:50.000000 pwforecast-1.0.1/pwforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-08 22:53:50.000000 pwforecast-1.0.1/pwforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 22:53:50.000000 pwforecast-1.0.1/pwforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 22:53:50.978203 pwforecast-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-08 22:53:41.000000 pwforecast-1.0.1/setup.py
```

### Comparing `pwforecast-1.0.0/LICENSE` & `pwforecast-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pwforecast-1.0.0/PKG-INFO` & `pwforecast-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: pwforecast
-Version: 1.0.0
-Summary: A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.
-Home-page: https://github.com/timhawker/pwforecast
-Author: Tim Hawker
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## PwForecast
 
 A Python module to charge/discharge Powerwall based on solar forecast and peak/off-peak tariffs. 
 
 Utilises the excellent [TeslaPy](https://tesla-api.timdorr.com/) by Tim Dorssers.
 
 PwForecast is primarily designed for those with dual rate tariffs. If there is interest in expanding this to provide
@@ -65,31 +56,53 @@
 to by setting the `min_reserve_peak_rate` value.
 
 ```python
 pw_forecast.min_reserve_peak_rate = 10  # Default 20
 pw_forecast.set_peak_mode()
 ```
 
+PwForecast will try to ensure power flow behaves as expected. Please see [Retry Logic](#retry-logic) for more info. 
+
+A summary report will then be printed:
+```text
+-----------------------------------
+Powerwall state of charge: 19.7%
+Powerwall backup reserve: 100%
+Powerwall capacity: 26.59kWh
+Powerwall state of health: 95.0%
+-----------------------------------
+```
+
 
 ## Setting Off-Peak Mode
 
 Use this method when your off-peak rate starts. This requires a little more configuration.
  * Configure what backup reserve the Powerwall can discharge down to by setting the 'min_reserve_off_peak_rate' attribute.
  * Configure the maximum backup reserve allowed by setting the 'max_reserve' attribute. 
- * Configure the amount of energy you require during the peak-rate. 
-
-TODO: ADD BIT ABOUT TAKING 20 SECONDS, SHOW OUTPUT
+ * Configure the amount of energy you require during the peak-rate.
 
 ```python
 pw_forecast.min_reserve_off_peak_rate = 25  # Default 30
 pw_forecast.max_reserve = 95  # Default 100
 pw_forecast.required_energy_peak_rate = 20000  # Default 30000
 pw_forecast.set_off_peak_mode()
 ```
 
+PwForecast will try to ensure power flow behaves as expected. Please see [Retry Logic](#retry-logic) for more info. 
+
+A summary report will then be printed:
+```text
+-----------------------------------
+Solar forecast tomorrow: 10.2kWh
+Powerwall state of charge: 19.7%
+Powerwall backup reserve: 100%
+Powerwall capacity: 26.59kWh
+Powerwall state of health: 95.0%
+-----------------------------------
+```
 
 ## Retry Logic
 
 When setting backup reserve, it is common to take two or three attempts before power flow changes to the expected 
 figures. As the Tesla API is unofficial, it is difficult to determine why. Waiting longer does not seem to fix this 
 issue, although waiting upwards of 45 minutes does sometimes result in power flow eventually changing correctly. 
 Re-applying the setting does appear to fix this issue. Perhaps the unofficial Tesla API is missing a commit command.
```

### Comparing `pwforecast-1.0.0/README.md` & `pwforecast-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: pwforecast
+Version: 1.0.1
+Summary: A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.
+Home-page: https://github.com/timhawker/pwforecast
+Author: Tim Hawker
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## PwForecast
 
 A Python module to charge/discharge Powerwall based on solar forecast and peak/off-peak tariffs. 
 
 Utilises the excellent [TeslaPy](https://tesla-api.timdorr.com/) by Tim Dorssers.
 
 PwForecast is primarily designed for those with dual rate tariffs. If there is interest in expanding this to provide
@@ -56,31 +65,53 @@
 to by setting the `min_reserve_peak_rate` value.
 
 ```python
 pw_forecast.min_reserve_peak_rate = 10  # Default 20
 pw_forecast.set_peak_mode()
 ```
 
+PwForecast will try to ensure power flow behaves as expected. Please see [Retry Logic](#retry-logic) for more info. 
+
+A summary report will then be printed:
+```text
+-----------------------------------
+Powerwall state of charge: 19.7%
+Powerwall backup reserve: 100%
+Powerwall capacity: 26.59kWh
+Powerwall state of health: 95.0%
+-----------------------------------
+```
+
 
 ## Setting Off-Peak Mode
 
 Use this method when your off-peak rate starts. This requires a little more configuration.
  * Configure what backup reserve the Powerwall can discharge down to by setting the 'min_reserve_off_peak_rate' attribute.
  * Configure the maximum backup reserve allowed by setting the 'max_reserve' attribute. 
- * Configure the amount of energy you require during the peak-rate. 
-
-TODO: ADD BIT ABOUT TAKING 20 SECONDS, SHOW OUTPUT
+ * Configure the amount of energy you require during the peak-rate.
 
 ```python
 pw_forecast.min_reserve_off_peak_rate = 25  # Default 30
 pw_forecast.max_reserve = 95  # Default 100
 pw_forecast.required_energy_peak_rate = 20000  # Default 30000
 pw_forecast.set_off_peak_mode()
 ```
 
+PwForecast will try to ensure power flow behaves as expected. Please see [Retry Logic](#retry-logic) for more info. 
+
+A summary report will then be printed:
+```text
+-----------------------------------
+Solar forecast tomorrow: 10.2kWh
+Powerwall state of charge: 19.7%
+Powerwall backup reserve: 100%
+Powerwall capacity: 26.59kWh
+Powerwall state of health: 95.0%
+-----------------------------------
+```
 
 ## Retry Logic
 
 When setting backup reserve, it is common to take two or three attempts before power flow changes to the expected 
 figures. As the Tesla API is unofficial, it is difficult to determine why. Waiting longer does not seem to fix this 
 issue, although waiting upwards of 45 minutes does sometimes result in power flow eventually changing correctly. 
 Re-applying the setting does appear to fix this issue. Perhaps the unofficial Tesla API is missing a commit command.
```

### Comparing `pwforecast-1.0.0/pwforecast/__init__.py` & `pwforecast-1.0.1/pwforecast/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         """
         for i in range(1, self.global_retry + 1):
             try:
                 # status update
                 msg = 'Setting peak mode, attempt {i} of {total}'
                 print(msg.format(i=i, total=self.global_retry))
                 # set the peak reserve
-                status = self._set_backup_reserve_percent(self.min_reserve_peak_rate)
+                status = self.set_backup_reserve_percent(self.min_reserve_peak_rate)
                 self._print_summary(**status)
             except Exception as e:
                 if i == self.global_retry:
                     raise
                 msg = '{c}: {e}'
                 print(msg.format(c=e.__class__.__name__, e=e))
                 # sleep in case of temporary outage
@@ -327,15 +327,15 @@
             soc (float): The Powerwall state of charge.
             reserve (float): The Powerwall backup reserve percentage.
             capacity (float): The Powerwall total capacity in Wh.
             soh (float): The Powerwall overall state of health percentage.
             solar_forecast (float): The solar forecast in Wh.
 
         """
-        print('-' * 20)
+        print('-' * 35)
         if solar_forecast:
             print('Solar forecast tomorrow: {:.1f}kWh'.format(solar_forecast/1000))
         print('Powerwall state of charge: {:.1f}%'.format(soc))
         print('Powerwall backup reserve: {}%'.format(reserve))
         print('Powerwall capacity: {:.2f}kWh'.format(capacity/1000))
         print('Powerwall state of health: {:.1f}%'.format(soh))
-        print('-' * 20)
+        print('-' * 35)
```

### Comparing `pwforecast-1.0.0/pwforecast.egg-info/PKG-INFO` & `pwforecast-1.0.1/pwforecast.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwforecast
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.
 Home-page: https://github.com/timhawker/pwforecast
 Author: Tim Hawker
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PwForecast
@@ -65,31 +65,53 @@
 to by setting the `min_reserve_peak_rate` value.
 
 ```python
 pw_forecast.min_reserve_peak_rate = 10  # Default 20
 pw_forecast.set_peak_mode()
 ```
 
+PwForecast will try to ensure power flow behaves as expected. Please see [Retry Logic](#retry-logic) for more info. 
+
+A summary report will then be printed:
+```text
+-----------------------------------
+Powerwall state of charge: 19.7%
+Powerwall backup reserve: 100%
+Powerwall capacity: 26.59kWh
+Powerwall state of health: 95.0%
+-----------------------------------
+```
+
 
 ## Setting Off-Peak Mode
 
 Use this method when your off-peak rate starts. This requires a little more configuration.
  * Configure what backup reserve the Powerwall can discharge down to by setting the 'min_reserve_off_peak_rate' attribute.
  * Configure the maximum backup reserve allowed by setting the 'max_reserve' attribute. 
- * Configure the amount of energy you require during the peak-rate. 
-
-TODO: ADD BIT ABOUT TAKING 20 SECONDS, SHOW OUTPUT
+ * Configure the amount of energy you require during the peak-rate.
 
 ```python
 pw_forecast.min_reserve_off_peak_rate = 25  # Default 30
 pw_forecast.max_reserve = 95  # Default 100
 pw_forecast.required_energy_peak_rate = 20000  # Default 30000
 pw_forecast.set_off_peak_mode()
 ```
 
+PwForecast will try to ensure power flow behaves as expected. Please see [Retry Logic](#retry-logic) for more info. 
+
+A summary report will then be printed:
+```text
+-----------------------------------
+Solar forecast tomorrow: 10.2kWh
+Powerwall state of charge: 19.7%
+Powerwall backup reserve: 100%
+Powerwall capacity: 26.59kWh
+Powerwall state of health: 95.0%
+-----------------------------------
+```
 
 ## Retry Logic
 
 When setting backup reserve, it is common to take two or three attempts before power flow changes to the expected 
 figures. As the Tesla API is unofficial, it is difficult to determine why. Waiting longer does not seem to fix this 
 issue, although waiting upwards of 45 minutes does sometimes result in power flow eventually changing correctly. 
 Re-applying the setting does appear to fix this issue. Perhaps the unofficial Tesla API is missing a commit command.
```

### Comparing `pwforecast-1.0.0/setup.py` & `pwforecast-1.0.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 
 # read the contents of README file
 readme = (this_directory / 'README.md').read_text()
 
 setuptools.setup(
     name='pwforecast',
-    version='1.0.0',
+    version='1.0.1',
     author='Tim Hawker',
     description='A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.',
     url='https://github.com/timhawker/pwforecast',
     long_description_content_type='text/markdown',
     long_description=readme,
     packages=['pwforecast'],
     install_requires=['tzlocal', 'requests', 'python-dateutil', 'TeslaPy']
```

