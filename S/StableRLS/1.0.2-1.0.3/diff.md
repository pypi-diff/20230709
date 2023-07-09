# Comparing `tmp/StableRLS-1.0.2.tar.gz` & `tmp/StableRLS-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StableRLS-1.0.2.tar", last modified: Sun Jul  9 16:31:59 2023, max compression
+gzip compressed data, was "StableRLS-1.0.3.tar", last modified: Sun Jul  9 16:36:47 2023, max compression
```

## Comparing `StableRLS-1.0.2.tar` & `StableRLS-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 16:31:59.817880 StableRLS-1.0.2/
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)    35148 2023-03-21 15:46:09.000000 StableRLS-1.0.2/LICENSE.txt
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4686 2023-07-09 16:31:59.817880 StableRLS-1.0.2/PKG-INFO
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4314 2023-07-09 15:09:21.000000 StableRLS-1.0.2/README.md
-drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 16:31:59.817880 StableRLS-1.0.2/StableRLS.egg-info/
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4686 2023-07-09 16:31:59.000000 StableRLS-1.0.2/StableRLS.egg-info/PKG-INFO
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)      328 2023-07-09 16:31:59.000000 StableRLS-1.0.2/StableRLS.egg-info/SOURCES.txt
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)        1 2023-07-09 16:31:59.000000 StableRLS-1.0.2/StableRLS.egg-info/dependency_links.txt
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       37 2023-07-09 16:31:59.000000 StableRLS-1.0.2/StableRLS.egg-info/requires.txt
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       10 2023-07-09 16:31:59.000000 StableRLS-1.0.2/StableRLS.egg-info/top_level.txt
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       38 2023-07-09 16:31:59.817880 StableRLS-1.0.2/setup.cfg
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)      780 2023-07-09 16:31:51.000000 StableRLS-1.0.2/setup.py
-drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 16:31:59.817880 StableRLS-1.0.2/stablerls/
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)        0 2023-03-21 15:46:09.000000 StableRLS-1.0.2/stablerls/__init__.py
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     2918 2023-07-09 15:00:17.000000 StableRLS-1.0.2/stablerls/configreader.py
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     2868 2023-07-09 15:00:25.000000 StableRLS-1.0.2/stablerls/createFMU.py
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4188 2023-07-01 15:03:04.000000 StableRLS-1.0.2/stablerls/fmutools.py
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)    15697 2023-05-08 13:15:04.000000 StableRLS-1.0.2/stablerls/getports.m
--rw-rw-r--   0 cao2851   (1000) cao2851   (1000)    17470 2023-07-01 15:03:05.000000 StableRLS-1.0.2/stablerls/gymFMU.py
+drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 16:36:47.001827 StableRLS-1.0.3/
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)    35148 2023-03-21 15:46:09.000000 StableRLS-1.0.3/LICENSE.txt
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4680 2023-07-09 16:36:47.001827 StableRLS-1.0.3/PKG-INFO
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4314 2023-07-09 15:09:21.000000 StableRLS-1.0.3/README.md
+drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 16:36:47.001827 StableRLS-1.0.3/StableRLS.egg-info/
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4680 2023-07-09 16:36:46.000000 StableRLS-1.0.3/StableRLS.egg-info/PKG-INFO
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)      328 2023-07-09 16:36:46.000000 StableRLS-1.0.3/StableRLS.egg-info/SOURCES.txt
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)        1 2023-07-09 16:36:46.000000 StableRLS-1.0.3/StableRLS.egg-info/dependency_links.txt
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       37 2023-07-09 16:36:46.000000 StableRLS-1.0.3/StableRLS.egg-info/requires.txt
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       10 2023-07-09 16:36:46.000000 StableRLS-1.0.3/StableRLS.egg-info/top_level.txt
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)       38 2023-07-09 16:36:47.001827 StableRLS-1.0.3/setup.cfg
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)      787 2023-07-09 16:36:43.000000 StableRLS-1.0.3/setup.py
+drwxrwxr-x   0 cao2851   (1000) cao2851   (1000)        0 2023-07-09 16:36:47.001827 StableRLS-1.0.3/stablerls/
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)        0 2023-03-21 15:46:09.000000 StableRLS-1.0.3/stablerls/__init__.py
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     2918 2023-07-09 15:00:17.000000 StableRLS-1.0.3/stablerls/configreader.py
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     2868 2023-07-09 15:00:25.000000 StableRLS-1.0.3/stablerls/createFMU.py
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)     4188 2023-07-01 15:03:04.000000 StableRLS-1.0.3/stablerls/fmutools.py
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)    15697 2023-05-08 13:15:04.000000 StableRLS-1.0.3/stablerls/getports.m
+-rw-rw-r--   0 cao2851   (1000) cao2851   (1000)    17470 2023-07-01 15:03:05.000000 StableRLS-1.0.3/stablerls/gymFMU.py
```

### Comparing `StableRLS-1.0.2/LICENSE.txt` & `StableRLS-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.2/PKG-INFO` & `StableRLS-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StableRLS
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simulate Simulink FMUs as Gymnasium environment
 Home-page: https://github.com/rAnnuth/stablerls
 Author: Robert Annuth
 Author-email: robert.annuth@tuhh.de
 License: LICENSE.txt
 Keywords: simulation RL reinforcement learning Simulink matlab FMU
 Description-Content-Type: text/markdown
