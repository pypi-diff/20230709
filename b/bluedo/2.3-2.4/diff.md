# Comparing `tmp/bluedo-2.3.tar.gz` & `tmp/bluedo-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluedo-2.3.tar", last modified: Fri Jul  7 23:45:37 2023, max compression
+gzip compressed data, was "bluedo-2.4.tar", last modified: Sun Jul  9 09:20:03 2023, max compression
```

## Comparing `bluedo-2.3.tar` & `bluedo-2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.787989 bluedo-2.3/
--rw-rw-r--   0 lars      (1000) lars      (1000)    35149 2022-11-05 18:15:30.000000 bluedo-2.3/LICENSE
--rw-rw-r--   0 lars      (1000) lars      (1000)      487 2022-11-05 18:15:30.000000 bluedo-2.3/MANIFEST.in
--rw-rw-r--   0 lars      (1000) lars      (1000)     4050 2023-07-07 23:45:37.787989 bluedo-2.3/PKG-INFO
--rw-rw-r--   0 lars      (1000) lars      (1000)     3181 2023-07-07 23:40:24.000000 bluedo-2.3/README.md
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.783989 bluedo-2.3/applications/
--rw-rw-r--   0 lars      (1000) lars      (1000)      251 2022-11-05 18:15:30.000000 bluedo-2.3/applications/bluedo.desktop
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.787989 bluedo-2.3/bluedo/
--rwxrwxr-x   0 lars      (1000) lars      (1000)      252 2022-11-04 22:23:57.000000 bluedo-2.3/bluedo/__init__.py
--rw-rw-r--   0 lars      (1000) lars      (1000)   106494 2022-11-04 22:23:57.000000 bluedo-2.3/bluedo/bluedo.png
--rw-rw-r--   0 lars      (1000) lars      (1000)    27134 2023-07-07 23:43:01.000000 bluedo-2.3/bluedo/bluedoapp.py
--rw-rw-r--   0 lars      (1000) lars      (1000)    79675 2022-11-04 22:23:57.000000 bluedo-2.3/bluedo/lock_animation.gif
--rw-rw-r--   0 lars      (1000) lars      (1000)     8631 2022-11-04 22:23:57.000000 bluedo-2.3/bluedo/unlocked.png
--rw-rw-r--   0 lars      (1000) lars      (1000)    21441 2023-07-07 23:38:29.000000 bluedo-2.3/bluedo/window.glade
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.787989 bluedo-2.3/bluedo.egg-info/
--rw-r--r--   0 lars      (1000) lars      (1000)     4050 2023-07-07 23:45:37.000000 bluedo-2.3/bluedo.egg-info/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      415 2023-07-07 23:45:37.000000 bluedo-2.3/bluedo.egg-info/SOURCES.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-07-07 23:45:37.000000 bluedo-2.3/bluedo.egg-info/dependency_links.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       40 2023-07-07 23:45:37.000000 bluedo-2.3/bluedo.egg-info/entry_points.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       48 2023-07-07 23:45:37.000000 bluedo-2.3/bluedo.egg-info/requires.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        7 2023-07-07 23:45:37.000000 bluedo-2.3/bluedo.egg-info/top_level.txt
--rw-rw-r--   0 lars      (1000) lars      (1000)       38 2023-07-07 23:45:37.787989 bluedo-2.3/setup.cfg
--rw-rw-r--   0 lars      (1000) lars      (1000)     2263 2023-07-07 23:38:29.000000 bluedo-2.3/setup.py
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.783989 bluedo-2.3/share/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.783989 bluedo-2.3/share/icons/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.783989 bluedo-2.3/share/icons/hicolor/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.783989 bluedo-2.3/share/icons/hicolor/256x256/
-drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-07 23:45:37.787989 bluedo-2.3/share/icons/hicolor/256x256/apps/
--rw-rw-r--   0 lars      (1000) lars      (1000)   106494 2022-11-05 18:15:30.000000 bluedo-2.3/share/icons/hicolor/256x256/apps/bluedo.png
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.991805 bluedo-2.4/
+-rw-rw-r--   0 lars      (1000) lars      (1000)    35149 2022-11-05 18:15:30.000000 bluedo-2.4/LICENSE
+-rw-rw-r--   0 lars      (1000) lars      (1000)      487 2022-11-05 18:15:30.000000 bluedo-2.4/MANIFEST.in
+-rw-rw-r--   0 lars      (1000) lars      (1000)     4101 2023-07-09 09:20:03.991805 bluedo-2.4/PKG-INFO
+-rw-rw-r--   0 lars      (1000) lars      (1000)     3181 2023-07-09 09:14:35.000000 bluedo-2.4/README.md
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.987805 bluedo-2.4/applications/
+-rw-rw-r--   0 lars      (1000) lars      (1000)      251 2022-11-05 18:15:30.000000 bluedo-2.4/applications/bluedo.desktop
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.987805 bluedo-2.4/bluedo/
+-rwxrwxr-x   0 lars      (1000) lars      (1000)      252 2022-11-04 22:23:57.000000 bluedo-2.4/bluedo/__init__.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)   106494 2022-11-04 22:23:57.000000 bluedo-2.4/bluedo/bluedo.png
+-rw-rw-r--   0 lars      (1000) lars      (1000)    27528 2023-07-09 09:16:36.000000 bluedo-2.4/bluedo/bluedoapp.py
+-rw-rw-r--   0 lars      (1000) lars      (1000)    79675 2022-11-04 22:23:57.000000 bluedo-2.4/bluedo/lock_animation.gif
+-rw-rw-r--   0 lars      (1000) lars      (1000)     8631 2022-11-04 22:23:57.000000 bluedo-2.4/bluedo/unlocked.png
+-rw-rw-r--   0 lars      (1000) lars      (1000)    21441 2023-07-07 23:38:29.000000 bluedo-2.4/bluedo/window.glade
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.991805 bluedo-2.4/bluedo.egg-info/
+-rw-r--r--   0 lars      (1000) lars      (1000)     4101 2023-07-09 09:20:03.000000 bluedo-2.4/bluedo.egg-info/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      415 2023-07-09 09:20:03.000000 bluedo-2.4/bluedo.egg-info/SOURCES.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-07-09 09:20:03.000000 bluedo-2.4/bluedo.egg-info/dependency_links.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       40 2023-07-09 09:20:03.000000 bluedo-2.4/bluedo.egg-info/entry_points.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       48 2023-07-09 09:20:03.000000 bluedo-2.4/bluedo.egg-info/requires.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        7 2023-07-09 09:20:03.000000 bluedo-2.4/bluedo.egg-info/top_level.txt
+-rw-rw-r--   0 lars      (1000) lars      (1000)       38 2023-07-09 09:20:03.991805 bluedo-2.4/setup.cfg
+-rw-rw-r--   0 lars      (1000) lars      (1000)     2313 2023-07-09 09:14:03.000000 bluedo-2.4/setup.py
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.987805 bluedo-2.4/share/
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.987805 bluedo-2.4/share/icons/
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.987805 bluedo-2.4/share/icons/hicolor/
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.987805 bluedo-2.4/share/icons/hicolor/256x256/
+drwxrwxr-x   0 lars      (1000) lars      (1000)        0 2023-07-09 09:20:03.991805 bluedo-2.4/share/icons/hicolor/256x256/apps/
+-rw-rw-r--   0 lars      (1000) lars      (1000)   106494 2022-11-05 18:15:30.000000 bluedo-2.4/share/icons/hicolor/256x256/apps/bluedo.png
```

### Comparing `bluedo-2.3/LICENSE` & `bluedo-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bluedo-2.3/PKG-INFO` & `bluedo-2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: bluedo
-Version: 2.3
+Version: 2.4
 Summary: Bluetooth proximity automation
 Home-page: https://github.com/ways/BlueDo/
 Author: Lars Falk-Petersen
 Author-email: dev@falkp.no
 License: GPLv3+
 Keywords: bluetooth
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Desktop Environment
 Classifier: Topic :: Desktop Environment :: Gnome
 Classifier: Topic :: Security
 Classifier: Environment :: X11 Applications :: Gnome
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: English
 Requires-Python: >=3.10
