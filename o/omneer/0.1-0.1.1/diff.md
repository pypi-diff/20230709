# Comparing `tmp/omneer-0.1.tar.gz` & `tmp/omneer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omneer-0.1.tar", last modified: Sat Jul  1 05:35:43 2023, max compression
+gzip compressed data, was "omneer-0.1.1.tar", last modified: Sun Jul  9 05:47:52 2023, max compression
```

## Comparing `omneer-0.1.tar` & `omneer-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,58 @@
-drwxr-xr-x   0 willblair   (502) staff       (20)        0 2023-07-01 05:35:43.800131 omneer-0.1/
--rw-r--r--   0 willblair   (502) staff       (20)     3578 2023-07-01 05:35:43.799563 omneer-0.1/PKG-INFO
--rw-r--r--   0 willblair   (502) staff       (20)     3299 2023-07-01 03:48:24.000000 omneer-0.1/README.md
-drwxr-xr-x   0 willblair   (502) staff       (20)        0 2023-07-01 05:35:43.798786 omneer-0.1/omneer.egg-info/
--rw-r--r--   0 willblair   (502) staff       (20)     3578 2023-07-01 05:35:43.000000 omneer-0.1/omneer.egg-info/PKG-INFO
--rw-r--r--   0 willblair   (502) staff       (20)      200 2023-07-01 05:35:43.000000 omneer-0.1/omneer.egg-info/SOURCES.txt
--rw-r--r--   0 willblair   (502) staff       (20)        1 2023-07-01 05:35:43.000000 omneer-0.1/omneer.egg-info/dependency_links.txt
--rw-r--r--   0 willblair   (502) staff       (20)       47 2023-07-01 05:35:43.000000 omneer-0.1/omneer.egg-info/entry_points.txt
--rw-r--r--   0 willblair   (502) staff       (20)      216 2023-07-01 05:35:43.000000 omneer-0.1/omneer.egg-info/requires.txt
--rw-r--r--   0 willblair   (502) staff       (20)        1 2023-07-01 05:35:43.000000 omneer-0.1/omneer.egg-info/top_level.txt
--rw-r--r--   0 willblair   (502) staff       (20)       38 2023-07-01 05:35:43.800401 omneer-0.1/setup.cfg
--rw-r--r--   0 willblair   (502) staff       (20)      976 2023-07-01 05:35:41.000000 omneer-0.1/setup.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-09 05:47:52.004694 omneer-0.1.1/
+-rw-r--r--   0 williamblair   (501) staff       (20)     1063 2023-07-08 06:02:36.000000 omneer-0.1.1/LICENSE
+-rw-r--r--   0 williamblair   (501) staff       (20)     3716 2023-07-09 05:47:52.004396 omneer-0.1.1/PKG-INFO
+-rw-r--r--   0 williamblair   (501) staff       (20)     3292 2023-07-08 00:14:22.000000 omneer-0.1.1/README.md
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-09 05:47:51.973517 omneer-0.1.1/omneer/
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-08 00:14:22.000000 omneer-0.1.1/omneer/__init__.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-09 05:47:51.997387 omneer-0.1.1/omneer/model/
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-08 00:14:22.000000 omneer-0.1.1/omneer/model/__init__.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-09 05:47:51.997742 omneer-0.1.1/omneer/model/deeplearning/
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-08 00:14:22.000000 omneer-0.1.1/omneer/model/deeplearning/__init__.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     8580 2023-07-08 00:15:50.000000 omneer-0.1.1/omneer/model/deeplearning/mlp.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     6212 2023-07-08 00:14:22.000000 omneer-0.1.1/omneer/model/train.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-09 05:47:51.998413 omneer-0.1.1/omneer/processing/
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-08 00:14:22.000000 omneer-0.1.1/omneer/processing/__init__.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     2036 2023-07-08 00:14:22.000000 omneer-0.1.1/omneer/processing/bootstrap.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     4754 2023-07-08 04:20:49.000000 omneer-0.1.1/omneer/processing/main.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     8847 2023-07-08 00:14:22.000000 omneer-0.1.1/omneer/processing/misc.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-09 05:47:51.998933 omneer-0.1.1/omneer/processing/preprocess/
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-08 00:14:23.000000 omneer-0.1.1/omneer/processing/preprocess/__init__.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     3119 2023-07-08 01:30:14.000000 omneer-0.1.1/omneer/processing/preprocess/features.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     6077 2023-07-08 17:24:34.000000 omneer-0.1.1/omneer/processing/preprocess/preprocess.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-09 05:47:51.999232 omneer-0.1.1/omneer/visualization/
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-08 00:14:23.000000 omneer-0.1.1/omneer/visualization/__init__.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-09 05:47:52.001810 omneer-0.1.1/omneer/visualization/graph/
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-08 00:14:23.000000 omneer-0.1.1/omneer/visualization/graph/__init__.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     4917 2023-07-08 00:18:45.000000 omneer-0.1.1/omneer/visualization/graph/grid_search_.py
+-rw-r--r--   0 williamblair   (501) staff       (20)      979 2023-07-08 00:14:23.000000 omneer-0.1.1/omneer/visualization/graph/plot_summary.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     1573 2023-07-08 00:14:23.000000 omneer-0.1.1/omneer/visualization/graph/plot_swarm.py
+-rw-r--r--   0 williamblair   (501) staff       (20)      496 2023-07-08 00:14:23.000000 omneer-0.1.1/omneer/visualization/graph/shap_1_aggregate.py
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-08 00:14:23.000000 omneer-0.1.1/omneer/visualization/graph/shap_2_average.py
+-rw-r--r--   0 williamblair   (501) staff       (20)      744 2023-07-08 00:14:23.000000 omneer-0.1.1/omneer/visualization/graph/shap_3_correlation.py
+-rw-r--r--   0 williamblair   (501) staff       (20)      428 2023-07-08 00:14:23.000000 omneer-0.1.1/omneer/visualization/graph/shap_4_summary.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     1576 2023-07-08 00:19:43.000000 omneer-0.1.1/omneer/visualization/graph/shap_analysis__.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     2955 2023-07-08 00:14:23.000000 omneer-0.1.1/omneer/visualization/plot.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-09 05:47:52.002385 omneer-0.1.1/omneer/visualization/raw/
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-08 00:14:23.000000 omneer-0.1.1/omneer/visualization/raw/__init__.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     8451 2023-07-08 00:19:36.000000 omneer-0.1.1/omneer/visualization/raw/vis.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-09 05:47:51.996863 omneer-0.1.1/omneer.egg-info/
+-rw-r--r--   0 williamblair   (501) staff       (20)     3716 2023-07-09 05:47:51.000000 omneer-0.1.1/omneer.egg-info/PKG-INFO
+-rw-r--r--   0 williamblair   (501) staff       (20)     1420 2023-07-09 05:47:51.000000 omneer-0.1.1/omneer.egg-info/SOURCES.txt
+-rw-r--r--   0 williamblair   (501) staff       (20)        1 2023-07-09 05:47:51.000000 omneer-0.1.1/omneer.egg-info/dependency_links.txt
+-rw-r--r--   0 williamblair   (501) staff       (20)       48 2023-07-09 05:47:51.000000 omneer-0.1.1/omneer.egg-info/entry_points.txt
+-rw-r--r--   0 williamblair   (501) staff       (20)      268 2023-07-09 05:47:51.000000 omneer-0.1.1/omneer.egg-info/requires.txt
+-rw-r--r--   0 williamblair   (501) staff       (20)       18 2023-07-09 05:47:51.000000 omneer-0.1.1/omneer.egg-info/top_level.txt
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-09 05:47:52.002840 omneer-0.1.1/omneer_cli/
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-08 00:14:23.000000 omneer-0.1.1/omneer_cli/__init__.py
+-rw-r--r--   0 williamblair   (501) staff       (20)    10145 2023-07-09 05:19:34.000000 omneer-0.1.1/omneer_cli/main.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-09 05:47:52.003677 omneer-0.1.1/omneer_cli/processing/
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-08 07:10:22.000000 omneer-0.1.1/omneer_cli/processing/__init__.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     2036 2023-07-08 07:10:22.000000 omneer-0.1.1/omneer_cli/processing/bootstrap.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     4243 2023-07-08 19:21:19.000000 omneer-0.1.1/omneer_cli/processing/main.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     8847 2023-07-08 07:10:22.000000 omneer-0.1.1/omneer_cli/processing/misc.py
+drwxr-xr-x   0 williamblair   (501) staff       (20)        0 2023-07-09 05:47:52.004170 omneer-0.1.1/omneer_cli/processing/preprocess/
+-rw-r--r--   0 williamblair   (501) staff       (20)        0 2023-07-08 07:10:22.000000 omneer-0.1.1/omneer_cli/processing/preprocess/__init__.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     3119 2023-07-08 07:10:22.000000 omneer-0.1.1/omneer_cli/processing/preprocess/features.py
+-rw-r--r--   0 williamblair   (501) staff       (20)     7689 2023-07-09 04:34:50.000000 omneer-0.1.1/omneer_cli/processing/preprocess/preprocess.py
+-rw-r--r--   0 williamblair   (501) staff       (20)       38 2023-07-09 05:47:52.004742 omneer-0.1.1/setup.cfg
+-rw-r--r--   0 williamblair   (501) staff       (20)     1573 2023-07-09 05:47:39.000000 omneer-0.1.1/setup.py
```

### Comparing `omneer-0.1/PKG-INFO` & `omneer-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: omneer
-Version: 0.1
-Summary: Advanced personalized medicine diagnostics for neurodegenerative disorders
-Home-page: http://omneer.xyz
+Version: 0.1.1
+Summary: Omneer SDK
+Home-page: http://docs.omneer.xyz
 Author: William Blair
 Author-email: william.blair0708@gmail.com
 License: MIT
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 <div align="center">
 
 # Omneer SDK
 
 Omneer SDK is a state-of-the-art toolkit designed for the development and deployment of AI and machine learning powered personalized medicine applications in the neuroscience field. The SDK, with its Python-centric approach, provides an easy-to-use platform for developers to create and interact with their applications.
 
