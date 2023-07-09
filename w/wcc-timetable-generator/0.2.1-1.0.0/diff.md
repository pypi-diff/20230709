# Comparing `tmp/wcc-timetable-generator-0.2.1.tar.gz` & `tmp/wcc-timetable-generator-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcc-timetable-generator-0.2.1.tar", max compression
+gzip compressed data, was "wcc-timetable-generator-1.0.0.tar", max compression
```

## Comparing `wcc-timetable-generator-0.2.1.tar` & `wcc-timetable-generator-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0      751 2023-07-08 17:00:34.566062 wcc-timetable-generator-0.2.1/README.md
--rwxr-xr-x   0        0        0      410 2023-07-08 17:05:12.736741 wcc-timetable-generator-0.2.1/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-07-08 12:02:43.900092 wcc-timetable-generator-0.2.1/wcc_timetable_generator/__init__.py
--rwxr-xr-x   0        0        0      112 2023-07-08 17:09:39.252391 wcc-timetable-generator-0.2.1/wcc_timetable_generator/__main__.py
--rwxr-xr-x   0        0        0     1705 2023-07-08 12:38:40.191165 wcc-timetable-generator-0.2.1/wcc_timetable_generator/algo.py
--rwxr-xr-x   0        0        0        0 2023-07-08 16:45:51.393865 wcc-timetable-generator-0.2.1/wcc_timetable_generator/components/__init__.py
--rwxr-xr-x   0        0        0        0 2023-07-08 16:45:51.394083 wcc-timetable-generator-0.2.1/wcc_timetable_generator/components/entry.py
--rwxr-xr-x   0        0        0       97 2023-07-08 12:11:20.105677 wcc-timetable-generator-0.2.1/wcc_timetable_generator/subject_model.py
--rwxr-xr-x   0        0        0      214 2023-07-08 16:45:51.394562 wcc-timetable-generator-0.2.1/wcc_timetable_generator/timetable.css
--rwxr-xr-x   0        0        0     1289 2023-07-08 16:45:51.394991 wcc-timetable-generator-0.2.1/wcc_timetable_generator/timetable.py
--rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 wcc-timetable-generator-0.2.1/setup.py
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 wcc-timetable-generator-0.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1105 2023-07-09 08:22:35.853994 wcc-timetable-generator-1.0.0/README.md
+-rwxr-xr-x   0        0        0      410 2023-07-09 08:22:59.756232 wcc-timetable-generator-1.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-07-08 12:02:43.900092 wcc-timetable-generator-1.0.0/wcc_timetable_generator/__init__.py
+-rwxr-xr-x   0        0        0      112 2023-07-08 17:09:39.252391 wcc-timetable-generator-1.0.0/wcc_timetable_generator/__main__.py
+-rwxr-xr-x   0        0        0     1705 2023-07-09 08:04:10.954580 wcc-timetable-generator-1.0.0/wcc_timetable_generator/algo.py
+-rwxr-xr-x   0        0        0        0 2023-07-08 16:45:51.393865 wcc-timetable-generator-1.0.0/wcc_timetable_generator/components/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-07-08 16:45:51.394083 wcc-timetable-generator-1.0.0/wcc_timetable_generator/components/entry.py
+-rwxr-xr-x   0        0        0       97 2023-07-08 12:11:20.105677 wcc-timetable-generator-1.0.0/wcc_timetable_generator/subject_model.py
+-rwxr-xr-x   0        0        0      469 2023-07-09 08:03:43.777983 wcc-timetable-generator-1.0.0/wcc_timetable_generator/timetable.css
+-rwxr-xr-x   0        0        0     4057 2023-07-09 08:17:42.664844 wcc-timetable-generator-1.0.0/wcc_timetable_generator/timetable.py
+-rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 wcc-timetable-generator-1.0.0/setup.py
+-rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 wcc-timetable-generator-1.0.0/PKG-INFO
```

### Comparing `wcc-timetable-generator-0.2.1/wcc_timetable_generator/algo.py` & `wcc-timetable-generator-1.0.0/wcc_timetable_generator/algo.py`

 * *Files identical despite different names*

### Comparing `wcc-timetable-generator-0.2.1/setup.py` & `wcc-timetable-generator-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 entry_points = \
 {'console_scripts': ['wcc-timetable-generator = '
                      'wcc_timetable_generator.__main__:main']}
 
 setup_kwargs = {
     'name': 'wcc-timetable-generator',
-    'version': '0.2.1',
+    'version': '1.0.0',
     'description': '',
-    'long_description': "# Timetable 📊\n\n## 📰 Description \nA CLI tool that allow you to generate a timetable for your school or university such that : \n - A subject can't be seen on two consecutive days\n - A subject have a minimum of 2 hours per week and a maximum of 6\n - The timetable is divided in slots of 2 hours\n - The subjects are distributed between monday morning and saturady morning\n - Morning classes begin at 8:30 and end at 12:30\n - Afternoon classes begin at 13:30 and end at 17:30\n\n ## 📦 Installation \n\n ### 💻 Local installation\n\n ### 🌐 Installation with PIP\n ```bash\n pip install wcc-timetable-generator\n ```\n\n## 🖱 Usage\n```bash\ngenerate-timetable\n```\n\n## Roadmap\n- [x] Add the algorithm \n- [ ] Add GUI\n- [ ] Write tests\n- [ ] Publish to PyPI",
+    'long_description': "# Timetable 📊\n\n## 📰 Description \nA CLI tool that allow you to generate a timetable for your school or university such that : \n - A subject can't be seen on two consecutive days\n - A subject have a minimum of 2 hours per week and a maximum of 6\n - The timetable is divided in slots of 2 hours\n - The subjects are distributed between monday morning and saturady morning\n - Morning classes begin at 8:30 and end at 12:30\n - Afternoon classes begin at 13:30 and end at 17:30\n\n ## 📦 Installation \n\n ### 💻 Local installation\n\nTo install this project locally, you first have to clone this repo and install [poetry](https://python-poetry.org/) with pip : `pip install poetry`.\nThen, go to the root directory and run the following commands : \n```bash\npoetry install # install all the necessary dependencies\npoetry run \n\n ### 🌐 Installation with PIP\n ```bash\n pip install wcc-timetable-generator\n ```\n\n## 🖱 Usage\n```bash\nwcc-timetable-generator\n```\n\n## Roadmap\n- [x] Add the algorithm \n- [x] Add GUI-like UI\n- [x] Publish to PyPI\n- [ ] Write tests\n- [ ] Add quit button\n- [ ] Print error messages\n",
     'author': 'Tsierenana Bôtramanagna Gracy',
     'author_email': 'gtsierenana@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `wcc-timetable-generator-0.2.1/PKG-INFO` & `wcc-timetable-generator-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcc-timetable-generator
-Version: 0.2.1
+Version: 1.0.0
 Summary: 
 Author: Tsierenana Bôtramanagna Gracy
 Author-email: gtsierenana@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -23,22 +23,31 @@
  - Morning classes begin at 8:30 and end at 12:30
  - Afternoon classes begin at 13:30 and end at 17:30
 
  ## 📦 Installation 
 
  ### 💻 Local installation
 
+To install this project locally, you first have to clone this repo and install [poetry](https://python-poetry.org/) with pip : `pip install poetry`.
+Then, go to the root directory and run the following commands : 
+```bash
+poetry install # install all the necessary dependencies
+poetry run 
+
  ### 🌐 Installation with PIP
  ```bash
  pip install wcc-timetable-generator
  ```
 
 ## 🖱 Usage
 ```bash
-generate-timetable
+wcc-timetable-generator
 ```
 
 ## Roadmap
 - [x] Add the algorithm 
-- [ ] Add GUI
+- [x] Add GUI-like UI
+- [x] Publish to PyPI
 - [ ] Write tests
-- [ ] Publish to PyPI
+- [ ] Add quit button
+- [ ] Print error messages
+
```

