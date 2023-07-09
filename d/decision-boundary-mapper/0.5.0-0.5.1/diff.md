# Comparing `tmp/decision-boundary-mapper-0.5.0.tar.gz` & `tmp/decision-boundary-mapper-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decision-boundary-mapper-0.5.0.tar", last modified: Sat May 20 06:03:27 2023, max compression
+gzip compressed data, was "decision-boundary-mapper-0.5.1.tar", last modified: Sun Jul  9 17:30:53 2023, max compression
```

## Comparing `decision-boundary-mapper-0.5.0.tar` & `decision-boundary-mapper-0.5.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.718901 decision-boundary-mapper-0.5.0/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1071 2023-03-30 08:17:56.000000 decision-boundary-mapper-0.5.0/LICENSE.txt
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     3730 2023-05-20 06:03:27.719112 decision-boundary-mapper-0.5.0/PKG-INFO
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     2818 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/README.md
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      107 2023-05-20 06:03:27.719660 decision-boundary-mapper-0.5.0/setup.cfg
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1737 2023-05-20 06:03:22.000000 decision-boundary-mapper-0.5.0/setup.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.703022 decision-boundary-mapper-0.5.0/src/
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.705730 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.708838 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)    43104 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/AbstractDBM.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     5735 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/AbstractNN.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.710153 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)    12647 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/DBM.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     5108 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/NNInv.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      600 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/__init__.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1519 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/projections.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.711575 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     7062 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/Autoencoder.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     9850 2023-05-19 14:34:10.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/SDBM.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     7841 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/SSNP.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      618 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/__init__.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      753 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/__init__.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)    13834 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/tools.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.714072 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)    28700 2023-05-19 13:46:27.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/DBMPlotterController.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)    24678 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/DBMPlotterGUI.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)    20600 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/GUI.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)    13781 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/GUIController.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      641 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/__init__.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1906 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/utils.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.715712 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     2872 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/Logger.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     3096 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/LoggerGUI.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1006 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/LoggerInterface.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1794 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/LoggerModel.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      721 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/__init__.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      826 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/__init__.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.717074 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     6454 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/DBM_usage_example.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     4718 2023-05-19 14:34:53.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/SDBM_usage_example.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      726 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/__init__.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     3279 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/utils.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.718595 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/utils/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      753 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/utils/__init__.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1351 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/utils/config.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     4123 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/utils/dataReader.py
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1296 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/utils/tools.py
-drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-05-20 06:03:27.707428 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     3730 2023-05-20 06:03:27.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/PKG-INFO
--rw-r--r--   0 cristiangrosu   (501) staff       (20)     1842 2023-05-20 06:03:27.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 cristiangrosu   (501) staff       (20)        1 2023-05-20 06:03:27.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 cristiangrosu   (501) staff       (20)      144 2023-05-20 06:03:27.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/requires.txt
--rw-r--r--   0 cristiangrosu   (501) staff       (20)       25 2023-05-20 06:03:27.000000 decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.796658 decision-boundary-mapper-0.5.1/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1071 2023-03-30 08:17:56.000000 decision-boundary-mapper-0.5.1/LICENSE.txt
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     3730 2023-07-09 17:30:53.797084 decision-boundary-mapper-0.5.1/PKG-INFO
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     2818 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/README.md
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      107 2023-07-09 17:30:53.797559 decision-boundary-mapper-0.5.1/setup.cfg
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1737 2023-07-09 17:30:46.000000 decision-boundary-mapper-0.5.1/setup.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.782154 decision-boundary-mapper-0.5.1/src/
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.785012 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.788188 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    51902 2023-07-09 08:46:17.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/AbstractDBM.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     5735 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/AbstractNN.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.789394 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    12647 2023-07-09 08:44:46.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/DBM.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     5108 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/NNInv.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      600 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1519 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/projections.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.790573 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     7062 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/Autoencoder.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     9850 2023-05-19 14:34:10.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/SDBM.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     7841 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/SSNP.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      618 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      753 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    13280 2023-05-29 12:45:43.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/tools.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.792638 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    28939 2023-07-09 11:12:41.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/DBMPlotterController.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    25700 2023-07-09 11:13:27.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/DBMPlotterGUI.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    20600 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/GUI.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)    13781 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/GUIController.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      641 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1906 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/utils.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.794093 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     2872 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/Logger.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     3096 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/LoggerGUI.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1006 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/LoggerInterface.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1794 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/LoggerModel.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      721 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      826 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/__init__.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.795258 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     6454 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/DBM_usage_example.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     4718 2023-05-19 14:34:53.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/SDBM_usage_example.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      726 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     3279 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/utils.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.796402 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      753 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/__init__.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1351 2023-05-20 06:01:02.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/config.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     4123 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/dataReader.py
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1296 2023-05-19 10:01:25.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/tools.py
+drwxr-xr-x   0 cristiangrosu   (501) staff       (20)        0 2023-07-09 17:30:53.786795 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     3730 2023-07-09 17:30:53.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)     1842 2023-07-09 17:30:53.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)        1 2023-07-09 17:30:53.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)      144 2023-07-09 17:30:53.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/requires.txt
+-rw-r--r--   0 cristiangrosu   (501) staff       (20)       25 2023-07-09 17:30:53.000000 decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/top_level.txt
```

### Comparing `decision-boundary-mapper-0.5.0/LICENSE.txt` & `decision-boundary-mapper-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/PKG-INFO` & `decision-boundary-mapper-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decision-boundary-mapper
-Version: 0.5.0
+Version: 0.5.1
 Summary: A tool for visualizing the decision boundary of a machine learning model.
 Home-page: https://github.com/cristi2019255/MasterThesis2023
 Author: Cristian Grosu
 Author-email: c.grosu@students.uu.nl
 License: MIT
 Description: # Short Description