@@ -34,18 +39,18 @@
 
 - Omneer SDK continues to be a ground-breaking platform for personalized healthcare solutions. Browse our collection of existing and actively maintained solutions at [Omneer Community]().
 
 ### Getting Started
 
 See the SDK in action by following the steps below to register your first workflow with Omneer.
 
-First, install latch through `pip`.
+First, install omneer through `pip`.
 
 ```
-$ python3 pip install omneer
+$ pip install omneer
 ```
 
 Then, create some boilerplate code for your new workflow.
 
 ```
 $ omneer init diagnosis
 ```
```

### Comparing `omneer-0.1/README.md` & `omneer-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
 - Omneer SDK continues to be a ground-breaking platform for personalized healthcare solutions. Browse our collection of existing and actively maintained solutions at [Omneer Community]().
 
 ### Getting Started
 
 See the SDK in action by following the steps below to register your first workflow with Omneer.
 
-First, install latch through `pip`.
+First, install omneer through `pip`.
 
 ```
-$ python3 pip install omneer
+$ pip install omneer
 ```
 
 Then, create some boilerplate code for your new workflow.
 
 ```
 $ omneer init diagnosis
 ```
```

### Comparing `omneer-0.1/omneer.egg-info/PKG-INFO` & `omneer-0.1.1/omneer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: omneer
-Version: 0.1
-Summary: Advanced personalized medicine diagnostics for neurodegenerative disorders
-Home-page: http://omneer.xyz
+Version: 0.1.1
+Summary: Omneer SDK
+Home-page: http://docs.omneer.xyz
 Author: William Blair
 Author-email: william.blair0708@gmail.com
 License: MIT
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 <div align="center">
 
 # Omneer SDK
 
 Omneer SDK is a state-of-the-art toolkit designed for the development and deployment of AI and machine learning powered personalized medicine applications in the neuroscience field. The SDK, with its Python-centric approach, provides an easy-to-use platform for developers to create and interact with their applications.
 
