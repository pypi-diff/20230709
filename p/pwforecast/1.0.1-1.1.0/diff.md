# Comparing `tmp/pwforecast-1.0.1.tar.gz` & `tmp/pwforecast-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwforecast-1.0.1.tar", last modified: Sat Jul  8 22:53:50 2023, max compression
+gzip compressed data, was "pwforecast-1.1.0.tar", last modified: Sun Jul  9 02:40:10 2023, max compression
```

## Comparing `pwforecast-1.0.1.tar` & `pwforecast-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:50.978203 pwforecast-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-08 22:53:41.000000 pwforecast-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-08 22:53:50.978203 pwforecast-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-08 22:53:41.000000 pwforecast-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:50.978203 pwforecast-1.0.1/pwforecast/
--rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-07-08 22:53:41.000000 pwforecast-1.0.1/pwforecast/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:53:50.978203 pwforecast-1.0.1/pwforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-08 22:53:50.000000 pwforecast-1.0.1/pwforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-08 22:53:50.000000 pwforecast-1.0.1/pwforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:53:50.000000 pwforecast-1.0.1/pwforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-08 22:53:50.000000 pwforecast-1.0.1/pwforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 22:53:50.000000 pwforecast-1.0.1/pwforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 22:53:50.978203 pwforecast-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-08 22:53:41.000000 pwforecast-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:40:10.443442 pwforecast-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-09 02:39:57.000000 pwforecast-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-09 02:40:10.443442 pwforecast-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-09 02:39:57.000000 pwforecast-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:40:10.443442 pwforecast-1.1.0/pwforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-07-09 02:39:57.000000 pwforecast-1.1.0/pwforecast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:40:10.443442 pwforecast-1.1.0/pwforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-09 02:40:10.000000 pwforecast-1.1.0/pwforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-09 02:40:10.000000 pwforecast-1.1.0/pwforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 02:40:10.000000 pwforecast-1.1.0/pwforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-09 02:40:10.000000 pwforecast-1.1.0/pwforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 02:40:10.000000 pwforecast-1.1.0/pwforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 02:40:10.443442 pwforecast-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-09 02:39:57.000000 pwforecast-1.1.0/setup.py
```

### Comparing `pwforecast-1.0.1/LICENSE` & `pwforecast-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pwforecast-1.0.1/PKG-INFO` & `pwforecast-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwforecast
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.
 Home-page: https://github.com/timhawker/pwforecast
 Author: Tim Hawker
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PwForecast
@@ -23,16 +23,16 @@
 
 PwForecast requires a Solcast API key and Site ID. You can sign up for a 
 [free Hobbyist account](https://toolkit.solcast.com.au/register) which allows up to two sites and 50 API calls per day. 
 
 [TeslaPy](https://tesla-api.timdorr.com/) has great documentation on getting started. It even works with two-factor
 authentication enabled.
 
-Rather than wrap [TeslaPy](https://tesla-api.timdorr.com/), PwForecast requires an instance of a Tesla class passed to 
-it. This allows you to configure the object based on your credentials before passing to PwForecast.  
+Rather than inherit [TeslaPy](https://tesla-api.timdorr.com/), PwForecast requires an instance of a Tesla class passed 
+to it. This allows you to configure the object based on your credentials before passing to PwForecast.  
 
 When using PwForecast, Self Powered mode is recommended. Time Based Control could be used if you need to charge
 faster than 1.7kW per Powerwall, but results may be unpredictable. 
 
 
 ## Overview 
 
@@ -54,15 +54,14 @@
 
     pw_forecast = PwForecast(teslapy_session=tesla,
                              solcast_api_key=solcast_api_key,
                              solcast_site_ids=solcast_site_ids)
 ```
 
 
-
 ## Setting Peak Mode
 
 Use this method when your peak rate starts. You can configure what backup reserve the Powerwall can discharge down
 to by setting the `min_reserve_peak_rate` value.
 
 ```python
 pw_forecast.min_reserve_peak_rate = 10  # Default 20
@@ -80,18 +79,22 @@
 Powerwall state of health: 95.0%
 -----------------------------------
 ```
 
 
 ## Setting Off-Peak Mode
 
-Use this method when your off-peak rate starts. This requires a little more configuration.
- * Configure what backup reserve the Powerwall can discharge down to by setting the 'min_reserve_off_peak_rate' attribute.
- * Configure the maximum backup reserve allowed by setting the 'max_reserve' attribute. 
- * Configure the amount of energy you require during the peak-rate.
+Use this method when your off-peak rate starts. This requires a little more setup.
+ * Configure what backup reserve the Powerwall can discharge down to by setting the `min_reserve_off_peak_rate` attribute.
+ * Configure the maximum backup reserve allowed by setting the `max_reserve` attribute. 
+ * Configure the amount of energy you require during the peak-rate by setting the `required_energy_peak_rate` attribute.
+
+When setting peak mode, PwForecast will determine how much solar will be generated tomorrow. It will then calculate how 
+much to fill the batteries based on the remaining energy requirement that solar will not satisfy. If solar generation
+completely satisfies `required_energy_peak_rate`, the backup reserve will be set to `min_reserve_off_peak_rate`. 
 
 ```python
 pw_forecast.min_reserve_off_peak_rate = 25  # Default 30
 pw_forecast.max_reserve = 95  # Default 100
 pw_forecast.required_energy_peak_rate = 20000  # Default 30000
 pw_forecast.set_off_peak_mode()
 ```
@@ -113,20 +116,24 @@
 
 When setting backup reserve, it is common to take two or three attempts before power flow changes to the expected 
 figures. As the Tesla API is unofficial, it is difficult to determine why. Waiting longer does not seem to fix this 
 issue, although waiting upwards of 45 minutes does sometimes result in power flow eventually changing correctly. 
 Re-applying the setting does appear to fix this issue. Perhaps the unofficial Tesla API is missing a commit command. 
 Please do let me know if you have any ideas. 
 
-Calling `set_peak_mode` and `set_off_peak_mode` will set the backup reserve, wait 20 seconds, and then check site power 
-flow to confirm the setting has been applied. If an incorrect power flow is detected, the method will retry up to the 
-`reserve_retry` limit. If the `retry_limit` is reached, an exception will be raised. PwForecast will then attempt to 
-apply the setting up to the `global_retry` limit, eventually raising an exception. 
+Calling `set_peak_mode` and `set_off_peak_mode` will set the backup reserve, wait 20 seconds, and then check site 
+power flow to confirm the setting has been applied. If an incorrect power flow is detected, the method will retry 
+up to the `set_backup_reserve_retry_limit` limit. If the `set_backup_reserve_retry_limit` is reached, an exception 
+will be raised and caught by the global retry logic. PwForecast will then attempt to re-apply the setting up to the 
+`global_retry_limit` limit, eventually raising an exception. 
+
+Both `set_backup_reserve_retry_limit` and `global_retry_limit` can be configured on the PwForecast instance. The 
+`set_backup_reserve_retry_limit` has been split from the `global_retry_limit` to try and avoid exhausting Solcast API calls. 
 
-Both `reserve_retry` and `global_retry` can be configured on the PwForecast instance. The `reserve_retry` has been 
-split from the `global_retry` to try and avoid exhausting Solcast API calls. 
+The amount of time between each `global_retry` can be configured via `global_retry_sleep`. The amount of time 
+between each `set_backup_reserve_retry_limit` can be configured via `set_backup_reserve_response_sleep`.
 
 
 ## Advanced Configuration
 
 PwForecast has a few advanced configuration options. Please check the class docstring for more info.
```

### Comparing `pwforecast-1.0.1/README.md` & `pwforecast-1.1.0/pwforecast.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: pwforecast
+Version: 1.1.0
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
@@ -14,16 +23,16 @@
 
 PwForecast requires a Solcast API key and Site ID. You can sign up for a 
 [free Hobbyist account](https://toolkit.solcast.com.au/register) which allows up to two sites and 50 API calls per day. 
 
 [TeslaPy](https://tesla-api.timdorr.com/) has great documentation on getting started. It even works with two-factor
 authentication enabled.
 
-Rather than wrap [TeslaPy](https://tesla-api.timdorr.com/), PwForecast requires an instance of a Tesla class passed to 
-it. This allows you to configure the object based on your credentials before passing to PwForecast.  
+Rather than inherit [TeslaPy](https://tesla-api.timdorr.com/), PwForecast requires an instance of a Tesla class passed 
+to it. This allows you to configure the object based on your credentials before passing to PwForecast.  
 
 When using PwForecast, Self Powered mode is recommended. Time Based Control could be used if you need to charge
 faster than 1.7kW per Powerwall, but results may be unpredictable. 
 
 
 ## Overview 
 
@@ -45,15 +54,14 @@
 
     pw_forecast = PwForecast(teslapy_session=tesla,
                              solcast_api_key=solcast_api_key,
                              solcast_site_ids=solcast_site_ids)
 ```
 
 
-
 ## Setting Peak Mode
 
 Use this method when your peak rate starts. You can configure what backup reserve the Powerwall can discharge down
 to by setting the `min_reserve_peak_rate` value.
 
 ```python
 pw_forecast.min_reserve_peak_rate = 10  # Default 20
@@ -71,18 +79,22 @@
 Powerwall state of health: 95.0%
 -----------------------------------
 ```
 
 
 ## Setting Off-Peak Mode
 
-Use this method when your off-peak rate starts. This requires a little more configuration.
- * Configure what backup reserve the Powerwall can discharge down to by setting the 'min_reserve_off_peak_rate' attribute.
- * Configure the maximum backup reserve allowed by setting the 'max_reserve' attribute. 
- * Configure the amount of energy you require during the peak-rate.
+Use this method when your off-peak rate starts. This requires a little more setup.
+ * Configure what backup reserve the Powerwall can discharge down to by setting the `min_reserve_off_peak_rate` attribute.
+ * Configure the maximum backup reserve allowed by setting the `max_reserve` attribute. 
+ * Configure the amount of energy you require during the peak-rate by setting the `required_energy_peak_rate` attribute.
+
+When setting peak mode, PwForecast will determine how much solar will be generated tomorrow. It will then calculate how 
+much to fill the batteries based on the remaining energy requirement that solar will not satisfy. If solar generation
+completely satisfies `required_energy_peak_rate`, the backup reserve will be set to `min_reserve_off_peak_rate`. 
 
 ```python
 pw_forecast.min_reserve_off_peak_rate = 25  # Default 30
 pw_forecast.max_reserve = 95  # Default 100
 pw_forecast.required_energy_peak_rate = 20000  # Default 30000
 pw_forecast.set_off_peak_mode()
 ```
@@ -104,20 +116,24 @@
 
 When setting backup reserve, it is common to take two or three attempts before power flow changes to the expected 
 figures. As the Tesla API is unofficial, it is difficult to determine why. Waiting longer does not seem to fix this 
 issue, although waiting upwards of 45 minutes does sometimes result in power flow eventually changing correctly. 
 Re-applying the setting does appear to fix this issue. Perhaps the unofficial Tesla API is missing a commit command. 
 Please do let me know if you have any ideas. 
 
-Calling `set_peak_mode` and `set_off_peak_mode` will set the backup reserve, wait 20 seconds, and then check site power 
-flow to confirm the setting has been applied. If an incorrect power flow is detected, the method will retry up to the 
-`reserve_retry` limit. If the `retry_limit` is reached, an exception will be raised. PwForecast will then attempt to 
-apply the setting up to the `global_retry` limit, eventually raising an exception. 
+Calling `set_peak_mode` and `set_off_peak_mode` will set the backup reserve, wait 20 seconds, and then check site 
+power flow to confirm the setting has been applied. If an incorrect power flow is detected, the method will retry 
+up to the `set_backup_reserve_retry_limit` limit. If the `set_backup_reserve_retry_limit` is reached, an exception 
+will be raised and caught by the global retry logic. PwForecast will then attempt to re-apply the setting up to the 
+`global_retry_limit` limit, eventually raising an exception. 
+
+Both `set_backup_reserve_retry_limit` and `global_retry_limit` can be configured on the PwForecast instance. The 
+`set_backup_reserve_retry_limit` has been split from the `global_retry_limit` to try and avoid exhausting Solcast API calls. 
 
-Both `reserve_retry` and `global_retry` can be configured on the PwForecast instance. The `reserve_retry` has been 
-split from the `global_retry` to try and avoid exhausting Solcast API calls. 
+The amount of time between each `global_retry` can be configured via `global_retry_sleep`. The amount of time 
+between each `set_backup_reserve_retry_limit` can be configured via `set_backup_reserve_response_sleep`.
 
 
 ## Advanced Configuration
 
 PwForecast has a few advanced configuration options. Please check the class docstring for more info.
```

### Comparing `pwforecast-1.0.1/pwforecast/__init__.py` & `pwforecast-1.1.0/pwforecast/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,65 +9,70 @@
 # TODO: Calculate required energy by looking at average historic usage during peak-rate between certain time period.
 
 
 class PwForecast(object):
     """
     A tool that dynamically sets Powerwall backup reserve percent based on solar forecast.
 
-    PwForecast is useful if you have a day/night rate, and the night rate is long enough to
-    charge the batteries.
+    PwForecast is useful if you have a day/night rate, and the night rate is long enough
+    to charge the batteries.
 
     PwForecast has primarily been designed for use with 'Self Consumption' mode, although
     it can be used in 'Time Based Control' mode with unpredictable results.
 
     A Solcast API Key and at least one Site ID will be needed.
 
     Args:
         teslapy_session (teslapy.Tesla): The tesla session object.
         solcast_api_key (str): The Solcast API Key.
-        solcast_site_ids (dict): A dict of Solcast site ID's, where key is the site name and
-            value is the site ID.
+        solcast_site_ids (dict): A dict of Solcast site ID's, where key is the site name
+            and value is the site ID.
 
     Attributes:
-        min_reserve_peak_rate (int): The minimum backup reserve to be set when in peak grid rates.
-            Default 20.
-        min_reserve_off_peak_rate (int): The minimum backup reserve that can be set when in off-peak
-            grid rates. Default 30.
-        max_reserve (int): The maximum backup reserve that can be set. If you don't like charging
-            your batteries to 100%, you can set this value. Default 100.
-        timezone (datetime.tzinfo): The tzdata timezone the system sits within. Will use timezone
-            from system by default.
-        required_energy_peak_rate (int): The amount of energy required during peak rate in Wh. When
-            setting peak mode, PwForecast will determine how much solar will be generated. It
-            will then calculate how much to fill the batteries based on the remaining energy
-            requirement. Default 30000.
-        global_retry (int): The number of times the set function should try before failing. This
-            is useful if there is a temporary service outage. Be careful setting this value too
-            high as solcast has a limited number of
-        reserve_retry (int): The number of retries to make when setting reserve percent. A failure
-            is defined as an unsuccessful switch transition by monitoring the power flow, even if
-            the tesla API returns success.
-        retry_sleep (int): The time in seconds to sleep before retrying if an error occurs.
-            Default 20.
-        wait_for_response_sleep (int): The time in seconds to sleep before testing the current
-            site power flow. This is useful as the Powerwall sometimes takes time to respond to
-            requests. Default 20.
-        reserve_switch_margin (int): The minimum number of watts to satisfy a successful backup
-            reserve power flow transition (e.g. from discharging to charging). When setting the
-            backup reserve higher than the current charge, the battery needs to be importing more
-            than this value. When setting the backup reserve lower than the current charge, the
-            sum of battery+solar needs to be producing more than this value. Default 100.
-        charge_margin (int): If the Powerwall current charge level is within this margin to the
-            value being set, the reserve_switch_margin is not monitored. This is necessary because
-            the Powerwall can have unexpected behaviour when setting percentages close to current
-            charge percentage. There have been cases where the Powerwall has started charging when
-            setting a backup reserve 0.7% less than current charge percentage, causing the reserve
-            switch checking logic to fail. Default 1.
-        full_pack_energy (int): The full pack energy in Wh of a brand new powerwall. This is used
-            to calculate the overall state of health of all batteries in the system. Default 14000.
+        min_reserve_peak_rate (int): The minimum backup reserve to be set when in peak
+            grid rates. Default 20.
+        min_reserve_off_peak_rate (int): The minimum backup reserve that can be set when
+            in off-peak grid rates. Default 30.
+        max_reserve (int): The maximum backup reserve that can be set. If you don't like
+            charging your batteries to 100%, you can set this value. Default 100.
+        timezone (datetime.tzinfo): The tzdata timezone the system sits within. Will use
+            timezone from system by default.
+        required_energy_peak_rate (int): The amount of energy required during peak rate
+            in Wh. When setting peak mode, PwForecast will determine how much solar will
+            be generated. It will then calculate how much to fill the batteries based on
+            the remaining energy requirement. Default 30000.
+        global_retry_limit (int): The number of times the set function should try before
+            failing. This is useful if there is a temporary service outage. Be careful
+            setting this value too high as solcast has a limited number of API calls.
+            Default 5
+        global_retry_sleep (int): The time in seconds to sleep before retrying if an
+            error occurs. Default 20.
+        set_backup_reserve_retry_limit (int): The number of retries to make when setting
+            reserve percent. A failure is defined as an unsuccessful switch transition
+            by monitoring the power flow, even if the tesla API returns success.
+            Default 5.
+        set_backup_reserve_response_sleep (int): The time in seconds to sleep before
+            testing the current site power flow. This is useful as the Powerwall
+            sometimes takes time to respond to requests. Default 20.
+        reserve_switch_margin (int): The minimum number of watts to satisfy a successful
+            backup reserve power flow transition (e.g. from discharging to charging).
+            When setting the backup reserve higher than the current charge, the battery
+            needs to be importing more than this value. When setting the backup reserve
+            lower than the current charge, the sum of battery+solar needs to be producing
+            more than this value. Default 100.
+        charge_margin (int): If the Powerwall current charge level is within this margin
+            to the value being set, the reserve_switch_margin is not monitored. This is
+            necessary because the Powerwall can have unexpected behaviour when setting
+            percentages close to current charge percentage. There have been cases where
+            the Powerwall has started charging when setting a backup reserve 0.7% less
+            than current charge percentage, causing the reserve switch checking logic to
+            fail. Default 1.
+        full_pack_energy (int): The full pack energy in Wh of a brand new powerwall. This
+            is used to calculate the overall state of health of all batteries in the
+            system. Default 14000.
 
     """
     def __init__(self, teslapy_session, solcast_api_key, solcast_site_ids):
 
         # internal vars
         self._teslapy_session = teslapy_session
         self._solcast_api_key = solcast_api_key
@@ -77,18 +82,18 @@
         self.min_reserve_peak_rate = 20
         self.min_reserve_off_peak_rate = 30
         self.max_reserve = 100
         self.required_energy_peak_rate = 30000
 
         # advanced configuration
         self.timezone = tzlocal.get_localzone()
-        self.global_retry = 5
-        self.reserve_retry = 5
-        self.retry_sleep = 30
-        self.wait_for_response_sleep = 20
+        self.global_retry_limit = 5
+        self.global_retry_sleep = 30
+        self.set_backup_reserve_retry_limit = 5
+        self.set_backup_reserve_response_sleep = 20
         self.reserve_switch_margin = 100
         self.charge_margin = 1
         self.full_pack_energy = 14000
 
     # solcast
     def get_solar_forecast_tomorrow(self):
         """
@@ -104,15 +109,18 @@
         total_energy_kwh = 0.0
         for solcast_site_name, solcast_site_id in self._solcast_site_ids.items():
             result = requests.get(url.format(site_id=solcast_site_id,
                                              api_key=self._solcast_api_key)).json()
 
             # get tomorrow start and end dates
             now = datetime.datetime.now(tz=self.timezone)
-            today_start = datetime.datetime(year=now.year, month=now.month, day=now.day, tzinfo=self.timezone)
+            today_start = datetime.datetime(year=now.year,
+                                            month=now.month,
+                                            day=now.day,
+                                            tzinfo=self.timezone)
             tomorrow_start = today_start + datetime.timedelta(days=1)
             tomorrow_end = today_start + datetime.timedelta(days=2)
 
             # get forecast blocks for each time period within sunrise and sunset tomorrow
             forecast_blocks = []
             for forecast_block in result['forecasts']:
                 forecast_time = parser.parse(forecast_block['period_end'])
@@ -164,85 +172,93 @@
 
     def set_backup_reserve_percent(self, percent_target):
         """
         Sets the provided backup reserve percent. If an invalid state is detected after
         setting the reserve percent, the function will retry up to a max number of times
         defined by module level settings.
 
-        An invalid state is defined as charging when it should be discharging, and discharging
-        when it should be charging. This seems to happen often, and simply sending the command
-        again tends to fix the issue.
+        An invalid state is defined as charging when it should be discharging, and
+        discharging when it should be charging. This seems to happen often, and simply
+        sending the command again tends to fix the issue.
 
         Args:
             percent_target (int): The percent target to set as backup reserve.
 
         Returns:
             dict: A dictionary containing site status information.
 
         Raises:
-            Exception: If an invalid charge state is detected and the retry limit has been
-                reached.
+            Exception: If an invalid charge state is detected and the retry limit has
+                been reached.
 
         """
         # cast to int in case a float is provided
         percent_target = int(percent_target)
 
         # get the battery, which is a class representing the site
         battery_list = self._teslapy_session.battery_list()
         assert len(battery_list) == 1, 'More than one battery list returned!'
         battery = battery_list[0]
 
         # loop to allow reserve retries
-        for index in range(1, self.reserve_retry+1):
+        for index in range(1, self.set_backup_reserve_retry_limit+1):
 
             # set the battery reserve
-            print('Setting backup reserve to {}%, attempt {} of {}'.format(percent_target, index, self.reserve_retry))
+            print('Setting backup reserve to {}%, attempt {} of {}'.format(
+                percent_target, index, self.set_backup_reserve_retry_limit))
             battery.set_backup_reserve_percent(percent_target)
 
             # sleep to let the devices update and api sync
-            time.sleep(self.wait_for_response_sleep)
+            time.sleep(self.set_backup_reserve_response_sleep)
 
             # check to see if the battery charge/discharge state has correctly changed
             battery_data = battery.get_battery_data()
             msg = 'More than one power reading returned!'
             assert len(battery_data['power_reading']) == 1, msg
             total_pack_energy = battery_data['total_pack_energy']
             battery_count = battery_data['battery_count']
             assert battery_count > 0, 'No batteries detected!'
             pack_soh = (100 / (self.full_pack_energy * battery_count)) * total_pack_energy
             percent_charged = battery_data['percentage_charged']
             power_reading = battery_data['power_reading'][0]
             battery_power = power_reading['battery_power']
             solar_power = power_reading['solar_power']
 
-            # battery within charge margin, set reserve percent and don't check power flow as it can lead to
-            # false positives.
+            # battery within charge margin, set reserve percent and don't check power
+            # flow as it can lead to false positives.
             if percent_target-self.charge_margin <= percent_charged <= percent_target+self.charge_margin:
                 print('Battery charge within target reserve margin')
-                # although the setting is eventually applied, it seems to not change for up to a few hours, and the
-                # powerwall can continue draining until it has hit the previous reserve setting. If this is the first
-                # iteration, loop again to try and avoid this behaviour.
+                # although the setting is eventually applied, it seems to not change for
+                # up to a few hours, and the powerwall can continue draining until it has
+                # hit the previous reserve setting. If this is the first iteration, loop
+                # again to try and avoid this behaviour.
                 if index < 2:
-                    print('Reapplying setting to try and ensure powerwall power flow behaves as expected.')
+                    msg = ('Reapplying setting to try and ensure powerwall power flow '
+                           'behaves as expected.')
+                    print(msg)
                 else:
                     break
 
             # battery should be charging
             elif percent_target > percent_charged and battery_power < -self.reserve_switch_margin:
                 print('Battery charging at {:.1f}w'.format(battery_power))
                 break
 
-            # battery should be discharging, or battery in standby mode and solar providing power
+            # battery should be discharging, or battery in standby mode and solar
+            # providing power
             elif percent_target < percent_charged and battery_power+solar_power > self.reserve_switch_margin:
                 print('Battery discharging at {:.1f}w'.format(battery_power))
-                # although the setting is eventually applied, it seems to not change for up to a few hours, and the
-                # powerwall can continue draining until it has hit the previous reserve setting. If this is the first
-                # iteration, loop again to try and avoid this behaviour.
+                # although the setting is eventually applied, it seems to not change for
+                # up to a few hours, and the powerwall can continue draining until it has
+                # hit the previous reserve setting. If this is the first iteration, loop
+                # again to try and avoid this behaviour.
                 if index < 2:
-                    print('Reapplying setting to try and ensure powerwall will stop discharging at set reserve.')
+                    msg = ('Reapplying setting to try and ensure powerwall will stop '
+                           'discharging at set reserve.')
+                    print(msg)
                 else:
                     break
 
             else:
                 print('Incorrect charge/discharge state')
                 pprint.pprint(power_reading)
 
@@ -255,70 +271,73 @@
                 'reserve': percent_target,
                 'capacity': total_pack_energy,
                 'soh': pack_soh}
 
     # public
     def set_peak_mode(self):
         """
-        Sets backup reserve to 'min_reserve_peak_rate'. Used when transitioning to peak rates.
+        Sets backup reserve to 'min_reserve_peak_rate'. Used when transitioning to peak
+        rates.
 
-        Attempts to set mode multiple times if an error occurs up to the 'global_retry' limit.
+        Attempts to set mode multiple times if an error occurs up to the
+        value set in the 'global_retry_limit' attribute.
 
         Raises:
-            Exception: If an invalid charge state is detected and the retry limit has been
-                reached.
+            Exception: If an invalid charge state is detected and the retry limit has
+                been reached.
 
         """
-        for i in range(1, self.global_retry + 1):
+        for i in range(1, self.global_retry_limit + 1):
             try:
                 # status update
                 msg = 'Setting peak mode, attempt {i} of {total}'
-                print(msg.format(i=i, total=self.global_retry))
+                print(msg.format(i=i, total=self.global_retry_limit))
                 # set the peak reserve
                 status = self.set_backup_reserve_percent(self.min_reserve_peak_rate)
                 self._print_summary(**status)
             except Exception as e:
-                if i == self.global_retry:
+                if i == self.global_retry_limit:
                     raise
                 msg = '{c}: {e}'
                 print(msg.format(c=e.__class__.__name__, e=e))
                 # sleep in case of temporary outage
-                time.sleep(self.retry_sleep)
+                time.sleep(self.global_retry_sleep)
             else:
                 break
 
     def set_off_peak_mode(self):
         """
-        Sets backup reserve based on solar forecast tomorrow. The backup reserve will be set between
-        'min_reserve_off_peak_rate' and 'max_reserve'. Used when transitioning to off-peak rates.
+        Sets backup reserve based on solar forecast tomorrow. The backup reserve will be
+        set between 'min_reserve_off_peak_rate' and 'max_reserve'. Used when
+        transitioning to off-peak rates.
 
         Raises:
-            Exception: If an invalid charge state is detected and the retry limit has been
-                reached.
+            Exception: If an invalid charge state is detected and the retry limit has
+            been reached.
 
         """
-        for i in range(1, self.global_retry + 1):
+        for i in range(1, self.global_retry_limit + 1):
             try:
                 # status update
                 msg = 'Setting off-peak mode, attempt {i} of {total}'
-                print(msg.format(i=i, total=self.global_retry))
+                print(msg.format(i=i, total=self.global_retry_limit))
                 # get the off-peak reserve
                 forecast_tomorrow = self.get_solar_forecast_tomorrow()
                 charge_percent = self.calculate_backup_reserve(forecast_tomorrow)
                 # set the off-peak reserve
                 status = self.set_backup_reserve_percent(charge_percent)
                 status['solar_forecast'] = forecast_tomorrow
                 self._print_summary(**status)
             except Exception as e:
-                if i == self.global_retry:
+                if i == self.global_retry_limit:
                     raise
                 msg = '{c}: {e}'
                 print(msg.format(c=e.__class__.__name__, e=e))
                 # sleep in case of temporary outage
-                time.sleep(self.retry_sleep)
+                time.sleep(self.global_retry_sleep)
             else:
                 break
 
     # internal
     def _print_summary(self, soc, reserve, capacity, soh, solar_forecast=None):
         """
         Prints a status summary of the tesla site, including optional solar forecast.
```

### Comparing `pwforecast-1.0.1/pwforecast.egg-info/PKG-INFO` & `pwforecast-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: pwforecast
-Version: 1.0.1
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
@@ -23,16 +14,16 @@
 
 PwForecast requires a Solcast API key and Site ID. You can sign up for a 
 [free Hobbyist account](https://toolkit.solcast.com.au/register) which allows up to two sites and 50 API calls per day. 
 
 [TeslaPy](https://tesla-api.timdorr.com/) has great documentation on getting started. It even works with two-factor
 authentication enabled.
 
-Rather than wrap [TeslaPy](https://tesla-api.timdorr.com/), PwForecast requires an instance of a Tesla class passed to 
-it. This allows you to configure the object based on your credentials before passing to PwForecast.  
+Rather than inherit [TeslaPy](https://tesla-api.timdorr.com/), PwForecast requires an instance of a Tesla class passed 
+to it. This allows you to configure the object based on your credentials before passing to PwForecast.  
 
 When using PwForecast, Self Powered mode is recommended. Time Based Control could be used if you need to charge
 faster than 1.7kW per Powerwall, but results may be unpredictable. 
 
 
 ## Overview 
 
@@ -54,15 +45,14 @@
 
     pw_forecast = PwForecast(teslapy_session=tesla,
                              solcast_api_key=solcast_api_key,
                              solcast_site_ids=solcast_site_ids)
 ```
 
 
-
 ## Setting Peak Mode
 
 Use this method when your peak rate starts. You can configure what backup reserve the Powerwall can discharge down
 to by setting the `min_reserve_peak_rate` value.
 
 ```python
 pw_forecast.min_reserve_peak_rate = 10  # Default 20
@@ -80,18 +70,22 @@
 Powerwall state of health: 95.0%
 -----------------------------------
 ```
 
 
 ## Setting Off-Peak Mode
 
-Use this method when your off-peak rate starts. This requires a little more configuration.
- * Configure what backup reserve the Powerwall can discharge down to by setting the 'min_reserve_off_peak_rate' attribute.
- * Configure the maximum backup reserve allowed by setting the 'max_reserve' attribute. 
- * Configure the amount of energy you require during the peak-rate.
+Use this method when your off-peak rate starts. This requires a little more setup.
+ * Configure what backup reserve the Powerwall can discharge down to by setting the `min_reserve_off_peak_rate` attribute.
+ * Configure the maximum backup reserve allowed by setting the `max_reserve` attribute. 
+ * Configure the amount of energy you require during the peak-rate by setting the `required_energy_peak_rate` attribute.
+
+When setting peak mode, PwForecast will determine how much solar will be generated tomorrow. It will then calculate how 
+much to fill the batteries based on the remaining energy requirement that solar will not satisfy. If solar generation
+completely satisfies `required_energy_peak_rate`, the backup reserve will be set to `min_reserve_off_peak_rate`. 
 
 ```python
 pw_forecast.min_reserve_off_peak_rate = 25  # Default 30
 pw_forecast.max_reserve = 95  # Default 100
 pw_forecast.required_energy_peak_rate = 20000  # Default 30000
 pw_forecast.set_off_peak_mode()
 ```
@@ -113,20 +107,24 @@
 
 When setting backup reserve, it is common to take two or three attempts before power flow changes to the expected 
 figures. As the Tesla API is unofficial, it is difficult to determine why. Waiting longer does not seem to fix this 
 issue, although waiting upwards of 45 minutes does sometimes result in power flow eventually changing correctly. 
 Re-applying the setting does appear to fix this issue. Perhaps the unofficial Tesla API is missing a commit command. 
 Please do let me know if you have any ideas. 
 
-Calling `set_peak_mode` and `set_off_peak_mode` will set the backup reserve, wait 20 seconds, and then check site power 
-flow to confirm the setting has been applied. If an incorrect power flow is detected, the method will retry up to the 
-`reserve_retry` limit. If the `retry_limit` is reached, an exception will be raised. PwForecast will then attempt to 
-apply the setting up to the `global_retry` limit, eventually raising an exception. 
+Calling `set_peak_mode` and `set_off_peak_mode` will set the backup reserve, wait 20 seconds, and then check site 
+power flow to confirm the setting has been applied. If an incorrect power flow is detected, the method will retry 
+up to the `set_backup_reserve_retry_limit` limit. If the `set_backup_reserve_retry_limit` is reached, an exception 
+will be raised and caught by the global retry logic. PwForecast will then attempt to re-apply the setting up to the 
+`global_retry_limit` limit, eventually raising an exception. 
+
+Both `set_backup_reserve_retry_limit` and `global_retry_limit` can be configured on the PwForecast instance. The 
+`set_backup_reserve_retry_limit` has been split from the `global_retry_limit` to try and avoid exhausting Solcast API calls. 
 
-Both `reserve_retry` and `global_retry` can be configured on the PwForecast instance. The `reserve_retry` has been 
-split from the `global_retry` to try and avoid exhausting Solcast API calls. 
+The amount of time between each `global_retry` can be configured via `global_retry_sleep`. The amount of time 
+between each `set_backup_reserve_retry_limit` can be configured via `set_backup_reserve_response_sleep`.
 
 
 ## Advanced Configuration
 
 PwForecast has a few advanced configuration options. Please check the class docstring for more info.
```

### Comparing `pwforecast-1.0.1/setup.py` & `pwforecast-1.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 
 # read the contents of README file
 readme = (this_directory / 'README.md').read_text()
 
 setuptools.setup(
     name='pwforecast',
-    version='1.0.1',
+    version='1.1.0',
     author='Tim Hawker',
     description='A Python module to charge/discharge Powerwall based on solar forecast and peak/off peak tariffs.',
     url='https://github.com/timhawker/pwforecast',
     long_description_content_type='text/markdown',
     long_description=readme,
     packages=['pwforecast'],
     install_requires=['tzlocal', 'requests', 'python-dateutil', 'TeslaPy']
```

