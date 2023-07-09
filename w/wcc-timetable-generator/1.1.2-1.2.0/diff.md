# Comparing `tmp/wcc-timetable-generator-1.1.2.tar.gz` & `tmp/wcc-timetable-generator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcc-timetable-generator-1.1.2.tar", max compression
+gzip compressed data, was "wcc-timetable-generator-1.2.0.tar", max compression
```

## Comparing `wcc-timetable-generator-1.1.2.tar` & `wcc-timetable-generator-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1333 2023-07-09 09:23:53.784133 wcc-timetable-generator-1.1.2/README.md
--rwxr-xr-x   0        0        0      410 2023-07-09 11:03:18.179166 wcc-timetable-generator-1.1.2/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-07-09 08:40:52.293412 wcc-timetable-generator-1.1.2/wcc_timetable_generator/__init__.py
--rwxr-xr-x   0        0        0      112 2023-07-08 17:09:39.252391 wcc-timetable-generator-1.1.2/wcc_timetable_generator/__main__.py
--rwxr-xr-x   0        0        0     1734 2023-07-09 11:02:23.790668 wcc-timetable-generator-1.1.2/wcc_timetable_generator/algo.py
--rwxr-xr-x   0        0        0        0 2023-07-08 16:45:51.393865 wcc-timetable-generator-1.1.2/wcc_timetable_generator/components/__init__.py
--rwxr-xr-x   0        0        0        0 2023-07-08 16:45:51.394083 wcc-timetable-generator-1.1.2/wcc_timetable_generator/components/entry.py
--rwxr-xr-x   0        0        0       97 2023-07-08 12:11:20.105677 wcc-timetable-generator-1.1.2/wcc_timetable_generator/subject_model.py
--rwxr-xr-x   0        0        0      469 2023-07-09 09:24:38.486582 wcc-timetable-generator-1.1.2/wcc_timetable_generator/timetable.css
--rwxr-xr-x   0        0        0     4067 2023-07-09 10:57:27.407603 wcc-timetable-generator-1.1.2/wcc_timetable_generator/timetable.py
--rw-r--r--   0        0        0     2221 1970-01-01 00:00:00.000000 wcc-timetable-generator-1.1.2/setup.py
--rw-r--r--   0        0        0     1796 1970-01-01 00:00:00.000000 wcc-timetable-generator-1.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1273 2023-07-09 13:24:22.752682 wcc-timetable-generator-1.2.0/README.md
+-rwxr-xr-x   0        0        0      410 2023-07-09 13:26:16.913283 wcc-timetable-generator-1.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-07-09 08:40:52.293412 wcc-timetable-generator-1.2.0/wcc_timetable_generator/__init__.py
+-rwxr-xr-x   0        0        0      112 2023-07-08 17:09:39.252391 wcc-timetable-generator-1.2.0/wcc_timetable_generator/__main__.py
+-rwxr-xr-x   0        0        0     1734 2023-07-09 13:10:09.901632 wcc-timetable-generator-1.2.0/wcc_timetable_generator/algo.py
+-rwxr-xr-x   0        0        0        0 2023-07-08 16:45:51.393865 wcc-timetable-generator-1.2.0/wcc_timetable_generator/components/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-07-08 16:45:51.394083 wcc-timetable-generator-1.2.0/wcc_timetable_generator/components/entry.py
+-rwxr-xr-x   0        0        0       97 2023-07-08 12:11:20.105677 wcc-timetable-generator-1.2.0/wcc_timetable_generator/subject_model.py
+-rwxr-xr-x   0        0        0      560 2023-07-09 12:27:03.581260 wcc-timetable-generator-1.2.0/wcc_timetable_generator/timetable.css
+-rwxr-xr-x   0        0        0     5083 2023-07-09 13:27:10.078518 wcc-timetable-generator-1.2.0/wcc_timetable_generator/timetable.py
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 wcc-timetable-generator-1.2.0/setup.py
+-rw-r--r--   0        0        0     1736 1970-01-01 00:00:00.000000 wcc-timetable-generator-1.2.0/PKG-INFO
```

### Comparing `wcc-timetable-generator-1.1.2/README.md` & `wcc-timetable-generator-1.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Timetable 📊
 
 ## 📰 Description 
 A CLI tool that allow you to generate a timetable for your school or university such that : 
  - A subject can't be seen on two consecutive days
  - A subject have a minimum of 2 hours per week and a maximum of 6
- - The timetable is divided in slots of 2 hours
+ - The timetable is divided in slots of 1 hours
  - The subjects are distributed between monday morning and saturady morning
  - Morning classes begin at 8:30 and end at 12:30
  - Afternoon classes begin at 13:30 and end at 17:30
 
  ## 📦 Installation 
 
  ### 💻 Local installation
@@ -28,16 +28,15 @@
 
 ## 🖱 Usage
 If you installed it with pip, this is how to run the project : 
 ```bash
 wcc-timetable-generator
 ```
 
-## Roadmap
+## ✅ Roadmap
 - [x] Add the algorithm 
 - [x] Add GUI-like UI
 - [x] Publish to PyPI
-- [ ] Fix display and algo so that there are are 1 hour classes
 - [ ] Add an animated GIF as demo to `README.md`