@@ -34,18 +39,18 @@
 
 - Omneer SDK continues to be a ground-breaking platform for personalized healthcare solutions. Browse our collection of existing and actively maintained solutions at [Omneer Community]().
 
 ### Getting Started
 
 See the SDK in action by following the steps below to register your first workflow with Omneer.
 
-First, install latch through `pip`.
+First, install omneer through `pip`.
 
 ```
-$ python3 pip install omneer
+$ pip install omneer
 ```
 
 Then, create some boilerplate code for your new workflow.
 
 ```
 $ omneer init diagnosis
 ```
```

### Comparing `omneer-0.1/setup.py` & `omneer-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,31 @@
-from setuptools import setup, find_packages
+import sys
+
+from setuptools import find_packages, setup
+
+cur_ver = sys.version_info[:2]
+ver_str = ".".join(map(str, cur_ver))
+
+if cur_ver < (3, 8) or cur_ver > (3, 10):
+    raise RuntimeError(
+        f"Python {ver_str} is unsupported. Please use a Python version between 3.8 and"
+        " 3.10, inclusive."
+    )
 
 setup(
     name='omneer',
-    version='0.1',
-    packages=find_packages(include=['omneer', 'omneer.*']),
-    url='http://omneer.xyz',
+    version='v0.1.1',
+    url='http://docs.omneer.xyz',
     license='MIT',
     author='William Blair',
     author_email='william.blair0708@gmail.com',
-    description='Advanced personalized medicine diagnostics for neurodegenerative disorders',
+    description='Omneer SDK',
+    packages=find_packages(),
+    include_package_data=True,
+    python_requires=">=3.8,<3.11",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'numpy>=1.19.0',
         'pandas>=1.2.0',
         'matplotlib>=3.3.0',
         'scipy>=1.6.0',
@@ -22,14 +35,23 @@
         'flake8>=3.9.0',
         'black>=21.6b0',
         'scikit-learn>=0.24.0',
         'torch>=1.9.0',
         'tqdm>=4.62.0',
         'xgboost>=1.4.0',
         'joblib>=1.0.0',
+        'click>=8.0.1',
+        'typer>=0.3.2',
+        'halo>=0.0.31',
+        'rich>=10.6.0',
     ],
     entry_points={
         'console_scripts': [
-            'omneer=omneer.lc.main:main',
+            'omneer=omneer_cli.main:main',  # Replace with the correct module and function name
         ],
     },
-)
+        classifiers=[
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+        ],
+    )
```