@@ -31,15 +31,15 @@
 
 
 ## General Information
 Reinforcement Learning (RL) is a fast changing and innovative field. The main purpose of this package is to bring the easy-to-use MATLAB Simulink modeling interface together with the flexible and state-of-the-art Gymnasium interface. So the RL algorithm and learning interface are out of scope for this package. However, we make the interface between Matlab and Python as easy as possible.
 
 ## Installation
 The package is currently tested with Python 3.9.
-%TODO To install the package, run `pip install stablerls`.
+To install the package, run `pip install StableRLS`.
 
 You can also clone this repository and run `pip install -e StableRLS/` from the main directory. This will also install the main dependencies, which are included in `requirements.txt`. For active contribution, you should also install the `optional-requirements.txt`, which also includes the dependencies to build the documentation by running `pip install -r optional-requirements.txt`.
 
 We decided to exclude the typical machine learning frameworks (PyTorch, Tensorflow) from the requirements, because everyone has their own preferences and we want to keep this package small. But some of our example are based on PyTorch, so you need to run `pip install torch` if you want to run them locally. This will also be mentioned in the examples. To compile the documentation locally, Pandoc has to be installed on your computer.
 
 
 ### Matlab Version
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: StableRLS Version: 1.0.2 Summary: Simulate Simulink
+Metadata-Version: 2.1 Name: StableRLS Version: 1.0.3 Summary: Simulate Simulink
 FMUs as Gymnasium environment Home-page: https://github.com/rAnnuth/stablerls
 Author: Robert Annuth Author-email: robert.annuth@tuhh.de License: LICENSE.txt
 Keywords: simulation RL reinforcement learning Simulink matlab FMU Description-
 Content-Type: text/markdown License-File: LICENSE.txt ![](src/icon.png)
             ***** Stable Reinforcement Learning for Simulink *****
                   [Documentation_Status] [Code_style:_black]
 StableRLS is a software package to use your existing MATLAB Simulink models in
@@ -14,44 +14,44 @@
 easy-to-read code **And the best part is** that the only thing you need to do
 is: - defining a reward function to train your agent ## General Information
 Reinforcement Learning (RL) is a fast changing and innovative field. The main
 purpose of this package is to bring the easy-to-use MATLAB Simulink modeling
 interface together with the flexible and state-of-the-art Gymnasium interface.
 So the RL algorithm and learning interface are out of scope for this package.
 However, we make the interface between Matlab and Python as easy as possible.
