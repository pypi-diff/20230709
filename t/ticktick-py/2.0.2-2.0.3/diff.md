# Comparing `tmp/ticktick-py-2.0.2.tar.gz` & `tmp/ticktick-py-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ticktick-py-2.0.2.tar", last modified: Mon Dec 27 08:57:16 2021, max compression
+gzip compressed data, was "ticktick-py-2.0.3.tar", last modified: Sun Jul  9 05:05:17 2023, max compression
```

## Comparing `ticktick-py-2.0.2.tar` & `ticktick-py-2.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 08:57:16.437296 ticktick-py-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7304 2021-12-27 08:57:16.437296 ticktick-py-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6411 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-27 08:57:16.437296 ticktick-py-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4032 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 08:57:16.433296 ticktick-py-2.0.2/ticktick/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24114 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 08:57:16.433296 ticktick-py-2.0.2/ticktick/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/helpers/hex_color.py
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/helpers/time_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 08:57:16.433296 ticktick-py-2.0.2/ticktick/managers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      375 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/managers/check_logged_in.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/managers/focus.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/managers/habits.py
--rw-r--r--   0 runner    (1001) docker     (121)      261 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/managers/pomo.py
--rw-r--r--   0 runner    (1001) docker     (121)    42705 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/managers/projects.py
--rw-r--r--   0 runner    (1001) docker     (121)      355 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/managers/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    45541 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/managers/tags.py
--rw-r--r--   0 runner    (1001) docker     (121)    52768 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/managers/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)    13108 2021-12-27 08:56:59.000000 ticktick-py-2.0.2/ticktick/oauth2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-27 08:57:16.437296 ticktick-py-2.0.2/ticktick_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7304 2021-12-27 08:57:16.000000 ticktick-py-2.0.2/ticktick_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      669 2021-12-27 08:57:16.000000 ticktick-py-2.0.2/ticktick_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-27 08:57:16.000000 ticktick-py-2.0.2/ticktick_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-12-27 08:57:16.000000 ticktick-py-2.0.2/ticktick_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-27 08:57:16.000000 ticktick-py-2.0.2/ticktick_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:05:17.151407 ticktick-py-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-09 05:05:17.151407 ticktick-py-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 05:05:17.151407 ticktick-py-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:05:17.147407 ticktick-py-2.0.3/ticktick/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24392 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:05:17.147407 ticktick-py-2.0.3/ticktick/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/helpers/hex_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/helpers/time_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:05:17.147407 ticktick-py-2.0.3/ticktick/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/managers/check_logged_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/managers/focus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/managers/habits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/managers/pomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42705 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/managers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/managers/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45541 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/managers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52768 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/managers/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-07-09 05:05:06.000000 ticktick-py-2.0.3/ticktick/oauth2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 05:05:17.151407 ticktick-py-2.0.3/ticktick_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-09 05:05:17.000000 ticktick-py-2.0.3/ticktick_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-09 05:05:17.000000 ticktick-py-2.0.3/ticktick_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 05:05:17.000000 ticktick-py-2.0.3/ticktick_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-09 05:05:17.000000 ticktick-py-2.0.3/ticktick_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 05:05:17.000000 ticktick-py-2.0.3/ticktick_py.egg-info/top_level.txt
```

### Comparing `ticktick-py-2.0.2/LICENSE` & `ticktick-py-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ticktick-py-2.0.2/PKG-INFO` & `ticktick-py-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ticktick-py
-Version: 2.0.2
+Version: 2.0.3
 Summary: Unofficial API for TickTick.com
 Home-page: https://github.com/lazeroffmichael/ticktick-py
 Author: Michael Lazeroff
 Author-email: lazeroffmichael@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -183,8 +182,7 @@
     - Smart List Support
     - Column Creation For Kanban View
 - **Pomo and Focus**  
     - Getting the focus / pomo statistics for your profile  
     - Starting and stopping the focus / pomo timer    
 - **Habits**  
     - Get, create, archive, delete, and complete habits
-
```

### Comparing `ticktick-py-2.0.2/README.md` & `ticktick-py-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ticktick-py-2.0.2/setup.py` & `ticktick-py-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 # Package meta-data.
 NAME = 'ticktick-py'
 DESCRIPTION = 'Unofficial API for TickTick.com'
 URL = 'https://github.com/lazeroffmichael/ticktick-py'
 EMAIL = 'lazeroffmichael@gmail.com'
 AUTHOR = 'Michael Lazeroff'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '2.0.2'
