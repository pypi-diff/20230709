# Comparing `tmp/wcc-timetable-generator-0.2.0.tar.gz` & `tmp/wcc-timetable-generator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcc-timetable-generator-0.2.0.tar", max compression
+gzip compressed data, was "wcc-timetable-generator-0.2.1.tar", max compression
```

## Comparing `wcc-timetable-generator-0.2.0.tar` & `wcc-timetable-generator-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0      669 2023-07-08 12:47:30.471058 wcc-timetable-generator-0.2.0/README.md
--rwxr-xr-x   0        0        0      405 2023-07-08 16:56:58.927434 wcc-timetable-generator-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-07-08 12:02:43.900092 wcc-timetable-generator-0.2.0/wcc_timetable_generator/__init__.py
--rwxr-xr-x   0        0        0       73 2023-07-08 16:55:35.366224 wcc-timetable-generator-0.2.0/wcc_timetable_generator/__main__.py
--rwxr-xr-x   0        0        0     1705 2023-07-08 12:38:40.191165 wcc-timetable-generator-0.2.0/wcc_timetable_generator/algo.py
--rwxr-xr-x   0        0        0        0 2023-07-08 16:45:51.393865 wcc-timetable-generator-0.2.0/wcc_timetable_generator/components/__init__.py
--rwxr-xr-x   0        0        0        0 2023-07-08 16:45:51.394083 wcc-timetable-generator-0.2.0/wcc_timetable_generator/components/entry.py
--rwxr-xr-x   0        0        0       97 2023-07-08 12:11:20.105677 wcc-timetable-generator-0.2.0/wcc_timetable_generator/subject_model.py
--rwxr-xr-x   0        0        0      214 2023-07-08 16:45:51.394562 wcc-timetable-generator-0.2.0/wcc_timetable_generator/timetable.css
--rwxr-xr-x   0        0        0     1289 2023-07-08 16:45:51.394991 wcc-timetable-generator-0.2.0/wcc_timetable_generator/timetable.py
--rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 wcc-timetable-generator-0.2.0/setup.py
--rw-r--r--   0        0        0     1132 1970-01-01 00:00:00.000000 wcc-timetable-generator-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0      751 2023-07-08 17:00:34.566062 wcc-timetable-generator-0.2.1/README.md
+-rwxr-xr-x   0        0        0      410 2023-07-08 17:05:12.736741 wcc-timetable-generator-0.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-07-08 12:02:43.900092 wcc-timetable-generator-0.2.1/wcc_timetable_generator/__init__.py
+-rwxr-xr-x   0        0        0      112 2023-07-08 17:09:39.252391 wcc-timetable-generator-0.2.1/wcc_timetable_generator/__main__.py
+-rwxr-xr-x   0        0        0     1705 2023-07-08 12:38:40.191165 wcc-timetable-generator-0.2.1/wcc_timetable_generator/algo.py
+-rwxr-xr-x   0        0        0        0 2023-07-08 16:45:51.393865 wcc-timetable-generator-0.2.1/wcc_timetable_generator/components/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-07-08 16:45:51.394083 wcc-timetable-generator-0.2.1/wcc_timetable_generator/components/entry.py
+-rwxr-xr-x   0        0        0       97 2023-07-08 12:11:20.105677 wcc-timetable-generator-0.2.1/wcc_timetable_generator/subject_model.py
+-rwxr-xr-x   0        0        0      214 2023-07-08 16:45:51.394562 wcc-timetable-generator-0.2.1/wcc_timetable_generator/timetable.css
+-rwxr-xr-x   0        0        0     1289 2023-07-08 16:45:51.394991 wcc-timetable-generator-0.2.1/wcc_timetable_generator/timetable.py
+-rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 wcc-timetable-generator-0.2.1/setup.py
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 wcc-timetable-generator-0.2.1/PKG-INFO
```

### Comparing `wcc-timetable-generator-0.2.0/README.md` & `wcc-timetable-generator-0.2.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -10,15 +10,21 @@
  - Afternoon classes begin at 13:30 and end at 17:30
 
  ## 📦 Installation 
 
  ### 💻 Local installation
 
  ### 🌐 Installation with PIP