-## Installation The package is currently tested with Python 3.9. %TODO To
-install the package, run `pip install stablerls`. You can also clone this
-repository and run `pip install -e StableRLS/` from the main directory. This
-will also install the main dependencies, which are included in
-`requirements.txt`. For active contribution, you should also install the
-`optional-requirements.txt`, which also includes the dependencies to build the
-documentation by running `pip install -r optional-requirements.txt`. We decided
-to exclude the typical machine learning frameworks (PyTorch, Tensorflow) from
-the requirements, because everyone has their own preferences and we want to
-keep this package small. But some of our example are based on PyTorch, so you
-need to run `pip install torch` if you want to run them locally. This will also
-be mentioned in the examples. To compile the documentation locally, Pandoc has
-to be installed on your computer. ### Matlab Version The StableRLS package is
-able to compile a given MATLAB Simulink model to a FMU. The MATLAB engine
-Python package is a requirement for this. Before the MATLAB release R2022b it
-was inconvenient to install the engine, see the [instructions](https://
-de.mathworks.com/help/matlab/matlab_external/install-the-matlab-engine-for-
-python.html). After the release, it's possible to install it as a pip package.
-StableRLS won't try to install the MATLAB engine as dependency because the pip
-package only supports the newest MATLAB release. Currently, you can run `pip
-install matlabengine` if you have MATLAB 2023a installed, if you have MATLAB
-2022b installed run `pip install matlabengine==9.13.7`. For other releases
-refer to the documentation mentioned. ## Get Started Check out our examples (/
-examples) or the documentation, which also contains the examples. ##
-Contribution and other issues We are researchers in the field of electrical
-engineering, but this package is also useful for other engineers that use
-MATLAB Simulink as part of their research. If you want to collaborate and
-develop this tool further, simply create issues or pull requests. In case of
-issues installing or using this tool, you can also create an issue. For more
-information about contributions and issues, take a look at [HOW_TO_CONTRIBUTE]
+## Installation The package is currently tested with Python 3.9. To install the
+package, run `pip install StableRLS`. You can also clone this repository and
+run `pip install -e StableRLS/` from the main directory. This will also install
+the main dependencies, which are included in `requirements.txt`. For active
+contribution, you should also install the `optional-requirements.txt`, which
+also includes the dependencies to build the documentation by running `pip
+install -r optional-requirements.txt`. We decided to exclude the typical
+machine learning frameworks (PyTorch, Tensorflow) from the requirements,
+because everyone has their own preferences and we want to keep this package
+small. But some of our example are based on PyTorch, so you need to run `pip
+install torch` if you want to run them locally. This will also be mentioned in
+the examples. To compile the documentation locally, Pandoc has to be installed
+on your computer. ### Matlab Version The StableRLS package is able to compile a
+given MATLAB Simulink model to a FMU. The MATLAB engine Python package is a
+requirement for this. Before the MATLAB release R2022b it was inconvenient to
+install the engine, see the [instructions](https://de.mathworks.com/help/
+matlab/matlab_external/install-the-matlab-engine-for-python.html). After the
+release, it's possible to install it as a pip package. StableRLS won't try to
+install the MATLAB engine as dependency because the pip package only supports
+the newest MATLAB release. Currently, you can run `pip install matlabengine` if
+you have MATLAB 2023a installed, if you have MATLAB 2022b installed run `pip
+install matlabengine==9.13.7`. For other releases refer to the documentation
+mentioned. ## Get Started Check out our examples (/examples) or the
+documentation, which also contains the examples. ## Contribution and other
+issues We are researchers in the field of electrical engineering, but this
+package is also useful for other engineers that use MATLAB Simulink as part of
+their research. If you want to collaborate and develop this tool further,
+simply create issues or pull requests. In case of issues installing or using
+this tool, you can also create an issue. For more information about
+contributions and issues, take a look at [HOW_TO_CONTRIBUTE]
 [HOW_TO_CONTRIBUTE.md]. ## Building the documentation Run `sphinx-autobuild
 docs/ docs/build/html` from the main directory and open the documentation
 `localhost:8000`. The page is updated automatically after any file in the
 documentation is changed. ## More information To install clean use `pip freeze
 | grep -v -f requirements.txt - | grep -v '^#' | grep -v '^-e ' | xargs pip
 uninstall -y` to remove all packages except the one with -e flag. Afterwards
 `pip install -r requirements.txt`. ## Make this public - [ ] [https://
```

### Comparing `StableRLS-1.0.2/README.md` & `StableRLS-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.2/StableRLS.egg-info/PKG-INFO` & `StableRLS-1.0.3/StableRLS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StableRLS
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simulate Simulink FMUs as Gymnasium environment
 Home-page: https://github.com/rAnnuth/stablerls
 Author: Robert Annuth
 Author-email: robert.annuth@tuhh.de
 License: LICENSE.txt
 Keywords: simulation RL reinforcement learning Simulink matlab FMU
 Description-Content-Type: text/markdown