+VERSION = '2.0.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-     'requests==2.26.0', 'pytz==2021.1', 'regex==2021.4.4', 'urllib3==1.26.7'
+    'requests==2.26.0', 'pytz==2021.1', 'regex==2021.4.4', 'urllib3==1.26.7'
 ]
 
 # What packages are optional?
 EXTRAS = {
-     'tests': ['pytest']
+    'tests': ['pytest']
 }
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
 
@@ -76,15 +76,16 @@
         try:
             self.status('Removing previous builds…')
             rmtree(os.path.join(here, 'dist'))
         except OSError:
             pass
 
         self.status('Building Source and Wheel (universal) distribution…')
-        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
+        os.system(
+            '{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
 
         self.status('Uploading the package to PyPI via Twine…')
         os.system('twine upload dist/*')
 
         self.status('Pushing git tags…')
         os.system('git tag v{0}'.format(about['__version__']))
         os.system('git push --tags')
@@ -99,15 +100,16 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    packages=find_packages(
+        exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
```

### Comparing `ticktick-py-2.0.2/ticktick/api.py` & `ticktick-py-2.0.3/ticktick/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import secrets
+
 from ticktick.managers.focus import FocusTimeManager
 from ticktick.managers.habits import HabitManager
 from ticktick.managers.pomo import PomoManager
 from ticktick.managers.projects import ProjectManager
 from ticktick.managers.settings import SettingsManager
 from ticktick.managers.tags import TagsManager
 from ticktick.managers.tasks import TaskManager
@@ -12,16 +14,19 @@
     BASE_URL = 'https://api.ticktick.com/api/v2/'
 
     OPEN_API_BASE_URL = 'https://api.ticktick.com'
 
     INITIAL_BATCH_URL = BASE_URL + 'batch/check/0'
 
     USER_AGENT = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:95.0) Gecko/20100101 Firefox/95.0"
+    X_DEVICE_ = '{"platform":"web","os":"OS X","device":"Firefox 95.0","name":"unofficial api!","version":4531,' \
+                '"id":"6490' + secrets.token_hex(10) + '","channel":"website","campaign":"","websocket":""}'
 
-    HEADERS = {'User-Agent': USER_AGENT}
+    HEADERS = {'User-Agent': USER_AGENT,
+               'x-device': X_DEVICE_}
 
     def __init__(self, username: str, password: str, oauth: OAuth2) -> None:
         """
         Initializes a client session. In order to interact with the API
         a successful login must occur.
 
         Arguments:
```

### Comparing `ticktick-py-2.0.2/ticktick/cache.py` & `ticktick-py-2.0.3/ticktick/cache.py`

 * *Files identical despite different names*

### Comparing `ticktick-py-2.0.2/ticktick/helpers/hex_color.py` & `ticktick-py-2.0.3/ticktick/helpers/hex_color.py`

 * *Files identical despite different names*

### Comparing `ticktick-py-2.0.2/ticktick/helpers/time_methods.py` & `ticktick-py-2.0.3/ticktick/helpers/time_methods.py`

 * *Files identical despite different names*

### Comparing `ticktick-py-2.0.2/ticktick/managers/projects.py` & `ticktick-py-2.0.3/ticktick/managers/projects.py`

 * *Files identical despite different names*

### Comparing `ticktick-py-2.0.2/ticktick/managers/tags.py` & `ticktick-py-2.0.3/ticktick/managers/tags.py`

 * *Files identical despite different names*

### Comparing `ticktick-py-2.0.2/ticktick/managers/tasks.py` & `ticktick-py-2.0.3/ticktick/managers/tasks.py`

 * *Files identical despite different names*

### Comparing `ticktick-py-2.0.2/ticktick/oauth2.py` & `ticktick-py-2.0.3/ticktick/oauth2.py`

 * *Files identical despite different names*

### Comparing `ticktick-py-2.0.2/ticktick_py.egg-info/PKG-INFO` & `ticktick-py-2.0.3/ticktick_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ticktick-py
-Version: 2.0.2
+Version: 2.0.3
 Summary: Unofficial API for TickTick.com
 Home-page: https://github.com/lazeroffmichael/ticktick-py
 Author: Michael Lazeroff
 Author-email: lazeroffmichael@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -183,8 +182,7 @@
     - Smart List Support
     - Column Creation For Kanban View
 - **Pomo and Focus**  
     - Getting the focus / pomo statistics for your profile  
     - Starting and stopping the focus / pomo timer    
 - **Habits**  
     - Get, create, archive, delete, and complete habits
-
```

### Comparing `ticktick-py-2.0.2/ticktick_py.egg-info/SOURCES.txt` & `ticktick-py-2.0.3/ticktick_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