```

### Comparing `decision-boundary-mapper-0.5.0/README.md` & `decision-boundary-mapper-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/setup.py` & `decision-boundary-mapper-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # remove the old documentation folder
 rmtree('docs', ignore_errors=True)
 
 os.system("pdoc --html src/decision_boundary_mapper -o docs")
 
 setup(
     name='decision-boundary-mapper',
-    version='0.5.0',
+    version='0.5.1',
     license='MIT',
     author="Cristian Grosu",
     author_email='c.grosu@students.uu.nl',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/cristi2019255/MasterThesis2023',
     keywords='Decision Boundary Mapper',
```

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/AbstractDBM.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/AbstractDBM.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,29 +24,29 @@
 from enum import Enum
 
 from .tools import binary_split, generate_windows, get_confidence_based_split, get_inv_proj_error, get_nd_indices_parallel, euclidean, get_pixel_priority, get_proj_error_parallel, get_projection_errors_using_inverse_projection, get_tasks_with_same_priority, get_window_borders
 from .AbstractNN import AbstractNN
 from ..utils import track_time_wrapper, INVERSE_PROJECTION_ERRORS_FILE, PROJECTION_ERRORS_INTERPOLATED_FILE, PROJECTION_ERRORS_INVERSE_PROJECTION_FILE
 from ..Logger import Logger, LoggerInterface
 
-DBM_DEFAULT_CHUNK_SIZE = 30000
+DBM_DEFAULT_CHUNK_SIZE = 10000
 DBM_DEFAULT_RESOLUTION = 256
 DEFAULT_WINDOW_SIZE = 8
 DBM_IMAGE_NAME = "boundary_map"
 DBM_CONFIDENCE_IMAGE_NAME = "boundary_map_confidence"
 
 PROJECTION_ERRORS_NEIGHBORS_NUMBER = 10
 
 time_tracker_console = Logger(name="Decision Boundary Mapper - DBM", info_color="cyan", show_init=False)
 
 class FAST_DBM_STRATEGIES(Enum):
     NONE = "none"
     BINARY = "binary_split"
     CONFIDENCE_BASED = "confidence_split"
-    HYBRID = "hybrid_split"
+    CONFIDENCE_INTERPOLATION = "confidence_interpolation"
 
     @classmethod
     def list(cls):
         return list(map(lambda c: c.value, cls))
 
 class AbstractDBM:
     """ 
@@ -84,15 +84,17 @@
 
         self.console.log("Loaded classifier: " + classifier.name + "")
         self.classifier = classifier
         self.neural_network: AbstractNN
         self.X2d: np.ndarray
         self.Xnd: np.ndarray
         self.resolution: int
-
+        # a dictionary that maps the resolution to the best block resolution for the confidence interpolation strategy in fast decoding
+        self.resolution_to_blocks_resolution_map = {} 
+        
     def refit_classifier(self, Xnd: np.ndarray, Y: np.ndarray, save_folder: str, epochs: int = 2, batch_size: int = 32):
         """ 
         Refits the classifier on the given data set.
 
         Args:             
             Xnd (np.ndarray): The data set
             Y (np.ndarray): The new labels
@@ -154,27 +156,27 @@
             img_confidence (np.ndarray): The DBM confidence image
         """
         save_img_path = os.path.join(load_folder, DBM_IMAGE_NAME)
         save_img_confidence_path = os.path.join(load_folder, DBM_CONFIDENCE_IMAGE_NAME)
 
         match fast_decoding_strategy:
             case FAST_DBM_STRATEGIES.NONE:
-                img, img_confidence = self._get_img_dbm_(resolution)
+                img, img_confidence, _ = self._get_img_dbm_(resolution)
             case FAST_DBM_STRATEGIES.BINARY:
                 save_img_path += f"_fast_{FAST_DBM_STRATEGIES.BINARY.value}"
                 save_img_confidence_path += f"_fast_{FAST_DBM_STRATEGIES.BINARY.value}"
-                img, img_confidence = self._get_img_dbm_fast_(resolution)
+                img, img_confidence, _ = self._get_img_dbm_fast_(resolution)
             case FAST_DBM_STRATEGIES.CONFIDENCE_BASED:
                 save_img_path += f"_fast_{FAST_DBM_STRATEGIES.CONFIDENCE_BASED.value}"
                 save_img_confidence_path += f"_fast_{FAST_DBM_STRATEGIES.CONFIDENCE_BASED.value}"
-                img, img_confidence = self._get_img_dbm_fast_confidences_strategy(resolution)
-            case FAST_DBM_STRATEGIES.HYBRID:
-                save_img_path += f"_fast_{FAST_DBM_STRATEGIES.HYBRID.value}"
-                save_img_confidence_path += f"_fast_{FAST_DBM_STRATEGIES.HYBRID.value}"
-                img, img_confidence = self._get_img_dbm_fast_hybrid_strategy(resolution)
+                img, img_confidence, _ = self._get_img_dbm_fast_confidences_strategy(resolution)
+            case FAST_DBM_STRATEGIES.CONFIDENCE_INTERPOLATION:
+                save_img_path += f"_fast_{FAST_DBM_STRATEGIES.CONFIDENCE_INTERPOLATION.value}"
+                save_img_confidence_path += f"_fast_{FAST_DBM_STRATEGIES.CONFIDENCE_INTERPOLATION.value}"
+                img, img_confidence, _ = self._get_img_dbm_fast_confidence_interpolation_strategy(resolution)
 
         with open(f"{save_img_path}.npy", 'wb') as f:
             np.save(f, img)  # type: ignore
         with open(f"{save_img_confidence_path}.npy", 'wb') as f:
             np.save(f, img_confidence)  # type: ignore
 
         return img, img_confidence  # type: ignore
@@ -210,41 +212,44 @@
             predicted_labels, predicted_confidence, _ = self._predict2dspace_(space2d_chunk)
             img = np.concatenate((img, predicted_labels))
             img_confidence = np.concatenate((img_confidence, predicted_confidence))
 
         img = img.reshape((resolution, resolution))
         img_confidence = img_confidence.reshape((resolution, resolution))
 
-        return (img, img_confidence)
+        return img, img_confidence, None
 
     @track_time_wrapper(logger=time_tracker_console)
-    def _get_img_dbm_fast_(self, resolution: int, computational_budget=None, interpolation_method: str = "linear", window_size: int = DEFAULT_WINDOW_SIZE):
+    def _get_img_dbm_fast_(self, resolution: int, computational_budget=None, interpolation_method: str = "linear", initial_resolution: int | None = None):
         """
         This function generates the 2D image of the boundary map. It uses a fast algorithm to generate the image.
 
         Args:
             resolution (int): the resolution of the 2D image to be generated
             computational_budget (int, optional): The computational budget to be used. Defaults to None.
             interpolation_method (str, optional): The interpolation method to be used for the interpolation of sparse data generated by the fast algorithm.
                                                   Defaults to "linear". The options are: "nearest", "linear", "cubic"
-            window_size (int, optional): The window size to be used. Defaults to 8.
+            initial_resolution (int, optional): The initial number of blocks. Defaults to None, meaning that the initial resolution is taken as resolution // DEFAULT_WINDOW_SIZE
 
         Returns:
             img, img_confidence: The 2D image of the boundary map and a image with the confidence for each pixel
-            spaceNd: The nD space points
+            confidence_map: The confidence map that  constructs the confidence image
         Example:
-            >>> img, img_confidence = self._get_img_dbm_fast_(resolution=32, computational_budget=1000)
+            >>> img, img_confidence, confidence_map = self._get_img_dbm_fast_(resolution=32, computational_budget=1000)
         """
-        assert(window_size < resolution)
-        assert(window_size > 0)
-        assert(int(window_size) == window_size)
+        if initial_resolution is None:
+            initial_resolution = resolution // DEFAULT_WINDOW_SIZE
+            
+        assert(initial_resolution > 0)
+        assert(int(initial_resolution) == initial_resolution)    
+        assert(initial_resolution < resolution)
         # ------------------------------------------------------------
         INITIAL_COMPUTATIONAL_BUDGET = computational_budget = resolution * resolution if computational_budget is None else computational_budget
 
-        indexes, sizes, labels, computational_budget, img, confidence_map = self._fill_initial_windows_(window_size=window_size, 
+        indexes, sizes, labels, computational_budget, img, confidence_map = self._fill_initial_windows_(initial_resolution=initial_resolution, 
                                                                                                         resolution=resolution, 
                                                                                                         computational_budget=computational_budget,
                                                                                                         confidence_interpolation_method=interpolation_method)
            
         # analyze the initial points and generate the priority queue
         priority_queue = PriorityQueue()
         priority_queue = self._update_priority_queue_(priority_queue, img, indexes, sizes, labels)
@@ -312,46 +317,49 @@
         self.console.log(f"Items left in the priority queue: {priority_queue.qsize()}")
 
         # generating the confidence image using interpolation based on the confidence map
         img_confidence = self._generate_interpolated_image_(sparse_map=confidence_map,
                                                             resolution=resolution,
                                                             method=interpolation_method).T
 
-        return img, img_confidence
+        return img, img_confidence, confidence_map
 
     @track_time_wrapper(logger=time_tracker_console)
-    def _get_img_dbm_fast_confidences_strategy(self, resolution: int, computational_budget=None, interpolation_method: str = "linear", window_size: int = DEFAULT_WINDOW_SIZE):
+    def _get_img_dbm_fast_confidences_strategy(self, resolution: int, computational_budget=None, interpolation_method: str = "linear", initial_resolution : int | None = None):
         """
         This function generates the 2D image of the boundary map. It uses a fast algorithm that uses a confidence based strategy to generate the image.
 
         Args:
             resolution (int): the resolution of the 2D image to be generated
             computational_budget (int, optional): The computational budget to be used. Defaults to None.
             interpolation_method (str, optional): The interpolation method to be used for the interpolation of sparse data generated by the fast algorithm.
                                                   Defaults to "linear". The options are: "nearest", "linear", "cubic"
-            window_size (int, optional): The window size to be used. Defaults to 8.
+            initial_resolution (int, optional): The initial number of blocks. Defaults to None, meaning that the initial resolution is taken as resolution // DEFAULT_WINDOW_SIZE
 
         Returns:
             img, img_confidence: The 2D image of the boundary map and a image with the confidence for each pixel
-            spaceNd: The nD space points
+            confidence_map: The confidence map that  constructs the confidence image
         Example:
-            >>> img, img_confidence = self._get_img_dbm_fast_confidences_strategy(resolution=32, computational_budget=1000)
+            >>> img, img_confidence, confidence_map = self._get_img_dbm_fast_confidences_strategy(resolution=32, computational_budget=1000)
         """
-        assert(window_size < resolution)
-        assert(window_size > 0)
-        assert(int(window_size) == window_size)
+        if initial_resolution is None:
+            initial_resolution = resolution // DEFAULT_WINDOW_SIZE
+        
+        assert(initial_resolution > 0)
+        assert(int(initial_resolution) == initial_resolution)    
+        assert(initial_resolution < resolution)
         # ------------------------------------------------------------
         # Setting the initial parameters
         INITIAL_COMPUTATIONAL_BUDGET = computational_budget = resolution * resolution if computational_budget is None else computational_budget
 
-        initial_resolution = resolution // window_size
         img = np.zeros((resolution, resolution), dtype=np.int16)
         img_indexes = np.zeros((resolution, resolution, 2), dtype=np.int16)
         # ------------------------------------------------------------
 
+        window_size = resolution // initial_resolution
         # ------------------------------------------------------------
         # generate the initial points
         indexes, sizes, initial_resolution = generate_windows(window_size, initial_resolution=initial_resolution, resolution=resolution)
         space2d = np.array(indexes) / resolution  
         predicted_labels, predicted_confidence, predicted_confidences = self._predict2dspace_(space2d)
         pseudo_conf_img = np.zeros((resolution, resolution, len(predicted_confidences[0])))
 
@@ -378,15 +386,15 @@
         # -------------------------------------
         # start the iterative process of filling the image
         self.console.log(f"Starting the iterative process of refining windows...")
 
         iteration = 0
         while computational_budget > 0 and not priority_queue.empty():
             iteration += 1
-            print("Priority queue size: ", priority_queue.qsize())
+            # print("Priority queue size: ", priority_queue.qsize())
             # take the highest priority tasks
             items = get_tasks_with_same_priority(priority_queue)
 
             space2d, indices, window_sizes = [], [], []
             single_points_space, single_points_indices = [], []
 
             for (w, h, i, j) in items:
@@ -447,41 +455,46 @@
         self.console.log(f"Items left in the priority queue: {priority_queue.qsize()}")
 
         # generating the confidence image using interpolation based on the confidence map
         img_confidence = self._generate_interpolated_image_(sparse_map=confidence_map,
                                                             resolution=resolution,
                                                             method=interpolation_method).T
 
-        return img, img_confidence
+        return img, img_confidence, confidence_map
 
     @track_time_wrapper(logger=time_tracker_console)
-    def _get_img_dbm_fast_hybrid_strategy(self, resolution: int, computational_budget=None, interpolation_method: str = "linear", window_size: int = DEFAULT_WINDOW_SIZE):
+    def _get_img_dbm_fast_hybrid_strategy(self, resolution: int, computational_budget=None, interpolation_method: str = "linear", initial_resolution: int | None = None):
         """
         This function generates the 2D image of the boundary map. It uses a fast algorithm that uses a binary split based strategy to generate the image.
 
         Args:
             resolution (int): the resolution of the 2D image to be generated
             computational_budget (int, optional): The computational budget to be used. Defaults to None.
             interpolation_method (str, optional): The interpolation method to be used for the interpolation of sparse data generated by the fast algorithm.
                                                   Defaults to "linear". The options are: "nearest", "linear", "cubic"
-            window_size (int, optional): The window size to be used. Defaults to 8.
+            initial_resolution (int, optional): The initial number of blocks. Defaults to None, meaning that the initial resolution is taken as resolution // DEFAULT_WINDOW_SIZE
+
         Returns:
             img, img_confidence: The 2D image of the boundary map and a image with the confidence for each pixel
-            spaceNd: The nD space points
+            confidence_map: The confidence map that  constructs the confidence image
         Example:
-            >>> img, img_confidence = self._get_img_dbm_fast_hybrid_strategy(resolution=32, computational_budget=1000)
+            >>> img, img_confidence, confidence_map = self._get_img_dbm_fast_hybrid_strategy(resolution=32, computational_budget=1000)
         """
-        assert(window_size < resolution)
-        assert(window_size > 0)
-        assert(int(window_size) == window_size)
+        if initial_resolution is None:
+            initial_resolution = resolution // DEFAULT_WINDOW_SIZE
+        
+        assert(initial_resolution > 0)
+        assert(int(initial_resolution) == initial_resolution)    
+        assert(initial_resolution < resolution)
+
         # ------------------------------------------------------------
         # Setting the initial parameters
         INITIAL_COMPUTATIONAL_BUDGET = computational_budget = resolution * resolution if computational_budget is None else computational_budget
 
-        indexes, sizes, labels, computational_budget, img, confidence_map = self._fill_initial_windows_(window_size=window_size, 
+        indexes, sizes, labels, computational_budget, img, confidence_map = self._fill_initial_windows_(initial_resolution=initial_resolution, 
                                                                                                         resolution=resolution, 
                                                                                                         computational_budget=computational_budget,
                                                                                                         confidence_interpolation_method=interpolation_method)
 
         # analyze the initial windows
         items_to_decode = []
         for index in range(len(indexes)):
@@ -523,19 +536,150 @@
         self.console.log(f"Finished decoding the image, initial computational budget: {INITIAL_COMPUTATIONAL_BUDGET} computational budget left: {computational_budget}")
 
         # generating the confidence image using interpolation based on the confidence map
         img_confidence = self._generate_interpolated_image_(sparse_map=confidence_map,
                                                             resolution=resolution,
                                                             method=interpolation_method).T
 
-        return img, img_confidence
+        return img, img_confidence, confidence_map
+    
+    @track_time_wrapper(logger=time_tracker_console)
+    def _get_img_dbm_fast_confidence_interpolation_strategy(self, resolution: int, interpolation_method: str = "cubic", initial_resolution: int | None = None):
+        """
+        This function generates the 2D image of the boundary map. It uses a fast algorithm that uses a confidence interpolation strategy.
+        Args:
+            resolution (int): the resolution of the 2D image to be generated
+            interpolation_method (str, optional): The interpolation method to be used for the interpolation of sparse data generated by the fast algorithm.
+                                                  Defaults to "cubic". The options are: "nearest", "linear", "cubic"
+            initial_resolution (int, optional): The initial number of blocks. Defaults to None, meaning that the best initial resolution is searched before computing the dbm.
+        Returns:
+            img, img_confidence , _: The 2D image of the boundary map and a image with the confidence for each pixel
+        Example:
+            >>> img, img_confidence, _ = self._get_img_dbm_fast_confidence_interpolation_strategy(resolution=32)
+        """
+        
+        img_confidence = np.zeros((resolution, resolution, 1))
+        
+        # check if the block resolution is provided by the user
+        if initial_resolution is not None:
+            assert(initial_resolution < resolution)
+            assert(initial_resolution > 0)
+            assert(int(initial_resolution) == initial_resolution)
+            img_confidence = self.__compute_confidence_interpolation__(initial_resolution, resolution, interpolation_method)
+        # check if the block resolution for this resolution was already computed
+        elif resolution in self.resolution_to_blocks_resolution_map:
+            initial_resolution = self.resolution_to_blocks_resolution_map[resolution]
+            img_confidence = self.__compute_confidence_interpolation__(initial_resolution, resolution, interpolation_method)
+        # get the best block resolution for this resolution otherwise
+        else:    
+            self.console.log("Finding the necessary number of initial blocks for interpolation")
+            initial_resolution = 2
+            CONFIDENCE_EPSILON = 0.01
+            old_img_confidence = None
+            
+            while initial_resolution < resolution:
+                self.console.log(f"Computing confidence map for blocks resolution: {initial_resolution}x{initial_resolution}")
+                img_confidence = self.__compute_confidence_interpolation__(initial_resolution, resolution, interpolation_method)
+            
+                if old_img_confidence is None:
+                    old_img_confidence = np.copy(img_confidence)
+                    initial_resolution *= 2
+                    continue
+                
+                if np.mean(np.abs(img_confidence - old_img_confidence)) < CONFIDENCE_EPSILON:
+                    self.resolution_to_blocks_resolution_map[resolution] = initial_resolution
+                    self.console.log(f"Using blocks resolution: {initial_resolution}x{initial_resolution}")                  
+                    break 
+                
+                initial_resolution *= 2
+                old_img_confidence = np.copy(img_confidence)
+            
+            
+        img = np.zeros((resolution, resolution))
+        confidence_img = np.zeros((resolution, resolution))
+        self.console.log(f"Filling the decision boundary map using the interpolated confidence map")
+        for (i, j) in np.ndindex(img.shape):
+            confidences = img_confidence[i, j]
+            label = np.argmax(confidences)
+            confidence_img[i, j] =  np.max(confidences)
+            img[i, j] = int(label)
+        
+        # apply brute force at the boundaries to get less errors
+        """
+        pseudo_decision_boundary_indexes = []
+        self.console.log("Finding the pseudo boundaries")
+        for (i, j) in np.ndindex(img.shape):
+            label = img[i, j]
+            if i - 1 >= 0 and img[i - 1, j] != label:
+                pseudo_decision_boundary_indexes.append((i, j))
+                continue
+            if i + 1 < resolution and img[i + 1, j] != label:
+                pseudo_decision_boundary_indexes.append((i, j))
+                continue
+            if j - 1 >= 0 and img[i, j - 1] != label:
+                pseudo_decision_boundary_indexes.append((i, j))
+                continue
+            if j + 1 < resolution and img[i, j + 1] != label:
+                pseudo_decision_boundary_indexes.append((i, j))
+                continue
+        
+        
+        self.console.log(f"Computing the pseudo-decision boundary, {len(pseudo_decision_boundary_indexes)} points.")
+        if len(pseudo_decision_boundary_indexes) == 0:
+            return img, confidence_img, None   
+        space2d = np.array(pseudo_decision_boundary_indexes) / resolution
+        predicted_labels, predicted_confidence, _ = self._predict2dspace_(space2d)
+        # fill the actual predicted labels and confidences
+        for (i, j), label, conf in zip(pseudo_decision_boundary_indexes, predicted_labels, predicted_confidence):
+            img[i, j] = int(label)
+            confidence_img[i, j] = conf
+        """
+
+        return img, confidence_img, None
+
+    def __compute_confidence_interpolation__(self, blocks_resolution, resolution, interpolation_method):
+        window_size = resolution // blocks_resolution
+        
+        # generate the initial points
+        indexes, _, initial_resolution = generate_windows(window_size, initial_resolution=blocks_resolution, resolution=resolution)
+        # creating an artificial border for the 2D confidence image
+            
+        confidence_map = []
+            
+        if interpolation_method != "nearest":
+            border_indices = [(i * window_size + window_size / 2 - 0.5, 0) for i in range(initial_resolution)] + \
+                    [(i * window_size + window_size / 2 - 0.5, resolution - 1) for i in range(initial_resolution)] + \
+                    [(0, i * window_size + window_size / 2 - 0.5) for i in range(-1, initial_resolution + 1)] + \
+                    [(resolution - 1, i * window_size + window_size / 2 - 0.5) for i in range(-1, initial_resolution + 1)]
+
+            space2d_border = np.array(border_indices) / resolution
+            _, _, confidences = self._predict2dspace_(space2d_border)
+            confidence_map = [(i, j, confs) for (i, j), confs in zip(border_indices, confidences)]
+            
+        space2d = np.array(indexes) / resolution  
+        _, _, predicted_confidences = self._predict2dspace_(space2d)
+        
+        for (i,j), confs in zip(indexes, predicted_confidences):
+            confidence_map.append((i, j, confs)) # type: ignore
+
+        num_classes = len(predicted_confidences[0])
+            
+        # interpolate the confidence map for each class
+        img_confidence = np.zeros((resolution, resolution, num_classes))
+        for k in range(num_classes):
+            confidence_map_class = [(i, j, confs[k]) for (i, j, confs) in confidence_map]
+            img_confidence[:, :, k] = self._generate_interpolated_image_(sparse_map=confidence_map_class,
+                                                                                resolution=resolution,
+                                                                                method=interpolation_method).T
+        
+        return img_confidence
 
-    def _fill_initial_windows_(self, window_size: int, resolution: int, computational_budget: int, confidence_interpolation_method: str = "linear"):
+    def _fill_initial_windows_(self, initial_resolution: int, resolution: int, computational_budget: int, confidence_interpolation_method: str = "linear"):
         
-        initial_resolution = resolution // window_size
+        window_size = resolution // initial_resolution
         img = np.zeros((resolution, resolution), dtype=np.int16)
         # ------------------------------------------------------------
 
         # ------------------------------------------------------------
         # generate the initial points
         indexes, sizes, initial_resolution = generate_windows(window_size, initial_resolution=initial_resolution, resolution=resolution)
         # creating an artificial border for the 2D confidence image
@@ -657,15 +801,15 @@
             Z.append(z)
         X, Y, Z = np.array(X), np.array(Y), np.array(Z)
         xi = np.linspace(0, resolution-1, resolution)
         yi = np.linspace(0, resolution-1, resolution)
         return interpolate.griddata((X, Y), Z, (xi[None, :], yi[:, None]), method=method)
 
     @track_time_wrapper(logger=time_tracker_console)
-    def _generate_interpolation_rbf_(self, sparse_map, resolution, function='linear'):
+    def _generate_interpolation_rbf_(self, sparse_map, resolution:int, method:str='linear'):
         """A private method that uses interpolation to generate the values for the 2D space image
            The sparse map is a list of tuples (x, y, data) where x, y and data are in the range [0, 1]
 
         Args:
             sparse_map (np.ndarray): a list of tuples (x, y, data) where x and y are the coordinates of the pixel and data is the data value
             resolution (int): the resolution of the image we want to generate (the image will be a square image)
             function (str, optional): Defaults to 'euclidean'.
@@ -674,15 +818,15 @@
             "Computing the interpolated image using RBF interpolation...")
         X, Y, Z = [], [], []
         for (x, y, z) in sparse_map:
             X.append(x)
             Y.append(y)
             Z.append(z)
 
-        rbf = interpolate.Rbf(X, Y, Z, function=function)
+        rbf = interpolate.Rbf(X, Y, Z, function=method)
         ti = np.linspace(0, 1, resolution)
         xx, yy = np.meshgrid(ti, ti)
         
         """
             using dask to parallelize the computation of the rbf function
             the rbf function is applied to each pixel of the image
             the image is divided into chunks and each chunk is processed in parallel
@@ -791,15 +935,15 @@
         self.console.log("Finished computing the nD distance indices")
 
         sparse_map = []
         for k in range(len(X2d)):
             x, y = X2d[k]
             sparse_map.append((x, y, get_proj_error_parallel(indices_source[k], indices_embedded[k], k=K)))
 
-        errors = self._generate_interpolation_rbf_(sparse_map, resolution, function='linear').T
+        errors = self._generate_interpolation_rbf_(sparse_map, resolution, method='linear').T
 
         # resize the errors in range [0,1]
         errors = (errors - errors.min()) / (errors.max() - errors.min())
 
         return errors
 
     @track_time_wrapper(logger=time_tracker_console)
```

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/AbstractNN.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/AbstractNN.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/DBM.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/DBM.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/NNInv.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/NNInv.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/__init__.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/DBM/projections.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/DBM/projections.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/Autoencoder.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/Autoencoder.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/SDBM.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/SDBM.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/SSNP.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/SSNP.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/SDBM/__init__.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/SDBM/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/__init__.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/DBM/tools.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/DBM/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -278,30 +278,14 @@
     if (bound < x1) and (bound + 1 < boundary < x1):
         return boundary
     if (bound > x1) and (x1 < boundary < bound - 1):
         return boundary
     
     return None
 
-@njit
-def get_split_position_v1(x1: float, x2: float, bound: float, c1, c2):
-    assert(x1 != x2)
-    c2 = -c2
-
-    a, b = (c1 - c2) / (x1 - x2), c1 - x1 * ((c1 - c2) / (x1 - x2)) 
-    
-    boundary = round( - b / a)
-
-    if (bound < x1) and (bound < boundary < x1):
-        return boundary
-    if (bound > x1) and (x1 < boundary < bound - 1):
-        return boundary
-    
-    return None
-
 def get_confidence_splits(img, conf_img, img_indexes, c_y, c_x, top, bottom, left, right):
     resolution = img.shape[0]
     i, j = int(c_y), int(c_x)
     label = img[i, j]
     c11 = conf_img[i, j][label]
 
     splits_x, splits_y = [], []    
@@ -311,25 +295,23 @@
     horizontal = [left] if left >= 0 else []
     horizontal += [right] if right < resolution else []
     
     for k in vertical:
         new_label = img[k, j]
         (x, y) = img_indexes[k, j]
         if new_label != label:
-            #split = get_split_position(c_y, y, k, c11, conf_img[y, j][label], conf_img[i, j][new_label], conf_img[y, j][new_label])
-            split = get_split_position_v1(c_y, y, k, c11, conf_img[y, j][label])
+            split = get_split_position(c_y, y, k, c11, conf_img[y, j][label], conf_img[i, j][new_label], conf_img[y, j][new_label])
             if split is not None:
                 splits_y.append(split)
 
     for k in horizontal:
         new_label = img[i, k]
         (x, y) = img_indexes[i, k]
         if new_label != label:
-            #split = get_split_position(c_x, x, k, c11, conf_img[i, x][label], conf_img[i, j][new_label], conf_img[i, x][new_label])
-            split = get_split_position_v1(c_x, x, k, c11, conf_img[i, x][label])
+            split = get_split_position(c_x, x, k, c11, conf_img[i, x][label], conf_img[i, j][new_label], conf_img[i, x][new_label])
             if split is not None:
                 splits_x.append(split)
                 
     return splits_x, splits_y
 
 def get_confidence_based_split(img, conf_img, img_indexes, i, j, W, H):
     c_y, c_x = i, j
```

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/DBMPlotterController.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/DBMPlotterController.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 CLASSIFIER_STACKED_LABELS_CHANGES_FILE = "classifier_old_labels_changes.npy"
 CLASSIFIER_STACKED_BOUNDARY_MAP_FILE = "classifier_old_boundary_map.npy"
 CLASSIFIER_STACKED_CONFIDENCE_MAP_FILE = "classifier_old_boundary_map_confidence.npy"
 
 LABELS_CHANGES_FILE = "label_changes.json"
 
 EPOCHS_FOR_REFIT = 2
+EPOCHS_FOR_REFIT_RANGE = (1, 100)
 
 class DBMPlotterController:
     def __init__(self,
                 logger,
                 dbm_model,
                 img, img_confidence,
                 X_train, Y_train,
@@ -178,30 +179,30 @@
 
         times, accuracies, losses = [], [], []
         with open(path, "r") as f:
             for line in f.readlines():
                 line = line.strip()
                 if len(line) == 0:
                     continue
-                _, time, _, acc, _, _, loss = line.replace("\n", "").replace("%", "").split(" ")
+                _, time, _, acc, _, loss, _, _ = line.replace("\n", "").replace("%", "").split(" ")
                 times.append(time)
                 accuracies.append(float(acc))
                 losses.append(float(loss))
         return times, accuracies, losses
     
-    def compute_classifier_metrics(self):
+    def compute_classifier_metrics(self, epochs):
         self.console.log("Evaluating classifier...")
         loss, accuracy = self.dbm_model.classifier.evaluate(self.X_test, self.Y_test, verbose=0)
         self.console.log(f"Classifier Accuracy: {(100 * accuracy):.2f}%  Loss: {loss:.2f}")
 
         path = os.path.join(self.save_folder, CLASSIFIER_PERFORMANCE_HISTORY_FILE)
 
         with open(path, "a") as f:
             time = datetime.now().strftime("%D %H:%M:%S")
-            message = f"Accuracy: {(100 * accuracy):.2f}%  Loss: {loss:.2f}"
+            message = f"Accuracy: {(100 * accuracy):.2f}% Loss: {loss:.2f} Epochs: {epochs}"
             f.write(f"{time} {message}\n")
         return accuracy, loss
     
     def pop_classifier_evaluation(self):
         path = os.path.join(self.save_folder, CLASSIFIER_PERFORMANCE_HISTORY_FILE)
         # removing the last line
         with open(path, "r") as f:
@@ -382,33 +383,35 @@
         self.img = img
         self.img_confidence = img_confidence
         self.encoded_train = encoded_train
         self.encoded_test = encoded_test
         self.Y_train = Y_transformed
         self.initialize()
         
-    def apply_labels_changes(self, decoding_strategy):
+    def apply_labels_changes(self, decoding_strategy, epochs = None):
         num_changes = len(self.expert_updates_labels_mapper)
         if num_changes == 0:
-            raise Exception("No changes to apply")
+            self.console.error("No changes to apply")
+            return
         if num_changes < 10:
-            raise Exception("Less than 10 changes to apply, please apply more changes")
+            self.console.error("Less than 10 changes to apply, please apply more changes")
+            return
 
         # store the changes done so far so we can restore them when needed
         with open(os.path.join(self.save_folder, CLASSIFIER_STACKED_LABELS_CHANGES_FILE), "wb") as f:
             np.save(f, self.positions_of_labels_changes)
 
         self.console.log("Transforming changes...")
         Y_transformed, label_changes, positions_of_labels_changes = self.transform_changes(self.Y_train, self.expert_updates_labels_mapper, self.positions_of_labels_changes)
         self.positions_of_labels_changes = positions_of_labels_changes
 
         self.console.log("Saving changes to a local folder...")
         self.save_labels_changes(self.save_folder, label_changes=label_changes)
 
-        self.updates_logger.log("Applying changes... This might take a couple of seconds, after this the window will be closed")
+        self.updates_logger.log("Applying changes... This might take a couple of seconds...")
 
         save_folder = os.path.join(self.save_folder, CLASSIFIER_REFIT_FOLDER)
 
         # store the old model so we can restore it when needed
         self.dbm_model.save_classifier(save_folder=os.path.join(self.save_folder, CLASSIFIER_STACKED_FOLDER))
         # store the old labels so we can restore them when needed
         with open(os.path.join(self.save_folder, CLASSIFIER_STACKED_LABELS_FILE), "wb") as f:
@@ -416,15 +419,20 @@
 
         # store the old decision boundary map and confidence map so we can restore them when needed
         with open(os.path.join(self.save_folder, CLASSIFIER_STACKED_BOUNDARY_MAP_FILE), "wb") as f:
             np.save(f, self.img)
         with open(os.path.join(self.save_folder, CLASSIFIER_STACKED_CONFIDENCE_MAP_FILE), "wb") as f:
             np.save(f, self.img_confidence)
 
-        self.dbm_model.refit_classifier(self.X_train, Y_transformed, save_folder=save_folder, epochs=EPOCHS_FOR_REFIT)
+        if epochs is None:
+            epochs = EPOCHS_FOR_REFIT
+        
+        self.updates_logger.log(f"The classifier will be retrained for {epochs} epochs")
+
+        self.dbm_model.refit_classifier(self.X_train, Y_transformed, save_folder=save_folder, epochs=epochs)
         self.regenerate_boundary_map(Y_transformed, decoding_strategy)
         
     def set_dbm_model_logger(self, logger):
         self.dbm_model.console = logger
     
     def set_updates_logger(self, logger):
         self.updates_logger = logger
```

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/DBMPlotterGUI.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/DBMPlotterGUI.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 import matplotlib.pyplot as plt
 from PIL import Image
 import PySimpleGUI as sg
 import matplotlib
 
 from .. import Logger, LoggerGUI, FAST_DBM_STRATEGIES
 from .DBMPlotterController import DBMPlotterController
+from .DBMPlotterController import EPOCHS_FOR_REFIT, EPOCHS_FOR_REFIT_RANGE
 from ..utils import TRAIN_DATA_POINT_MARKER, TEST_DATA_POINT_MARKER, BLACK_COLOR, WHITE_COLOR, RED_COLOR, GREEN_COLOR, YELLOW_COLOR, RIGHTS_MESSAGE_1, RIGHTS_MESSAGE_2, APP_PRIMARY_COLOR, APP_FONT
 
 matplotlib.use("TkAgg")
 
 def draw_figure_to_canvas(canvas, figure, canvas_toolbar=None):
     if canvas.children:
         for child in canvas.winfo_children():
@@ -235,14 +236,27 @@
                             key="-DBM FAST DECODING STRATEGY-",
                             background_color=WHITE_COLOR,
                             text_color=BLACK_COLOR,
                             button_background_color=APP_PRIMARY_COLOR,
                             readonly=True,
                         ),
                     ],