@@ -31,15 +31,15 @@
 
 
 ## General Information
 Reinforcement Learning (RL) is a fast changing and innovative field. The main purpose of this package is to bring the easy-to-use MATLAB Simulink modeling interface together with the flexible and state-of-the-art Gymnasium interface. So the RL algorithm and learning interface are out of scope for this package. However, we make the interface between Matlab and Python as easy as possible.
 
 ## Installation
 The package is currently tested with Python 3.9.
-%TODO To install the package, run `pip install stablerls`.
+To install the package, run `pip install StableRLS`.
 
 You can also clone this repository and run `pip install -e StableRLS/` from the main directory. This will also install the main dependencies, which are included in `requirements.txt`. For active contribution, you should also install the `optional-requirements.txt`, which also includes the dependencies to build the documentation by running `pip install -r optional-requirements.txt`.
 
 We decided to exclude the typical machine learning frameworks (PyTorch, Tensorflow) from the requirements, because everyone has their own preferences and we want to keep this package small. But some of our example are based on PyTorch, so you need to run `pip install torch` if you want to run them locally. This will also be mentioned in the examples. To compile the documentation locally, Pandoc has to be installed on your computer.
 
 
 ### Matlab Version
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: StableRLS Version: 1.0.2 Summary: Simulate Simulink
+Metadata-Version: 2.1 Name: StableRLS Version: 1.0.3 Summary: Simulate Simulink
 FMUs as Gymnasium environment Home-page: https://github.com/rAnnuth/stablerls
 Author: Robert Annuth Author-email: robert.annuth@tuhh.de License: LICENSE.txt
 Keywords: simulation RL reinforcement learning Simulink matlab FMU Description-
 Content-Type: text/markdown License-File: LICENSE.txt ![](src/icon.png)
             ***** Stable Reinforcement Learning for Simulink *****
                   [Documentation_Status] [Code_style:_black]
 StableRLS is a software package to use your existing MATLAB Simulink models in
@@ -14,44 +14,44 @@
 easy-to-read code **And the best part is** that the only thing you need to do
 is: - defining a reward function to train your agent ## General Information
 Reinforcement Learning (RL) is a fast changing and innovative field. The main
 purpose of this package is to bring the easy-to-use MATLAB Simulink modeling
 interface together with the flexible and state-of-the-art Gymnasium interface.
 So the RL algorithm and learning interface are out of scope for this package.
 However, we make the interface between Matlab and Python as easy as possible.