```

### Comparing `bluedo-2.3/README.md` & `bluedo-2.4/README.md`

 * *Files identical despite different names*

### Comparing `bluedo-2.3/bluedo/bluedo.png` & `bluedo-2.4/bluedo/bluedo.png`

 * *Files identical despite different names*

### Comparing `bluedo-2.3/bluedo/bluedoapp.py` & `bluedo-2.4/bluedo/bluedoapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import syslog
 import appdirs
 import configparser
 
 
 class BlueDo(Gtk.Application):
     project_name = 'bluedo'
-    project_version = 2.3
+    project_version = 2.4
     config_path = appdirs.user_config_dir(project_name) + '/' + project_name + '.ini'
     config_section = 'CONFIG'
     run_path = os.path.dirname(os.path.realpath(__file__)) + '/'
     autostart_dir = os.getenv("HOME") + '/.config/autostart/'
 
     builder = None
     enabled = False
@@ -611,14 +611,16 @@
             #     syslog.syslog("Error: %s" % err)
 
             if rssi is None or rssi < self.threshold:
                 if self.debug:
                     syslog.syslog("No connection")
                     if lost_pings > 0:
                         syslog.syslog("Lost %s" % lost_pings)
+                        if lost_pings%5 == 0:
+                            attempt_bluetooth_connection(self.bt_address)
 
                 if self.enabled:
                     lost_pings += 1
                     if lost_pings == self.away_count:
                         away_callback()
             elif lost_pings > 0:
                 lost_pings = 0