+                    [   
+                        sg.Text(f"Number of epochs:", font=APP_FONT, key="-DBM RELABELING CLASSIFIER EPOCHS TEXT-"),
+                        sg.Slider(range=EPOCHS_FOR_REFIT_RANGE, 
+                               default_value=EPOCHS_FOR_REFIT, 
+                               expand_x=True, 
+                               enable_events=False,
+                               orientation='horizontal',
+                               trough_color=WHITE_COLOR,
+                               font=APP_FONT,
+                               #button_color=(WHITE_COLOR, APP_PRIMARY_COLOR),
+                               tooltip="Select the number of epochs for which \nthe classifier will be retrained.",
+                               key="-DBM RELABELING CLASSIFIER EPOCHS-")
+                    ],
                     [
                         sg.Button("Apply Changes", font=APP_FONT, expand_x=True, key="-APPLY CHANGES-", button_color=(WHITE_COLOR, APP_PRIMARY_COLOR)),
                         sg.Button("Undo Changes", font=APP_FONT, expand_x=True, key="-UNDO CHANGES-", button_color=(WHITE_COLOR, APP_PRIMARY_COLOR)),
                     ],
                     [
                         sg.HSeparator()
                     ],
@@ -363,16 +377,16 @@
         mixed_img[:, :, :3] = color_img
         mixed_img[:, :, 3] = img_confidence
         self.axes_image = self.ax.imshow(mixed_img)
 
         # draw the figure to the canvas
         self.fig_agg = draw_figure_to_canvas(self.canvas, self.fig, self.canvas_controls)
        