-## Installation The package is currently tested with Python 3.9. %TODO To
-install the package, run `pip install stablerls`. You can also clone this
-repository and run `pip install -e StableRLS/` from the main directory. This
-will also install the main dependencies, which are included in
-`requirements.txt`. For active contribution, you should also install the
-`optional-requirements.txt`, which also includes the dependencies to build the
-documentation by running `pip install -r optional-requirements.txt`. We decided
-to exclude the typical machine learning frameworks (PyTorch, Tensorflow) from
-the requirements, because everyone has their own preferences and we want to
-keep this package small. But some of our example are based on PyTorch, so you
-need to run `pip install torch` if you want to run them locally. This will also
-be mentioned in the examples. To compile the documentation locally, Pandoc has
-to be installed on your computer. ### Matlab Version The StableRLS package is
-able to compile a given MATLAB Simulink model to a FMU. The MATLAB engine
-Python package is a requirement for this. Before the MATLAB release R2022b it
-was inconvenient to install the engine, see the [instructions](https://
-de.mathworks.com/help/matlab/matlab_external/install-the-matlab-engine-for-
-python.html). After the release, it's possible to install it as a pip package.
-StableRLS won't try to install the MATLAB engine as dependency because the pip
-package only supports the newest MATLAB release. Currently, you can run `pip
-install matlabengine` if you have MATLAB 2023a installed, if you have MATLAB
-2022b installed run `pip install matlabengine==9.13.7`. For other releases
-refer to the documentation mentioned. ## Get Started Check out our examples (/
-examples) or the documentation, which also contains the examples. ##
-Contribution and other issues We are researchers in the field of electrical
-engineering, but this package is also useful for other engineers that use
-MATLAB Simulink as part of their research. If you want to collaborate and
-develop this tool further, simply create issues or pull requests. In case of
-issues installing or using this tool, you can also create an issue. For more
-information about contributions and issues, take a look at [HOW_TO_CONTRIBUTE]
+## Installation The package is currently tested with Python 3.9. To install the
+package, run `pip install StableRLS`. You can also clone this repository and
+run `pip install -e StableRLS/` from the main directory. This will also install
+the main dependencies, which are included in `requirements.txt`. For active
+contribution, you should also install the `optional-requirements.txt`, which
+also includes the dependencies to build the documentation by running `pip
+install -r optional-requirements.txt`. We decided to exclude the typical
+machine learning frameworks (PyTorch, Tensorflow) from the requirements,
+because everyone has their own preferences and we want to keep this package
+small. But some of our example are based on PyTorch, so you need to run `pip
+install torch` if you want to run them locally. This will also be mentioned in
+the examples. To compile the documentation locally, Pandoc has to be installed
+on your computer. ### Matlab Version The StableRLS package is able to compile a
+given MATLAB Simulink model to a FMU. The MATLAB engine Python package is a
+requirement for this. Before the MATLAB release R2022b it was inconvenient to
+install the engine, see the [instructions](https://de.mathworks.com/help/
+matlab/matlab_external/install-the-matlab-engine-for-python.html). After the
+release, it's possible to install it as a pip package. StableRLS won't try to
+install the MATLAB engine as dependency because the pip package only supports
+the newest MATLAB release. Currently, you can run `pip install matlabengine` if
+you have MATLAB 2023a installed, if you have MATLAB 2022b installed run `pip
+install matlabengine==9.13.7`. For other releases refer to the documentation
+mentioned. ## Get Started Check out our examples (/examples) or the
+documentation, which also contains the examples. ## Contribution and other
+issues We are researchers in the field of electrical engineering, but this
+package is also useful for other engineers that use MATLAB Simulink as part of
+their research. If you want to collaborate and develop this tool further,
+simply create issues or pull requests. In case of issues installing or using
+this tool, you can also create an issue. For more information about
+contributions and issues, take a look at [HOW_TO_CONTRIBUTE]
 [HOW_TO_CONTRIBUTE.md]. ## Building the documentation Run `sphinx-autobuild
 docs/ docs/build/html` from the main directory and open the documentation
 `localhost:8000`. The page is updated automatically after any file in the
 documentation is changed. ## More information To install clean use `pip freeze
 | grep -v -f requirements.txt - | grep -v '^#' | grep -v '^-e ' | xargs pip
 uninstall -y` to remove all packages except the one with -e flag. Afterwards
 `pip install -r requirements.txt`. ## Make this public - [ ] [https://
```

### Comparing `StableRLS-1.0.2/setup.py` & `StableRLS-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools 
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
+long_description = (this_directory / '..' / "README.md").read_text()
 
 setuptools.setup(
   name='StableRLS',
-  version='1.0.2',
+  version='1.0.3',
   author='Robert Annuth',
   author_email='robert.annuth@tuhh.de',
   packages= setuptools.find_packages(),
   package_data={'stablerls':['*']},
   license='LICENSE.txt',
   description='Simulate Simulink FMUs as Gymnasium environment',
   long_description=long_description,
```

### Comparing `StableRLS-1.0.2/stablerls/configreader.py` & `StableRLS-1.0.3/stablerls/configreader.py`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.2/stablerls/createFMU.py` & `StableRLS-1.0.3/stablerls/createFMU.py`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.2/stablerls/fmutools.py` & `StableRLS-1.0.3/stablerls/fmutools.py`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.2/stablerls/getports.m` & `StableRLS-1.0.3/stablerls/getports.m`

 * *Files identical despite different names*

### Comparing `StableRLS-1.0.2/stablerls/gymFMU.py` & `StableRLS-1.0.3/stablerls/gymFMU.py`

 * *Files identical despite different names*