+ ```bash
+ pip install wcc-timetable-generator
+ ```
 
 ## 🖱 Usage
+```bash
+generate-timetable
+```
 
 ## Roadmap
 - [x] Add the algorithm 
 - [ ] Add GUI
 - [ ] Write tests
 - [ ] Publish to PyPI
```

### Comparing `wcc-timetable-generator-0.2.0/wcc_timetable_generator/algo.py` & `wcc-timetable-generator-0.2.1/wcc_timetable_generator/algo.py`

 * *Files identical despite different names*

### Comparing `wcc-timetable-generator-0.2.0/wcc_timetable_generator/timetable.py` & `wcc-timetable-generator-0.2.1/wcc_timetable_generator/timetable.py`

 * *Files identical despite different names*

### Comparing `wcc-timetable-generator-0.2.0/setup.py` & `wcc-timetable-generator-0.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['textual>=0.29.0,<0.30.0']
 
 entry_points = \
-{'console_scripts': ['generate-timetable = '
+{'console_scripts': ['wcc-timetable-generator = '
                      'wcc_timetable_generator.__main__:main']}
 
 setup_kwargs = {
     'name': 'wcc-timetable-generator',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': '',
-    'long_description': "# Timetable 📊\n\n## 📰 Description \nA CLI tool that allow you to generate a timetable for your school or university such that : \n - A subject can't be seen on two consecutive days\n - A subject have a minimum of 2 hours per week and a maximum of 6\n - The timetable is divided in slots of 2 hours\n - The subjects are distributed between monday morning and saturady morning\n - Morning classes begin at 8:30 and end at 12:30\n - Afternoon classes begin at 13:30 and end at 17:30\n\n ## 📦 Installation \n\n ### 💻 Local installation\n\n ### 🌐 Installation with PIP\n\n## 🖱 Usage\n\n## Roadmap\n- [x] Add the algorithm \n- [ ] Add GUI\n- [ ] Write tests\n- [ ] Publish to PyPI",
+    'long_description': "# Timetable 📊\n\n## 📰 Description \nA CLI tool that allow you to generate a timetable for your school or university such that : \n - A subject can't be seen on two consecutive days\n - A subject have a minimum of 2 hours per week and a maximum of 6\n - The timetable is divided in slots of 2 hours\n - The subjects are distributed between monday morning and saturady morning\n - Morning classes begin at 8:30 and end at 12:30\n - Afternoon classes begin at 13:30 and end at 17:30\n\n ## 📦 Installation \n\n ### 💻 Local installation\n\n ### 🌐 Installation with PIP\n ```bash\n pip install wcc-timetable-generator\n ```\n\n## 🖱 Usage\n```bash\ngenerate-timetable\n```\n\n## Roadmap\n- [x] Add the algorithm \n- [ ] Add GUI\n- [ ] Write tests\n- [ ] Publish to PyPI",
     'author': 'Tsierenana Bôtramanagna Gracy',
     'author_email': 'gtsierenana@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `wcc-timetable-generator-0.2.0/PKG-INFO` & `wcc-timetable-generator-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcc-timetable-generator
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Tsierenana Bôtramanagna Gracy
 Author-email: gtsierenana@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -24,15 +24,21 @@
  - Afternoon classes begin at 13:30 and end at 17:30
 
  ## 📦 Installation 
 
  ### 💻 Local installation
 
  ### 🌐 Installation with PIP
+ ```bash
+ pip install wcc-timetable-generator
+ ```
 
 ## 🖱 Usage
+```bash
+generate-timetable
+```
 
 ## Roadmap
 - [x] Add the algorithm 
 - [ ] Add GUI
 - [ ] Write tests
 - [ ] Publish to PyPI
```