-- [ ] Write tests
-- [ ] Add quit button
-- [ ] Print error messages
+- [x] Write tests
+- [x] Add quit button
+- [x] Print error messages
```

### Comparing `wcc-timetable-generator-1.1.2/wcc_timetable_generator/algo.py` & `wcc-timetable-generator-1.2.0/wcc_timetable_generator/algo.py`

 * *Files identical despite different names*

### Comparing `wcc-timetable-generator-1.1.2/setup.py` & `wcc-timetable-generator-1.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 entry_points = \
 {'console_scripts': ['wcc-timetable-generator = '
                      'wcc_timetable_generator.__main__:main']}
 
 setup_kwargs = {
     'name': 'wcc-timetable-generator',
-    'version': '1.1.2',
+    'version': '1.2.0',
     'description': '',
-    'long_description': "# Timetable 📊\n\n## 📰 Description \nA CLI tool that allow you to generate a timetable for your school or university such that : \n - A subject can't be seen on two consecutive days\n - A subject have a minimum of 2 hours per week and a maximum of 6\n - The timetable is divided in slots of 2 hours\n - The subjects are distributed between monday morning and saturady morning\n - Morning classes begin at 8:30 and end at 12:30\n - Afternoon classes begin at 13:30 and end at 17:30\n\n ## 📦 Installation \n\n ### 💻 Local installation\n\nTo install this project locally, you first have to clone this repo and install [poetry](https://python-poetry.org/) with pip : `pip install poetry`.\nThen, go to the root directory and run the following commands : \n```bash\npoetry install # install all the necessary dependencies\npoetry build\npoetry run python -m wcc_timetable_generator \n```\n\n ### 🌐 Installation with PIP\n ```bash\n pip install wcc-timetable-generator\n ```\n\n## 🖱 Usage\nIf you installed it with pip, this is how to run the project : \n```bash\nwcc-timetable-generator\n```\n\n## Roadmap\n- [x] Add the algorithm \n- [x] Add GUI-like UI\n- [x] Publish to PyPI\n- [ ] Fix display and algo so that there are are 1 hour classes\n- [ ] Add an animated GIF as demo to `README.md`\n- [ ] Write tests\n- [ ] Add quit button\n- [ ] Print error messages\n",
+    'long_description': "# Timetable 📊\n\n## 📰 Description \nA CLI tool that allow you to generate a timetable for your school or university such that : \n - A subject can't be seen on two consecutive days\n - A subject have a minimum of 2 hours per week and a maximum of 6\n - The timetable is divided in slots of 1 hours\n - The subjects are distributed between monday morning and saturady morning\n - Morning classes begin at 8:30 and end at 12:30\n - Afternoon classes begin at 13:30 and end at 17:30\n\n ## 📦 Installation \n\n ### 💻 Local installation\n\nTo install this project locally, you first have to clone this repo and install [poetry](https://python-poetry.org/) with pip : `pip install poetry`.\nThen, go to the root directory and run the following commands : \n```bash\npoetry install # install all the necessary dependencies\npoetry build\npoetry run python -m wcc_timetable_generator \n```\n\n ### 🌐 Installation with PIP\n ```bash\n pip install wcc-timetable-generator\n ```\n\n## 🖱 Usage\nIf you installed it with pip, this is how to run the project : \n```bash\nwcc-timetable-generator\n```\n\n## ✅ Roadmap\n- [x] Add the algorithm \n- [x] Add GUI-like UI\n- [x] Publish to PyPI\n- [ ] Add an animated GIF as demo to `README.md`\n- [x] Write tests\n- [x] Add quit button\n- [x] Print error messages\n",
     'author': 'Tsierenana Bôtramanagna Gracy',
     'author_email': 'gtsierenana@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `wcc-timetable-generator-1.1.2/PKG-INFO` & `wcc-timetable-generator-1.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcc-timetable-generator
-Version: 1.1.2
+Version: 1.2.0
 Summary: 
 Author: Tsierenana Bôtramanagna Gracy
 Author-email: gtsierenana@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,15 +14,15 @@
 
 # Timetable 📊
 
 ## 📰 Description 
 A CLI tool that allow you to generate a timetable for your school or university such that : 
  - A subject can't be seen on two consecutive days
  - A subject have a minimum of 2 hours per week and a maximum of 6
- - The timetable is divided in slots of 2 hours
+ - The timetable is divided in slots of 1 hours
  - The subjects are distributed between monday morning and saturady morning
  - Morning classes begin at 8:30 and end at 12:30
  - Afternoon classes begin at 13:30 and end at 17:30
 
  ## 📦 Installation 
 
  ### 💻 Local installation
@@ -42,17 +42,16 @@
 
 ## 🖱 Usage
 If you installed it with pip, this is how to run the project : 
 ```bash
 wcc-timetable-generator
 ```
 
-## Roadmap
+## ✅ Roadmap
 - [x] Add the algorithm 
 - [x] Add GUI-like UI
 - [x] Publish to PyPI
-- [ ] Fix display and algo so that there are are 1 hour classes
 - [ ] Add an animated GIF as demo to `README.md`
-- [ ] Write tests
-- [ ] Add quit button
-- [ ] Print error messages
+- [x] Write tests
+- [x] Add quit button
+- [x] Print error messages
```