-    def compute_classifier_metrics(self):
-        accuracy, loss = self.controller.compute_classifier_metrics()
+    def compute_classifier_metrics(self, epochs=None):
+        accuracy, loss = self.controller.compute_classifier_metrics(epochs)
         self.window["-CLASSIFIER ACCURACY-"].update(f"Classifier Accuracy: {(100 * accuracy):.2f} %  Loss: {loss:.2f}")
         self.update_classifier_performance_canvas()
 
     def pop_classifier_evaluation(self):
         accuracy, loss = self.controller.pop_classifier_evaluation()
         if accuracy is None or loss is None:
             return
@@ -436,17 +450,17 @@
         self.fig.canvas.draw_idle()
         
 
     def handle_circle_selecting_labels_change_event(self, event, values):
         self.update_labels_by_circle_select = values["-CIRCLE SELECTING LABELS-"]
 
     def handle_apply_changes_event(self, event, values):
-        self.controller.apply_labels_changes(decoding_strategy=FAST_DBM_STRATEGIES(values["-DBM FAST DECODING STRATEGY-"]))
+        self.controller.apply_labels_changes(decoding_strategy=FAST_DBM_STRATEGIES(values["-DBM FAST DECODING STRATEGY-"]), epochs=int(values["-DBM RELABELING CLASSIFIER EPOCHS-"]))
         self.initialize()
