# Comparing `tmp/yokkaichi-1.4.5.tar.gz` & `tmp/yokkaichi-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yokkaichi-1.4.5.tar", last modified: Tue May 16 21:24:53 2023, max compression
+gzip compressed data, was "yokkaichi-1.5.tar", last modified: Sun Jul  9 20:58:56 2023, max compression
```

## Comparing `yokkaichi-1.4.5.tar` & `yokkaichi-1.5.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-16 21:24:53.157905 yokkaichi-1.4.5/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.4.5/LICENSE.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-16 21:24:53.157905 yokkaichi-1.4.5/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2252 2023-05-12 19:27:27.000000 yokkaichi-1.4.5/README.md
--rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-05-16 21:24:53.157905 yokkaichi-1.4.5/setup.cfg
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1547 2023-05-14 22:01:12.000000 yokkaichi-1.4.5/setup.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-16 21:24:53.154572 yokkaichi-1.4.5/yokkaichi/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2921 2023-05-12 18:51:44.000000 yokkaichi-1.4.5/yokkaichi/MasscanScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     5835 2023-05-16 21:23:31.000000 yokkaichi-1.4.5/yokkaichi/ServerScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-05-16 21:23:31.000000 yokkaichi-1.4.5/yokkaichi/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     8949 2023-05-16 21:23:31.000000 yokkaichi-1.4.5/yokkaichi/__main__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1261 2023-05-12 18:51:44.000000 yokkaichi-1.4.5/yokkaichi/args_to_cfg.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3847 2023-05-15 20:13:39.000000 yokkaichi-1.4.5/yokkaichi/config_loader.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-16 21:24:53.157905 yokkaichi-1.4.5/yokkaichi/constants/
--rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.4.5/yokkaichi/constants/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       69 2023-05-14 19:38:14.000000 yokkaichi-1.4.5/yokkaichi/constants/rich_console.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1160 2023-05-12 18:51:44.000000 yokkaichi-1.4.5/yokkaichi/port_parser.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-16 21:24:53.157905 yokkaichi-1.4.5/yokkaichi/structs/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1053 2023-05-14 22:01:12.000000 yokkaichi-1.4.5/yokkaichi/structs/CFG.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.4.5/yokkaichi/structs/__init__.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-05-16 21:24:53.154572 yokkaichi-1.4.5/yokkaichi.egg-info/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     3022 2023-05-16 21:24:53.000000 yokkaichi-1.4.5/yokkaichi.egg-info/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)      487 2023-05-16 21:24:53.000000 yokkaichi-1.4.5/yokkaichi.egg-info/SOURCES.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-05-16 21:24:53.000000 yokkaichi-1.4.5/yokkaichi.egg-info/dependency_links.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       63 2023-05-16 21:24:53.000000 yokkaichi-1.4.5/yokkaichi.egg-info/requires.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-05-16 21:24:53.000000 yokkaichi-1.4.5/yokkaichi.egg-info/top_level.txt
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:58:56.856030 yokkaichi-1.5/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.5/LICENSE.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2997 2023-07-09 20:58:56.856030 yokkaichi-1.5/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2205 2023-05-24 18:11:37.000000 yokkaichi-1.5/README.md
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       57 2023-05-24 14:00:39.000000 yokkaichi-1.5/pyproject.toml
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-07-09 20:58:56.856030 yokkaichi-1.5/setup.cfg
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1626 2023-07-09 20:54:16.000000 yokkaichi-1.5/setup.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:58:56.852696 yokkaichi-1.5/yokkaichi/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2923 2023-05-24 14:00:39.000000 yokkaichi-1.5/yokkaichi/MasscanScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     5939 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/ServerScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       20 2023-07-09 20:55:21.000000 yokkaichi-1.5/yokkaichi/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     9027 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/__main__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1609 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/args_to_cfg.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     4364 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/config_loader.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:58:56.852696 yokkaichi-1.5/yokkaichi/constants/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.5/yokkaichi/constants/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       69 2023-05-14 19:38:14.000000 yokkaichi-1.5/yokkaichi/constants/rich_console.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:58:56.852696 yokkaichi-1.5/yokkaichi/enums/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       98 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/enums/MasscanMethods.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       89 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/enums/Platforms.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/enums/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1168 2023-05-24 14:00:39.000000 yokkaichi-1.5/yokkaichi/port_parser.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:58:56.852696 yokkaichi-1.5/yokkaichi/structs/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1015 2023-07-09 20:54:16.000000 yokkaichi-1.5/yokkaichi/structs/CFG.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-05-14 22:01:12.000000 yokkaichi-1.5/yokkaichi/structs/__init__.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-07-09 20:58:56.852696 yokkaichi-1.5/yokkaichi.egg-info/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2997 2023-07-09 20:58:56.000000 yokkaichi-1.5/yokkaichi.egg-info/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      593 2023-07-09 20:58:56.000000 yokkaichi-1.5/yokkaichi.egg-info/SOURCES.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-07-09 20:58:56.000000 yokkaichi-1.5/yokkaichi.egg-info/dependency_links.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       81 2023-07-09 20:58:56.000000 yokkaichi-1.5/yokkaichi.egg-info/requires.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-07-09 20:58:56.000000 yokkaichi-1.5/yokkaichi.egg-info/top_level.txt
```

### Comparing `yokkaichi-1.4.5/LICENSE.txt` & `yokkaichi-1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.4.5/PKG-INFO` & `yokkaichi-1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.4.5
+Version: 1.5
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 License: MIT
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -12,18 +12,22 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 License-File: LICENSE.txt
 
