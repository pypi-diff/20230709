# Comparing `tmp/tripplite-0.3.0.tar.gz` & `tmp/tripplite-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tripplite-0.3.0.tar", last modified: Thu Oct  1 16:06:00 2020, max compression
+gzip compressed data, was "tripplite-0.4.0.tar", last modified: Sun Jul  9 01:07:51 2023, max compression
```

## Comparing `tripplite-0.3.0.tar` & `tripplite-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 pat        (502) staff       (20)        0 2020-10-01 16:06:00.000000 tripplite-0.3.0/
--rw-r--r--   0 pat        (502) staff       (20)     6738 2020-10-01 16:06:00.000000 tripplite-0.3.0/PKG-INFO
--rw-r--r--   0 pat        (502) staff       (20)     4890 2020-10-01 15:46:11.000000 tripplite-0.3.0/README.md
--rw-r--r--   0 pat        (502) staff       (20)      112 2020-10-01 16:06:00.000000 tripplite-0.3.0/setup.cfg
--rw-r--r--   0 pat        (502) staff       (20)     1045 2020-10-01 16:02:40.000000 tripplite-0.3.0/setup.py
-drwxr-xr-x   0 pat        (502) staff       (20)        0 2020-10-01 16:06:00.000000 tripplite-0.3.0/tripplite/
--rw-r--r--   0 pat        (502) staff       (20)     1791 2020-10-01 16:04:26.000000 tripplite-0.3.0/tripplite/__init__.py
--rw-r--r--   0 pat        (502) staff       (20)     1182 2020-10-01 15:46:11.000000 tripplite-0.3.0/tripplite/collectors.py
--rw-r--r--   0 pat        (502) staff       (20)     4321 2020-04-22 20:52:05.000000 tripplite-0.3.0/tripplite/driver.py
--rw-r--r--   0 pat        (502) staff       (20)     2453 2020-10-01 15:46:11.000000 tripplite-0.3.0/tripplite/prometheus.py
-drwxr-xr-x   0 pat        (502) staff       (20)        0 2020-10-01 16:06:00.000000 tripplite-0.3.0/tripplite.egg-info/
--rw-r--r--   0 pat        (502) staff       (20)     6738 2020-10-01 16:06:00.000000 tripplite-0.3.0/tripplite.egg-info/PKG-INFO
--rw-r--r--   0 pat        (502) staff       (20)      318 2020-10-01 16:06:00.000000 tripplite-0.3.0/tripplite.egg-info/SOURCES.txt
--rw-r--r--   0 pat        (502) staff       (20)        1 2020-10-01 16:06:00.000000 tripplite-0.3.0/tripplite.egg-info/dependency_links.txt
--rw-r--r--   0 pat        (502) staff       (20)       54 2020-10-01 16:06:00.000000 tripplite-0.3.0/tripplite.egg-info/entry_points.txt
--rw-r--r--   0 pat        (502) staff       (20)       37 2020-10-01 16:06:00.000000 tripplite-0.3.0/tripplite.egg-info/requires.txt
--rw-r--r--   0 pat        (502) staff       (20)       10 2020-10-01 16:06:00.000000 tripplite-0.3.0/tripplite.egg-info/top_level.txt
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-09 01:07:51.871478 tripplite-0.4.0/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18092 2023-07-09 00:45:17.000000 tripplite-0.4.0/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5427 2023-07-09 01:07:51.871589 tripplite-0.4.0/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     4814 2023-07-09 00:45:17.000000 tripplite-0.4.0/README.md
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       89 2023-07-09 01:07:51.871905 tripplite-0.4.0/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1090 2023-07-09 01:05:53.000000 tripplite-0.4.0/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-09 01:07:51.870522 tripplite-0.4.0/tripplite/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1790 2023-07-09 00:55:29.000000 tripplite-0.4.0/tripplite/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1460 2023-07-09 00:54:09.000000 tripplite-0.4.0/tripplite/collectors.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     4345 2023-07-09 00:55:29.000000 tripplite-0.4.0/tripplite/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2639 2023-07-09 01:00:07.000000 tripplite-0.4.0/tripplite/prometheus.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-09 01:07:51.871343 tripplite-0.4.0/tripplite.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5427 2023-07-09 01:07:51.000000 tripplite-0.4.0/tripplite.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      326 2023-07-09 01:07:51.000000 tripplite-0.4.0/tripplite.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-07-09 01:07:51.000000 tripplite-0.4.0/tripplite.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       53 2023-07-09 01:07:51.000000 tripplite-0.4.0/tripplite.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       50 2023-07-09 01:07:51.000000 tripplite-0.4.0/tripplite.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       10 2023-07-09 01:07:51.000000 tripplite-0.4.0/tripplite.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tripplite-0.3.0/PKG-INFO` & `tripplite-0.4.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,173 +1,159 @@
-Metadata-Version: 2.1
-Name: tripplite
-Version: 0.3.0
-Summary: Python driver for TrippLite UPS battery backups.
-Home-page: http://github.com/numat/tripplite/
-Author: Patrick Fuller
-Author-email: pat@numat-tech.com
-License: GPLv2
-Description: # tripplite
-        
-        Python USB interface and command-line tool for TrippLite UPS battery backups.
-        
-        ![](https://www.markertek.com/productImage/450X450/SMART1500LCD.JPG)
-        
-        ## Background
-        
-        TrippLite offers [UI software](https://www.tripplite.com/products/power-alert)
-        for monitoring its batteries. However, most of its batteries don't have
-        network access, and the existing TrippLite software requires a local install.
-        
-        I wanted to monitor the UPS from a remote headless Linux server, so I wrote
-        this tool.
-        
-        ## Supported Hardware
-        
-        This has been exclusively tested on the TrippLite SMART1500LCD UPS. It will
-        likely work on similar firmware but there is a known communication issue with
-        some other TrippLite models (see [numat/tripplite#3](https://github.com/numat/tripplite/issues/3)).
-        
-        Use `lsusb` to check. `09ae:2012` should work, while `09ae:3016` may not.
-        
-        ## Installation
-        
-        ```console
-        apt install gcc libusb-1.0-0-dev libudev-dev
-        pip install tripplite
-        ```
-        
-        Connect a USB cable from the UPS to your headless server, and you should be
-        ready to run. If you don't want to run as root, see *Note on Permissions*
-        below.
-        
-        # Command Line
-        
-        ```json
-        $ tripplite
-        {
-            "config": {
-                "frequency": 60,  # Hz
-                "power": 1500,  # VA
-                "voltage": 120  # V
-            },
-            "health": 100,  # %
-            "input": {
-                "frequency": 59.7,  # Hz
-                "voltage": 117.2  # V
-            },
-            "output": {
-                "power": 324,  # W
-                "voltage": 117.2  # V
-            },
-            "status": {
-                "ac present": true,
-                "below remaining capacity": true,
-                "charging": false,
-                "discharging": false,
-                "fully charged": true,
-                "fully discharged": false,
-                "needs replacement": false,
-                "shutdown imminent": false
-            },
-            "time to empty": 1004  # s
-        }
-        ```
-        
-        To use in shell scripts, parse the json output with something like
-        [jq](https://stedolan.github.io/jq/). For example,
-        `tripplite | jq '.status."ac present"'` will return whether or not the unit
-        detects AC power.
-        
-        ## Python
-        
-        If you'd like to link this to more complex behavior (e.g. data logging,
-        text alerts), consider using a Python script.
-        
-        ```python
-        from tripplite import Battery
-        with Battery() as battery:
-            print(battery.get())
-        ```
-        
-        The `state` variable will contain an object with the same format as above. Use
-        `state['status']['ac present']` and `state['status']['shutdown imminent']` for
-        alerts, and consider logging voltage, frequency, and power.
-        
-        If you are logging multiple batteries, you will need to handle each connection
-        separately.
-        
-        ```python
-        from tripplite import Battery, battery_paths
-        for path in battery_paths:
-            with Battery(path) as battery:
-                print(battery.get())
-        ```
-        
-        These paths are unfortunately non-deterministic and will change on each
-        iteration. For long running processes please prefer to keep an open `Battery`
-        object and open + close on read errors. For example:
-        
-        ```python
-            def check_batteries(
-                self, battery_paths: List[str], check_period: float = 30.0
-            ) -> None:
-                """Read batteries and reopen in error"""
-                self.batteries = [Battery(path) for path in battery_paths]
-                for battery in self.batteries:
-                    battery.open()
-                while True:
-                    time.sleep(check_period)
-                    for state, battery in zip(self.state, self.batteries):
-                        try:
-                            state.update(battery.get())
-                        except OSError:
-                            logger.exception(f"Could not read battery {battery}.")
-                            battery.close()
-        ```
-        
-        ## Note on Permissions
-        
-        To read the TrippLite, you need access to the USB port. You have options:
-        
-        * Run everything as root
-        * Add your user to the `dialout` group to access *all* serial ports
-        * Create a group restricted to accessing TrippLite USB devices through `udev`
-        
-        For the last option, the rule looks like:
-        
-        ```console
-        echo 'SUBSYSTEM=="usb", ATTRS{idVendor}=="09ae", GROUP="tripplite"' > /etc/udev/rules.d/tripplite.rules
-        udevadm control --reload-rules
-        ```
-        
-        ## Prometheus Exporter
-        
-        This package offers an extra install to include a [Prometheus Exporter](https://prometheus.io/docs/instrumenting/exporters/)
-        which allows for data collection into a prometheus time series database. Esentially it's a small `HTTP` server that allows
-        Prometheus to *scrape* grabbing metrics at a configurable period.
-        
-        ### Install
-        
-        ```console
-        pip install tripplite[exporter]
-        ```
-        
-        * This adds the [prometheus_client](https://pypi.org/project/prometheus-client/) dependency.
-        
-        You can then manually run the `triplite-exporter` cli or use the
-        [tripplite_exporter.service](https://github.com/numat/tripplite/blob/master/tripplite_exporter.service)
-        systemd unit file to have systemd run and supervise the process.
-        
-        ### Failure Mode
-        
-        The script will try to close and reopen the USB serial connection to the device on an `OSError`. If an open fails,
-        the script will exit with the return code of 2.
-        
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Development Status :: 4 - Beta
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
-Description-Content-Type: text/markdown
-Provides-Extra: exporter
+# tripplite
+
+Python USB interface and command-line tool for TrippLite UPS battery backups.
+
+![](https://www.markertek.com/productImage/450X450/SMART1500LCD.JPG)
+
+## Background
+
+TrippLite offers [UI software](https://www.tripplite.com/products/power-alert)
+for monitoring its batteries. However, most of its batteries don't have
+network access, and the existing TrippLite software requires a local install.
+
+I wanted to monitor the UPS from a remote headless Linux server, so I wrote
+this tool.
+
+## Supported Hardware
+
+This has been exclusively tested on the TrippLite SMART1500LCD UPS. It will
+likely work on similar firmware but there is a known communication issue with
+some other TrippLite models (see [numat/tripplite#3](https://github.com/numat/tripplite/issues/3)).
+
+Use `lsusb` to check. `09ae:2012` should work, while `09ae:3016` may not.
+
+## Installation
+
+```console
+apt install gcc libusb-1.0-0-dev libudev-dev
+pip install tripplite
+```
+
+Connect a USB cable from the UPS to your headless server, and you should be
+ready to run. If you don't want to run as root, see *Note on Permissions*
+below.
+
+# Command Line
+
+```
+$ tripplite
+{
+    "config": {
+        "frequency": 60,  # Hz
+        "power": 1500,  # VA
+        "voltage": 120  # V
+    },
+    "health": 100,  # %
+    "input": {
+        "frequency": 59.7,  # Hz
+        "voltage": 117.2  # V
+    },
+    "output": {
+        "power": 324,  # W
+        "voltage": 117.2  # V
+    },
+    "status": {
+        "ac present": true,
+        "below remaining capacity": true,
+        "charging": false,
+        "discharging": false,
+        "fully charged": true,
+        "fully discharged": false,
+        "needs replacement": false,
+        "shutdown imminent": false
+    },
+    "time to empty": 1004  # s
+}
+```
+
+To use in shell scripts, parse the json output with something like
+[jq](https://stedolan.github.io/jq/). For example,
+`tripplite | jq '.status."ac present"'` will return whether or not the unit
+detects AC power.
+
+## Python
+
+If you'd like to link this to more complex behavior (e.g. data logging,
+text alerts), consider using a Python script.
+
+```python
+from tripplite import Battery
+with Battery() as battery:
+    print(battery.get())
+```
+
+The `state` variable will contain an object with the same format as above. Use
+`state['status']['ac present']` and `state['status']['shutdown imminent']` for
+alerts, and consider logging voltage, frequency, and power.
+
+If you are logging multiple batteries, you will need to handle each connection
+separately.
+
+```python
+from tripplite import Battery, battery_paths
+for path in battery_paths:
+    with Battery(path) as battery:
+        print(battery.get())
+```
+
+These paths are unfortunately non-deterministic and will change on each
+iteration.
+
+For long polling, you can improve stability by keeping connections open as long
+as possible and reconnecting on error. For example:
+
+```python
+state = None
+
+def read_batteries(check_period=5):
+    """Read battery and reopen in error. Use for long polling."""
+    battery = Battery()
+    battery.open()
+    while True:
+        time.sleep(check_period)
+        try:
+            state = battery.get()
+        except OSError:
+            logging.exception(f"Could not read battery {battery}.")
+            battery.close()
+            battery.open()
+```
+
+An example for multiple batteries can be found in [numat/tripplite#6](https://github.com/numat/tripplite/pull/6#issuecomment-700152340).
+
+## Note on Permissions
+
+To read the TrippLite, you need access to the USB port. You have options:
+
+* Run everything as root
+* Add your user to the `dialout` group to access *all* serial ports
+* Create a group restricted to accessing TrippLite USB devices through `udev`
+
+For the last option, the rule looks like:
+
+```console
+echo 'SUBSYSTEM=="usb", ATTRS{idVendor}=="09ae", GROUP="tripplite"' > /etc/udev/rules.d/tripplite.rules
+udevadm control --reload-rules
+```
+
+## Prometheus Exporter
+
+This package offers an extra install to include a [Prometheus Exporter](https://prometheus.io/docs/instrumenting/exporters/)
+which allows for data collection into a prometheus time series database. Esentially it's a small `HTTP` server that allows
+Prometheus to *scrape* grabbing metrics at a configurable period.
+
+### Install
+
+```console
+pip install tripplite[exporter]
+```
+
+* This adds the [prometheus_client](https://pypi.org/project/prometheus-client/) dependency.
+
+You can then manually run the `triplite-exporter` cli or use the
+[tripplite_exporter.service](https://github.com/numat/tripplite/blob/master/tripplite_exporter.service)
+systemd unit file to have systemd run and supervise the process.
+
+### Failure Mode
+
+The script will try to close and reopen the USB serial connection to the device on an `OSError`. If an open fails,
+the script will exit with the return code of 2.
```

### Comparing `tripplite-0.3.0/setup.py` & `tripplite-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """Package manager setup for TrippLite driver."""
 from setuptools import setup
 
-with open('README.md', 'r') as in_file:
+with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="tripplite",
-    version="0.3.0",
+    version="0.4.0",
     description="Python driver for TrippLite UPS battery backups.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url="http://github.com/numat/tripplite/",
+    url="https://github.com/numat/tripplite/",
     author="Patrick Fuller",
     author_email="pat@numat-tech.com",
     packages=['tripplite'],
     install_requires=['hidapi'],
     entry_points={
         'console_scripts': [
             'tripplite = tripplite:command_line',
         ],
     },
     extras_require={
-        "exporter": ["prometheus_client"],
+        'exporter': ['prometheus_client'],
+        'test': [
+            'ruff',
+        ],
     },
     license='GPLv2',
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Development Status :: 4 - Beta',
         'Natural Language :: English',
         'Programming Language :: Python',
```

### Comparing `tripplite-0.3.0/tripplite/__init__.py` & `tripplite-0.4.0/tripplite/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 """
 import argparse
 import logging
 import sys
 
 from tripplite.driver import Battery, battery_paths
 
-
 DEFAULT_PORT = 6969
 LOG = logging.getLogger(__name__)
 
 
 def _parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(description="Read TrippLite devices.")
     parser.add_argument(
@@ -41,15 +40,15 @@
     args = _parse_args()
     logging.basicConfig(
         format="[%(asctime)s] %(levelname)s: %(message)s (%(filename)s:%(lineno)d)",
         level=logging.DEBUG if args.debug else logging.INFO,
     )
 
     if not battery_paths:
-        raise IOError("No TrippLite devices found.")
+        raise OSError("No TrippLite devices found.")
 
     if args.exporter == "json":
         import json
         output = []
         for path in battery_paths:
             with Battery(path) as battery:
                 output.append(battery.get())
```

### Comparing `tripplite-0.3.0/tripplite/collectors.py` & `tripplite-0.4.0/tripplite/collectors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 #!/usr/bin/env python3
+"""Data collector for TripLite battery backups, used for Prometheus."""
 
 import logging
 from typing import Dict, Optional
 
 from tripplite.driver import Battery, battery_paths
 
-
 LOG = logging.getLogger(__name__)
 
 
 class Collector:
+    """Data collector to generate metrics."""
+
     battery: Optional[Battery] = None
     battery_path: str = ""
 
     def open_battery(self) -> None:
+        """Connect to a battery via USB."""
         if self.battery:
             return
 
         if not battery_paths:
             LOG.error("No Tripplite battery found")
             return None
 
         self.battery_path = battery_paths[0]
         self.battery = Battery(self.battery_path)
         self.battery.open()
         LOG.info(f"Connected to {self.battery_path} battery")
 
     def close_battery(self) -> None:
+        """Close the connection to the battery via USB."""
         self.battery.close()
         LOG.info(f"Disconnecting {self.battery_path} battery to try reconnect")
         self.battery = None
         self.battery_path = ""
 
     def get_data(self) -> Optional[Dict]:
+        """Get data from a battery connected via USB."""
         ups_data = None
         try:
             ups_data = self.battery.get()
         except OSError as ose:
             LOG.error(f"Unable to read from USB Serial for {self.battery_path}: {ose}")
             self.close_battery()
         return ups_data
```

### Comparing `tripplite-0.3.0/tripplite/driver.py` & `tripplite-0.4.0/tripplite/driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,28 +76,28 @@
         'address': 53,
         'bytes': 2,
         'format': 'i'
     }
 }
 
 
-class Battery(object):
+class Battery:
     """Driver for TrippLite UPS battery backups."""
 
     def __init__(self, path=None):
         """Connect to the device.
 
         Args:
             path (Optional): The HID path of the device. Only needed if
             reading multiple devices.
 
         """
         self.device = hid.device()
         if not battery_paths:
-            raise IOError("Could not find any connected TrippLite devices.")
+            raise OSError("Could not find any connected TrippLite devices.")
         if path is not None and path not in battery_paths:
             raise ValueError(f"Path {path} not in {', '.join(battery_paths)}.")
         self.path = path or battery_paths[0]
 
     def __enter__(self):
         """Provide entrance to context manager."""
         self.open()
@@ -114,14 +114,15 @@
     def close(self):
         """Close connection to the device."""
         self.device.close()
 
     def get(self):
         """Return an object containing all available data."""
         output = {}
+        output['device_id'] = self.path
         for category, data in structure.items():
             if 'address' in data:
                 output[category] = self._read(data)
             else:
                 output[category] = {}
                 for subcategory, options in data.items():
                     output[category][subcategory] = self._read(options)
@@ -135,19 +136,19 @@
         TrippLite communication interface manual for more.
         """
         report = self.device.get_feature_report(options['address'],
                                                 options['bytes'] + 1)
         if not report:
             if retries > 0:
                 return self._read(options, retries - 1)
-            raise IOError("Did not receive data.")
+            raise OSError("Did not receive data.")
         if options['address'] != report[0]:
-            raise IOError("Received unexpected data.")
+            raise OSError("Received unexpected data.")
         if options['format'] == 'b':
-            bits = '{:08b}'.format(report[1])[::-1]
+            bits = f'{report[1]:08b}'[::-1]
             return {k: bool(int(v)) for k, v in zip(options['keys'], bits)}
         elif options['format'] == 'i' and options['bytes'] == 2:
             return (report[2] << 8) + report[1]
         elif options['format'] == 'i' and options['bytes'] == 1:
             return report[1]
         elif options['format'] == 'f':
             return ((report[2] << 8) + report[1]) / 10.0
```

### Comparing `tripplite-0.3.0/tripplite/prometheus.py` & `tripplite-0.4.0/tripplite/prometheus.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 #!/usr/bin/env python3
+"""Collector of metrics from TripLite battery backup for Prometheus."""
 
 import argparse
 import logging
 import sys
 import time
 from socket import getfqdn
 from typing import Generator, List
 
+from tripplite.collectors import Collector
 
 LOG = logging.getLogger(__name__)
 
 
 try:
-    from prometheus_client.core import GaugeMetricFamily, REGISTRY
     from prometheus_client import start_http_server
+    from prometheus_client.core import REGISTRY, GaugeMetricFamily
 except ImportError as ie:
     LOG.error(
         f"prometheus_client not installed: {ie}. Please install with 'exporter' "
         "extra - e.g. `pip install tripplite[exporter]`"
     )
     sys.exit(1)
-from tripplite.collectors import Collector
-
 
 HOSTNAME = getfqdn()
 
 
 class PrometheusCollector(Collector):
-    """Prometheus Collector class to get Dict from Battery and export Prometheus
-    Guages via HTTP server."""
+    """
+    Prometheus Collector class.
+
+    Get Dict from Battery and export Prometheus Guages via HTTP server.
+    """
 
     key_prefix: str = "tripplite"
     labels: List[str] = ["hostname"]
 
     help_test = {
         "health": "UPS components health",
         "time_to_empty": "Runtime left in seconds",
@@ -46,14 +49,15 @@
             self.help_test.get(normalized_category, "Tripplite Metric"),
             labels=self.labels,
         )
         g.add_metric([HOSTNAME], value)
         return g
 
     def collect(self) -> Generator[GaugeMetricFamily, None, None]:
+        """Collect metrics to expose for Prometheus."""
         start_time = time.time()
         LOG.info("Collection started")
 
         self.open_battery()
         ups_data = self.get_data()
         if not ups_data:
             return
@@ -67,14 +71,15 @@
                     yield self._handle_counter(combined_category, float(subvalue))
 
         run_time = time.time() - start_time
         LOG.info(f"Collection finished in {run_time}s")
 
 
 def serve(args: argparse.Namespace) -> int:
+    """Serve metrics for Prometheus to scrape."""
     start_http_server(args.port)
     REGISTRY.register(PrometheusCollector())
     LOG.info(f"Tripplite UPS Prometheus Exporter - listening on {args.port}")
     try:
         while True:
             time.sleep(1)
     except KeyboardInterrupt:
```

### Comparing `tripplite-0.3.0/tripplite.egg-info/PKG-INFO` & `tripplite-0.4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,173 +1,177 @@
 Metadata-Version: 2.1
 Name: tripplite
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python driver for TrippLite UPS battery backups.
-Home-page: http://github.com/numat/tripplite/
+Home-page: https://github.com/numat/tripplite/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 License: GPLv2
-Description: # tripplite
-        
-        Python USB interface and command-line tool for TrippLite UPS battery backups.
-        
-        ![](https://www.markertek.com/productImage/450X450/SMART1500LCD.JPG)
-        
-        ## Background
-        
-        TrippLite offers [UI software](https://www.tripplite.com/products/power-alert)
-        for monitoring its batteries. However, most of its batteries don't have
-        network access, and the existing TrippLite software requires a local install.
-        
-        I wanted to monitor the UPS from a remote headless Linux server, so I wrote
-        this tool.
-        
-        ## Supported Hardware
-        
-        This has been exclusively tested on the TrippLite SMART1500LCD UPS. It will
-        likely work on similar firmware but there is a known communication issue with
-        some other TrippLite models (see [numat/tripplite#3](https://github.com/numat/tripplite/issues/3)).
-        
-        Use `lsusb` to check. `09ae:2012` should work, while `09ae:3016` may not.
-        
-        ## Installation
-        
-        ```console
-        apt install gcc libusb-1.0-0-dev libudev-dev
-        pip install tripplite
-        ```
-        
-        Connect a USB cable from the UPS to your headless server, and you should be
-        ready to run. If you don't want to run as root, see *Note on Permissions*
-        below.
-        
-        # Command Line
-        
-        ```json
-        $ tripplite
-        {
-            "config": {
-                "frequency": 60,  # Hz
-                "power": 1500,  # VA
-                "voltage": 120  # V
-            },
-            "health": 100,  # %
-            "input": {
-                "frequency": 59.7,  # Hz
-                "voltage": 117.2  # V
-            },
-            "output": {
-                "power": 324,  # W
-                "voltage": 117.2  # V
-            },
-            "status": {
-                "ac present": true,
-                "below remaining capacity": true,
-                "charging": false,
-                "discharging": false,
-                "fully charged": true,
-                "fully discharged": false,
-                "needs replacement": false,
-                "shutdown imminent": false
-            },
-            "time to empty": 1004  # s
-        }
-        ```
-        
-        To use in shell scripts, parse the json output with something like
-        [jq](https://stedolan.github.io/jq/). For example,
-        `tripplite | jq '.status."ac present"'` will return whether or not the unit
-        detects AC power.
-        
-        ## Python
-        
-        If you'd like to link this to more complex behavior (e.g. data logging,
-        text alerts), consider using a Python script.
-        
-        ```python
-        from tripplite import Battery
-        with Battery() as battery:
-            print(battery.get())
-        ```
-        
-        The `state` variable will contain an object with the same format as above. Use
-        `state['status']['ac present']` and `state['status']['shutdown imminent']` for
-        alerts, and consider logging voltage, frequency, and power.
-        
-        If you are logging multiple batteries, you will need to handle each connection
-        separately.
-        
-        ```python
-        from tripplite import Battery, battery_paths
-        for path in battery_paths:
-            with Battery(path) as battery:
-                print(battery.get())
-        ```
-        
-        These paths are unfortunately non-deterministic and will change on each
-        iteration. For long running processes please prefer to keep an open `Battery`
-        object and open + close on read errors. For example:
-        
-        ```python
-            def check_batteries(
-                self, battery_paths: List[str], check_period: float = 30.0
-            ) -> None:
-                """Read batteries and reopen in error"""
-                self.batteries = [Battery(path) for path in battery_paths]
-                for battery in self.batteries:
-                    battery.open()
-                while True:
-                    time.sleep(check_period)
-                    for state, battery in zip(self.state, self.batteries):
-                        try:
-                            state.update(battery.get())
-                        except OSError:
-                            logger.exception(f"Could not read battery {battery}.")
-                            battery.close()
-        ```
-        
-        ## Note on Permissions
-        
-        To read the TrippLite, you need access to the USB port. You have options:
-        
-        * Run everything as root
-        * Add your user to the `dialout` group to access *all* serial ports
-        * Create a group restricted to accessing TrippLite USB devices through `udev`
-        
-        For the last option, the rule looks like:
-        
-        ```console
-        echo 'SUBSYSTEM=="usb", ATTRS{idVendor}=="09ae", GROUP="tripplite"' > /etc/udev/rules.d/tripplite.rules
-        udevadm control --reload-rules
-        ```
-        
-        ## Prometheus Exporter
-        
-        This package offers an extra install to include a [Prometheus Exporter](https://prometheus.io/docs/instrumenting/exporters/)
-        which allows for data collection into a prometheus time series database. Esentially it's a small `HTTP` server that allows
-        Prometheus to *scrape* grabbing metrics at a configurable period.
-        
-        ### Install
-        
-        ```console
-        pip install tripplite[exporter]
-        ```
-        
-        * This adds the [prometheus_client](https://pypi.org/project/prometheus-client/) dependency.
-        
-        You can then manually run the `triplite-exporter` cli or use the
-        [tripplite_exporter.service](https://github.com/numat/tripplite/blob/master/tripplite_exporter.service)
-        systemd unit file to have systemd run and supervise the process.
-        
-        ### Failure Mode
-        
-        The script will try to close and reopen the USB serial connection to the device on an `OSError`. If an open fails,
-        the script will exit with the return code of 2.
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Description-Content-Type: text/markdown
 Provides-Extra: exporter
+Provides-Extra: test
+License-File: LICENSE
+
+# tripplite
+
+Python USB interface and command-line tool for TrippLite UPS battery backups.
+
+![](https://www.markertek.com/productImage/450X450/SMART1500LCD.JPG)
+
+## Background
+
+TrippLite offers [UI software](https://www.tripplite.com/products/power-alert)
+for monitoring its batteries. However, most of its batteries don't have
+network access, and the existing TrippLite software requires a local install.
+
+I wanted to monitor the UPS from a remote headless Linux server, so I wrote
+this tool.
+
+## Supported Hardware
+
+This has been exclusively tested on the TrippLite SMART1500LCD UPS. It will
+likely work on similar firmware but there is a known communication issue with
+some other TrippLite models (see [numat/tripplite#3](https://github.com/numat/tripplite/issues/3)).
+
+Use `lsusb` to check. `09ae:2012` should work, while `09ae:3016` may not.
+
+## Installation
+
+```console
+apt install gcc libusb-1.0-0-dev libudev-dev
+pip install tripplite
+```
+
+Connect a USB cable from the UPS to your headless server, and you should be
+ready to run. If you don't want to run as root, see *Note on Permissions*
+below.
+
+# Command Line
+
+```
+$ tripplite
+{
+    "config": {
+        "frequency": 60,  # Hz
+        "power": 1500,  # VA
+        "voltage": 120  # V
+    },
+    "health": 100,  # %
+    "input": {
+        "frequency": 59.7,  # Hz
+        "voltage": 117.2  # V
+    },
+    "output": {
+        "power": 324,  # W
+        "voltage": 117.2  # V
+    },
+    "status": {
+        "ac present": true,
+        "below remaining capacity": true,
+        "charging": false,
+        "discharging": false,
+        "fully charged": true,
+        "fully discharged": false,
+        "needs replacement": false,
+        "shutdown imminent": false
+    },
+    "time to empty": 1004  # s
+}
+```
+
+To use in shell scripts, parse the json output with something like
+[jq](https://stedolan.github.io/jq/). For example,
+`tripplite | jq '.status."ac present"'` will return whether or not the unit
+detects AC power.
+
+## Python
+
+If you'd like to link this to more complex behavior (e.g. data logging,
+text alerts), consider using a Python script.
+
+```python
+from tripplite import Battery
+with Battery() as battery:
+    print(battery.get())
+```
+
+The `state` variable will contain an object with the same format as above. Use
+`state['status']['ac present']` and `state['status']['shutdown imminent']` for
+alerts, and consider logging voltage, frequency, and power.
+
+If you are logging multiple batteries, you will need to handle each connection
+separately.
+
+```python
+from tripplite import Battery, battery_paths
+for path in battery_paths:
+    with Battery(path) as battery:
+        print(battery.get())
+```
+
+These paths are unfortunately non-deterministic and will change on each
+iteration.
+
+For long polling, you can improve stability by keeping connections open as long
+as possible and reconnecting on error. For example:
+
+```python
+state = None
+
+def read_batteries(check_period=5):
+    """Read battery and reopen in error. Use for long polling."""
+    battery = Battery()
+    battery.open()
+    while True:
+        time.sleep(check_period)
+        try:
+            state = battery.get()
+        except OSError:
+            logging.exception(f"Could not read battery {battery}.")
+            battery.close()
+            battery.open()
+```
+
+An example for multiple batteries can be found in [numat/tripplite#6](https://github.com/numat/tripplite/pull/6#issuecomment-700152340).
+
+## Note on Permissions
+
+To read the TrippLite, you need access to the USB port. You have options:
+
+* Run everything as root
+* Add your user to the `dialout` group to access *all* serial ports
+* Create a group restricted to accessing TrippLite USB devices through `udev`
+
+For the last option, the rule looks like:
+
+```console
+echo 'SUBSYSTEM=="usb", ATTRS{idVendor}=="09ae", GROUP="tripplite"' > /etc/udev/rules.d/tripplite.rules
+udevadm control --reload-rules
+```
+
+## Prometheus Exporter
+
+This package offers an extra install to include a [Prometheus Exporter](https://prometheus.io/docs/instrumenting/exporters/)
+which allows for data collection into a prometheus time series database. Esentially it's a small `HTTP` server that allows
+Prometheus to *scrape* grabbing metrics at a configurable period.
+
+### Install
+
+```console
+pip install tripplite[exporter]
+```
+
+* This adds the [prometheus_client](https://pypi.org/project/prometheus-client/) dependency.
+
+You can then manually run the `triplite-exporter` cli or use the
+[tripplite_exporter.service](https://github.com/numat/tripplite/blob/master/tripplite_exporter.service)
+systemd unit file to have systemd run and supervise the process.
+
+### Failure Mode
+
+The script will try to close and reopen the USB serial connection to the device on an `OSError`. If an open fails,
+the script will exit with the return code of 2.
```