-        self.compute_classifier_metrics()
+        self.compute_classifier_metrics(int(values["-DBM RELABELING CLASSIFIER EPOCHS-"]))
         self.handle_checkbox_change_event(event, values)
         self.fig_agg = draw_figure_to_canvas(self.canvas, self.fig, self.canvas_controls)
        
 
         self.updates_logger.log("Changes applied successfully!")
 
         if self.main_gui is not None and hasattr(self.main_gui, "handle_changes_in_dbm_plotter"):
```

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/GUI.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/GUI.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/GUIController.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/GUIController.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/__init__.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/GUI/utils.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/GUI/utils.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/Logger.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/Logger.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/LoggerGUI.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/LoggerGUI.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/LoggerInterface.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/LoggerInterface.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/LoggerModel.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/LoggerModel.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/Logger/__init__.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/Logger/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/__init__.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/DBM_usage_example.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/DBM_usage_example.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/SDBM_usage_example.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/SDBM_usage_example.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/__init__.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/examples/utils.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/examples/utils.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/utils/__init__.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/utils/config.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/config.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/utils/dataReader.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/dataReader.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper/utils/tools.py` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper/utils/tools.py`

 * *Files identical despite different names*

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/PKG-INFO` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decision-boundary-mapper
-Version: 0.5.0
+Version: 0.5.1
 Summary: A tool for visualizing the decision boundary of a machine learning model.
 Home-page: https://github.com/cristi2019255/MasterThesis2023
 Author: Cristian Grosu
 Author-email: c.grosu@students.uu.nl
 License: MIT
 Description: # Short Description
```

### Comparing `decision-boundary-mapper-0.5.0/src/decision_boundary_mapper.egg-info/SOURCES.txt` & `decision-boundary-mapper-0.5.1/src/decision_boundary_mapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