+<div align="center">
+
 # Yokkaichi (formely mcserverscanner) - Shodan-like server scanner for Minecraft.
-![total lines](https://img.shields.io/tokei/lines/github/Oreeeee/yokkaichi) ![downloads](https://img.shields.io/pypi/dm/yokkaichi) ![issues](https://img.shields.io/github/issues/Oreeeee/yokkaichi) ![pull requests](https://img.shields.io/github/issues-pr/Oreeeee/yokkaichi) ![license](https://img.shields.io/github/license/Oreeeee/yokkaichi) ![release](https://img.shields.io/github/v/release/Oreeeee/yokkaichi) ![commits since release](https://img.shields.io/github/commits-since/Oreeeee/yokkaichi/latest) ![code style](https://img.shields.io/badge/code%20style-black-black) ![stars](https://img.shields.io/github/stars/Oreeeee/yokkaichi?style=social)
+![downloads](https://img.shields.io/pypi/dm/yokkaichi) ![issues](https://img.shields.io/github/issues/Oreeeee/yokkaichi) ![pull requests](https://img.shields.io/github/issues-pr/Oreeeee/yokkaichi) ![license](https://img.shields.io/github/license/Oreeeee/yokkaichi) ![release](https://img.shields.io/github/v/release/Oreeeee/yokkaichi) ![commits since release](https://img.shields.io/github/commits-since/Oreeeee/yokkaichi/latest) ![code style](https://img.shields.io/badge/code%20style-black-black) ![stars](https://img.shields.io/github/stars/Oreeeee/yokkaichi?style=social)
+</div>
 
 ## Renaming notice!
 This project used to be named mcserverscanner, but on 2023-01-15 it got renamed to Yokkaichi.
 
 ### Features
 - Scanning for Java and Bedrock servers
 - Masscan integration
```

### Comparing `yokkaichi-1.4.5/README.md` & `yokkaichi-1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+<div align="center">
+
 # Yokkaichi (formely mcserverscanner) - Shodan-like server scanner for Minecraft.
-![total lines](https://img.shields.io/tokei/lines/github/Oreeeee/yokkaichi) ![downloads](https://img.shields.io/pypi/dm/yokkaichi) ![issues](https://img.shields.io/github/issues/Oreeeee/yokkaichi) ![pull requests](https://img.shields.io/github/issues-pr/Oreeeee/yokkaichi) ![license](https://img.shields.io/github/license/Oreeeee/yokkaichi) ![release](https://img.shields.io/github/v/release/Oreeeee/yokkaichi) ![commits since release](https://img.shields.io/github/commits-since/Oreeeee/yokkaichi/latest) ![code style](https://img.shields.io/badge/code%20style-black-black) ![stars](https://img.shields.io/github/stars/Oreeeee/yokkaichi?style=social)
+![downloads](https://img.shields.io/pypi/dm/yokkaichi) ![issues](https://img.shields.io/github/issues/Oreeeee/yokkaichi) ![pull requests](https://img.shields.io/github/issues-pr/Oreeeee/yokkaichi) ![license](https://img.shields.io/github/license/Oreeeee/yokkaichi) ![release](https://img.shields.io/github/v/release/Oreeeee/yokkaichi) ![commits since release](https://img.shields.io/github/commits-since/Oreeeee/yokkaichi/latest) ![code style](https://img.shields.io/badge/code%20style-black-black) ![stars](https://img.shields.io/github/stars/Oreeeee/yokkaichi?style=social)
+</div>
 
 ## Renaming notice!
 This project used to be named mcserverscanner, but on 2023-01-15 it got renamed to Yokkaichi.
 
 ### Features
 - Scanning for Java and Bedrock servers
 - Masscan integration
```

### Comparing `yokkaichi-1.4.5/setup.py` & `yokkaichi-1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from yokkaichi import __version__ as yokkaichi_ver
-from setuptools import setup
-from pathlib import Path
 import sys
+from pathlib import Path
+
+from setuptools import setup
+
+from yokkaichi import __version__ as yokkaichi_ver
 
 # Load README from README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-# Enforce Python version (3.7+)
-if sys.version_info[1] < 7:
-    sys.exit(
-        "Yokkaichi will NOT run on Python 3.6 and older. You can build the package yourself and remove the check, but don't report bugs that happen!"
+# Enforce Python version (3.8+)
+if sys.version_info[1] < 8:
+    print(
+        "NOTICE: Yokkaichi requires Python 3.8 or newer to run. Python 3.7 and older are not supported, and bugs might happen."
     )
 
 setup(
     name="yokkaichi",
     version=yokkaichi_ver,
     description="Shodan-like server scanner for Minecraft (formely mcserverscanner)",
     long_description=long_description,
@@ -26,21 +28,27 @@
         "rich",
         "mcstatus",
         "ip2location",
         "python-masscan",
         "requests",
         "tomli >= 1.1.0",
     ],
+    extras_require={"testing": ["pytest"]},
     classifiers=[
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
-    packages=["yokkaichi", "yokkaichi.constants", "yokkaichi.structs"],
+    packages=[
+        "yokkaichi",
+        "yokkaichi.constants",
+        "yokkaichi.structs",
+        "yokkaichi.enums",
+    ],
 )
```

### Comparing `yokkaichi-1.4.5/yokkaichi/MasscanScan.py` & `yokkaichi-1.5/yokkaichi/MasscanScan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from .constants.rich_console import console
-from pathlib import Path
+import json
 import platform
+from pathlib import Path
+
 import masscan
-import json
+
+from .constants.rich_console import console
 
 
 class MasscanScan:
     def __init__(self, cfg, ip_list):
         # Declare variables
         self.cfg = cfg
         self.ip_list = ip_list
```

### Comparing `yokkaichi-1.4.5/yokkaichi/ServerScan.py` & `yokkaichi-1.5/yokkaichi/ServerScan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Import modules
-from mcstatus import BedrockServer, JavaServer
-from .constants.rich_console import console
+import ast
+import json
+import threading
 from datetime import datetime
+
 import IP2Location
-import threading
-import json
-import ast
+from mcstatus import BedrockServer, JavaServer
+
+from .constants.rich_console import console
+from .enums import Platforms
 
 
 class ServerScan:
     def __init__(self, cfg, masscan_list, ip_list):
         self.cfg = cfg
         self.masscan_list = masscan_list
         self.ip_list = ip_list
@@ -70,15 +73,15 @@
             for port in ports:
                 for server_platform in self.cfg.platforms:
                     try:
                         self.check_server(ip, port, server_platform)
                     except Exception:
                         with self.lock:
                             console.print(
-                                f"[-] {ip}:{port} for {server_platform} is offline!",
+                                f"[-] {ip}:{port} for {server_platform.value} is offline!",
                                 style="red",
                             )
 
     def scan_ip_list(self):
         while True:
             with self.lock:
                 try:
@@ -93,22 +96,22 @@
             for port in self.cfg.ports:
                 for server_platform in self.cfg.platforms:
                     try:
                         self.check_server(ip, port, server_platform)
                     except Exception as e:
                         with self.lock:
                             console.print(
-                                f"[-] {ip}:{port} for {server_platform} is offline!",
+                                f"[-] {ip}:{port} for {server_platform.value} is offline!",
                                 style="red",
                             )
 
     def check_server(self, ip, port, server_platform):
-        if server_platform == "Java":
+        if server_platform == Platforms.JAVA:
             server_lookup = JavaServer.lookup(f"{ip}:{port}")
-        if server_platform == "Bedrock":
+        if server_platform == Platforms.BEDROCK:
             server_lookup = BedrockServer.lookup(f"{ip}:{port}")
 
         # Get player list
         if self.cfg.query_java:
             try:
                 player_list = server_lookup.query().players.names
             except Exception as e:
@@ -118,36 +121,37 @@
             player_list = None
 
         server_info = {
             "ip": ip,
             "port": port,
             "info": self.get_location_data(ip),
             "ping": round(server_lookup.status().latency),
-            "platform": server_platform,
+            "platform": server_platform.value,
             "motd": "",
             "version": "",
             "online_players": 0,
             "max_players": 0,
             "player_list": player_list,
             "time_discovered": datetime.now().isoformat(),
         }
-        if server_platform == "Java":
+        if server_platform == Platforms.JAVA:
             server_info["motd"] = server_lookup.status().description
             server_info["version"] = server_lookup.status().version.name
             server_info["online_players"] = server_lookup.status().players.online
             server_info["max_players"] = server_lookup.status().players.max
-        if server_platform == "Bedrock":
+        if server_platform == Platforms.BEDROCK:
             server_info["motd"] = server_lookup.status().motd
             server_info["version"] = ""
             server_info["online_players"] = server_lookup.status().players_online
             server_info["max_players"] = server_lookup.status().players_max
 
         with self.lock:
             console.print(
-                f"[+] {server_platform} server found at {ip}:{port}!", style="green"
+                f"[+] {server_platform.value} server found at {ip}:{port}!",
+                style="green",
             )
             self.add_to_file(server_info)
 
     def get_location_data(self, ip):
         # Make the data be a string
         ip2location_data_str = str(self.ip2location_db.get_all(ip))
         # Convert the data to dict
```

### Comparing `yokkaichi-1.4.5/yokkaichi/__main__.py` & `yokkaichi-1.5/yokkaichi/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Import modules
-from .constants.rich_console import console
-from .port_parser import parse_port_range
-from .args_to_cfg import args_to_cfg
-from .MasscanScan import MasscanScan
-from .ServerScan import ServerScan
-from yokkaichi import __version__
+import argparse
+import pathlib
+import platform
+import time
 from datetime import datetime
-from . import config_loader
+
 import IP2Location
-import platform
-import argparse
 import requests
-import pathlib
 import tomli
-import time
+
+from yokkaichi import __version__
+
+from . import config_loader
+from .args_to_cfg import args_to_cfg
+from .constants.rich_console import console
+from .enums.MasscanMethods import MasscanMethods
+from .MasscanScan import MasscanScan
+from .port_parser import parse_port_range
+from .ServerScan import ServerScan
 
 
 def display_version():
     console.print(
         f"yokkaichi [bold cyan]{__version__}[/bold cyan] on [bold cyan]{platform.python_implementation()} {platform.python_version()}[/bold cyan]",
         style="green",
     )
@@ -124,18 +128,18 @@
         console.print(f"Loaded {len(ip_list)} IPs", style="green")
     else:
         ip_list = None
 
     if cfg.masscan_scan:
         masscan_ips_from_file = []
         masscan_ips_for_countries = []
-        if cfg.masscan_ip_source == "countries":
+        if cfg.masscan_ip_source == MasscanMethods.COUNTRIES:
             # Get CIDR ranges for countries
             masscan_ips = get_country_ips(cfg.masscan_country_list)
-        elif cfg.masscan_ip_source == "list":
+        elif cfg.masscan_ip_source == MasscanMethods.LIST:
             # Load masscan IP list
             masscan_ips = load_ip_list(cfg.masscan_ip_list)
 
         # Combine two sources of masscan IPs together
         # masscan_ips = masscan_ips_from_file + masscan_ips_for_countries
 
         # Start masscan
```

### Comparing `yokkaichi-1.4.5/yokkaichi/args_to_cfg.py` & `yokkaichi-1.5/yokkaichi/args_to_cfg.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 from .constants.rich_console import console
+from .enums.MasscanMethods import MasscanMethods
+from .enums.Platforms import Platforms
 from .port_parser import parse_port_range
 from .structs.CFG import CFG
 
 
 def args_to_cfg(args):
     cfg = CFG()
 
     if args.java:
-        cfg.platforms.append("java")
+        cfg.platforms.append(Platforms.JAVA)
     if args.bedrock:
-        cfg.platforms.append("bedrock")
+        cfg.platforms.append(Platforms.BEDROCK)
 
     cfg.query_java = args.query
     cfg.masscan_scan = args.masscan
     cfg.ip_list_scan = args.ip_list_scan
 
-    if args.masscan_method not in ("countries", "list"):
+    if args.masscan_method == MasscanMethods.COUNTRIES.value:
+        cfg.masscan_ip_source = MasscanMethods.COUNTRIES
+    elif args.masscan_method == MasscanMethods.LIST.value:
+        cfg.masscan_ip_source == MasscanMethods.LIST
+    else:
         console.print(
-            "Proper values for --masscan-method are: countries, list", style="bold red"
+            f"Proper values for --masscan-method are: {[p.value for p in MasscanMethods]}",
+            style="bold red",
         )
         exit(1)
+        return True
 
-    cfg.masscan_ip_source = args.masscan_method
     cfg.masscan_args = args.masscan_args
 
     if args.masscan_json_output == "":
         cfg.masscan_output = False
 
     cfg.masscan_output_location = args.masscan_json_output
     cfg.masscan_ip_list = args.masscan_ip_list
     cfg.ip_list = args.ip_list
+    cfg.masscan_country_list = args.masscan_countries
     cfg.ports = parse_port_range(args.ports)
     cfg.threads = args.thread_count
     cfg.output = args.output_file
 
     if args.ip2location_db != "":
         cfg.use_ip2location = True
         cfg.ip2location_db = args.ip2location_db
```

### Comparing `yokkaichi-1.4.5/yokkaichi/config_loader.py` & `yokkaichi-1.5/yokkaichi/config_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+import tomli
+
 from .constants.rich_console import console
+from .enums.MasscanMethods import MasscanMethods
+from .enums.Platforms import Platforms
 from .port_parser import parse_port_range
 from .structs.CFG import CFG
-import tomli
 
 CONFIG_VERSION = "1"
 # TODO: Bring this back to a separate file
 SAMPLE_CFG = """
 # This is an example configuration file for Yokkaichi.
 # Configure this for your preferences.
 # Pass the location to this config file with -c as an argument.
 # Example: python -m yokkaichi -c sample.toml
 # You can pass this without the file location and it will look for yokkaichi.toml in your current location.
+# Do not comment any of the config's options, it will currently cause a crash
 
 version = "1" # Changed for every change breaking config compatibility
 
 [platforms]
 java = true
 bedrock = false
 
@@ -37,52 +41,65 @@
 [type.options_masscan.list]
 list = "masscan_ips.txt" # Location to the list of IPs to scan with masscan, separated by newlines
 
 [type.options_ip_list]
 list = "ips.txt" # Location to the list of IPs to scan, separated by newlines
 
 [scanner]
-ports = "25564-25566,25569" # Port list (not TOML's format! Splits ports by commas, sets ranges with hyphens)
+ports = "25564-25566,25569" # Port list (not TOML's format! Similarly to nmap and masscan splits ports by commas and sets ranges with hyphens)
 threads = 100 # Leave this at default unless you have a lot of servers
 output = "out.json" # IMPORTANT! That's where the servers go!
 
 [ip2location]
 enabled = false # Enable getting the location of the server
 db = "IP2LOCATION-LITE-DB11.BIN" # IP2Location .BIN database (get from lite.ip2location.com)
-cache = true # Enable for faster speed at the cost of RAM (doesn't really matter with Lite database)
+cache = true # Enable for faster speed at the cost of RAM
 """.strip()
 
 
-def parse_cfg(cfg_location):
-    # Read the config file
+def load_cfg(cfg_location):
     with open(cfg_location, "rb") as f:
         cfg_file = tomli.load(f)
+    return cfg_file
+
+
+def parse_cfg(cfg_location):
+    # Read the config file
+    cfg_file = load_cfg(cfg_location)
 
     cfg = CFG()
 
     # TODO: Check if the file is a valid Yokkaichi config!
     cfg_file_ver = cfg_file["version"]
     if cfg_file_ver != CONFIG_VERSION:
         console.print(
             f"Wrong config version detected! Please update your config. Your config: {cfg_file_ver}. Expected: {CONFIG_VERSION}",
             style="bold red",
         )
         exit(1)
+        return True
 
     if cfg_file["platforms"]["java"]:
-        cfg.platforms.append("Java")
+        cfg.platforms.append(Platforms.JAVA)
     if cfg_file["platforms"]["bedrock"]:
-        cfg.platforms.append("Bedrock")
+        cfg.platforms.append(Platforms.BEDROCK)
 
     cfg.query_java = cfg_file["platforms"]["additional"]["java_query"]
 
     cfg.masscan_scan = cfg_file["type"]["masscan"]
     cfg.ip_list_scan = cfg_file["type"]["ip_list"]
 
-    cfg.masscan_ip_source = cfg_file["type"]["options_masscan"]["ip_source"]
+    if (
+        cfg_file["type"]["options_masscan"]["ip_source"]
+        == MasscanMethods.COUNTRIES.value
+    ):
+        cfg.masscan_ip_source = MasscanMethods.COUNTRIES
+    elif cfg_file["type"]["options_masscan"]["ip_source"] == MasscanMethods.LIST.value:
+        cfg.masscan_ip_source = MasscanMethods.LIST
+
     cfg.masscan_args = cfg_file["type"]["options_masscan"]["args"]
     cfg.masscan_output = cfg_file["type"]["options_masscan"]["output"]
     cfg.masscan_output_location = cfg_file["type"]["options_masscan"]["output_location"]
 
     cfg.masscan_country_list = cfg_file["type"]["options_masscan"]["countries"][
         "countries"
     ]
```

### Comparing `yokkaichi-1.4.5/yokkaichi/port_parser.py` & `yokkaichi-1.5/yokkaichi/port_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
                 int(range_start), int(range_end) + 1
             ):  # Range end needs to be offset by 1 to make the range inclusive
                 ports.append(port)
         else:
             verify_ints(value)
             ports.append(int(value))
 
-    return list(set(ports))
+    return list(sorted(set(ports)))
```

### Comparing `yokkaichi-1.4.5/yokkaichi/structs/CFG.py` & `yokkaichi-1.5/yokkaichi/structs/CFG.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass, field
 
 
 @dataclass
 class CFG:
-    platforms: list = field(default_factory=list)  # Possible values: "java", "bedrock"
+    platforms: list = field(default_factory=list)
     query_java: bool = field(default_factory=bool)
     masscan_scan: bool = field(default_factory=bool)
     ip_list_scan: bool = field(default_factory=bool)
     masscan_ip_source: str = field(
         default_factory=str
     )  # Possible values: "countries", "list"
     masscan_args: str = field(default_factory=str)
```

### Comparing `yokkaichi-1.4.5/yokkaichi.egg-info/PKG-INFO` & `yokkaichi-1.5/yokkaichi.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.4.5
+Version: 1.5
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 License: MIT
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -12,18 +12,22 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 License-File: LICENSE.txt
 
+<div align="center">
+
 # Yokkaichi (formely mcserverscanner) - Shodan-like server scanner for Minecraft.
-![total lines](https://img.shields.io/tokei/lines/github/Oreeeee/yokkaichi) ![downloads](https://img.shields.io/pypi/dm/yokkaichi) ![issues](https://img.shields.io/github/issues/Oreeeee/yokkaichi) ![pull requests](https://img.shields.io/github/issues-pr/Oreeeee/yokkaichi) ![license](https://img.shields.io/github/license/Oreeeee/yokkaichi) ![release](https://img.shields.io/github/v/release/Oreeeee/yokkaichi) ![commits since release](https://img.shields.io/github/commits-since/Oreeeee/yokkaichi/latest) ![code style](https://img.shields.io/badge/code%20style-black-black) ![stars](https://img.shields.io/github/stars/Oreeeee/yokkaichi?style=social)
+![downloads](https://img.shields.io/pypi/dm/yokkaichi) ![issues](https://img.shields.io/github/issues/Oreeeee/yokkaichi) ![pull requests](https://img.shields.io/github/issues-pr/Oreeeee/yokkaichi) ![license](https://img.shields.io/github/license/Oreeeee/yokkaichi) ![release](https://img.shields.io/github/v/release/Oreeeee/yokkaichi) ![commits since release](https://img.shields.io/github/commits-since/Oreeeee/yokkaichi/latest) ![code style](https://img.shields.io/badge/code%20style-black-black) ![stars](https://img.shields.io/github/stars/Oreeeee/yokkaichi?style=social)
+</div>
 
 ## Renaming notice!
 This project used to be named mcserverscanner, but on 2023-01-15 it got renamed to Yokkaichi.
 
 ### Features
 - Scanning for Java and Bedrock servers
 - Masscan integration
```