@@ -670,14 +672,19 @@
             run_user_command(cmd=self.entry_away.get_text())
 
 
 #
 # Static functions
 #
 
+def attempt_bluetooth_connection(device):
+    """ Sometimes ubuntu seems to not reconnect automatically. """
+    syslog.syslog("Attempting to start a bluetooth connection.")
+    subprocess.run(f"/usr/bin/bluetoothctl connect {device} > /dev/null", shell=True, check=False)
+
 def run_user_command(cmd=''):
     ''' Run user supplied command '''
     syslog.syslog("Running user command <%s>." % cmd)
     subprocess.run(cmd, shell=True, check=True)
 
 def mute():
     ''' Mute sound '''
```

### Comparing `bluedo-2.3/bluedo/lock_animation.gif` & `bluedo-2.4/bluedo/lock_animation.gif`

 * *Files identical despite different names*

### Comparing `bluedo-2.3/bluedo/unlocked.png` & `bluedo-2.4/bluedo/unlocked.png`

 * *Files identical despite different names*

### Comparing `bluedo-2.3/bluedo/window.glade` & `bluedo-2.4/bluedo/window.glade`

 * *Files identical despite different names*

### Comparing `bluedo-2.3/bluedo.egg-info/PKG-INFO` & `bluedo-2.4/bluedo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: bluedo
-Version: 2.3
+Version: 2.4
 Summary: Bluetooth proximity automation
 Home-page: https://github.com/ways/BlueDo/
 Author: Lars Falk-Petersen
 Author-email: dev@falkp.no
 License: GPLv3+
 Keywords: bluetooth
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Desktop Environment
 Classifier: Topic :: Desktop Environment :: Gnome
 Classifier: Topic :: Security
 Classifier: Environment :: X11 Applications :: Gnome
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: English
 Requires-Python: >=3.10
```

### Comparing `bluedo-2.3/setup.py` & `bluedo-2.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
 
         # Specify the Python versions you support here.
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         "Topic :: Desktop Environment",
         "Topic :: Desktop Environment :: Gnome",
         "Topic :: Security",
         "Environment :: X11 Applications :: Gnome",
         "Operating System :: POSIX :: Linux",
         "Natural Language :: English"
     ],
```

### Comparing `bluedo-2.3/share/icons/hicolor/256x256/apps/bluedo.png` & `bluedo-2.4/share/icons/hicolor/256x256/apps/bluedo.png`

 * *Files identical despite different names*

