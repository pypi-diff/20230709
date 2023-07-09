# Comparing `tmp/pypostalwin-0.0.3.tar.gz` & `tmp/pypostalwin-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypostalwin-0.0.3.tar", last modified: Mon Apr 11 18:00:26 2022, max compression
+gzip compressed data, was "pypostalwin-0.0.4.tar", last modified: Sun Jul  9 10:51:20 2023, max compression
```

## Comparing `pypostalwin-0.0.3.tar` & `pypostalwin-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-04-11 18:00:26.519864 pypostalwin-0.0.3/
--rw-rw-rw-   0        0        0     1090 2022-04-11 17:43:44.000000 pypostalwin-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     4425 2022-04-11 18:00:26.519864 pypostalwin-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      248 2022-04-11 17:43:44.000000 pypostalwin-0.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2022-04-11 18:00:26.497682 pypostalwin-0.0.3/pypostalwin/
-drwxrwxrwx   0        0        0        0 2022-04-11 18:00:26.517867 pypostalwin-0.0.3/pypostalwin/src/
-drwxrwxrwx   0        0        0        0 2022-04-11 18:00:26.515872 pypostalwin-0.0.3/pypostalwin/src/pypostalwin.egg-info/
--rw-rw-rw-   0        0        0     4425 2022-04-11 18:00:26.000000 pypostalwin-0.0.3/pypostalwin/src/pypostalwin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2022-04-11 18:00:26.000000 pypostalwin-0.0.3/pypostalwin/src/pypostalwin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-11 18:00:26.000000 pypostalwin-0.0.3/pypostalwin/src/pypostalwin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-04-11 18:00:26.000000 pypostalwin-0.0.3/pypostalwin/src/pypostalwin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2936 2022-04-11 17:46:43.000000 pypostalwin-0.0.3/pypostalwin/src/pypostalwin.py
--rw-rw-rw-   0        0        0      221 2022-04-11 17:43:44.000000 pypostalwin-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-04-11 18:00:26.519864 pypostalwin-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1380 2022-04-11 17:58:14.000000 pypostalwin-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 10:51:20.922851 pypostalwin-0.0.4/
+-rw-rw-rw-   0        0        0     1090 2023-07-02 09:59:39.000000 pypostalwin-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4452 2023-07-09 10:51:20.921627 pypostalwin-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-07-02 09:59:39.000000 pypostalwin-0.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-09 10:51:20.878327 pypostalwin-0.0.4/pypostalwin/
+drwxrwxrwx   0        0        0        0 2023-07-09 10:51:20.919624 pypostalwin-0.0.4/pypostalwin/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 10:51:20.917625 pypostalwin-0.0.4/pypostalwin/src/pypostalwin.egg-info/
+-rw-rw-rw-   0        0        0     4452 2023-07-09 10:51:20.000000 pypostalwin-0.0.4/pypostalwin/src/pypostalwin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-07-09 10:51:20.000000 pypostalwin-0.0.4/pypostalwin/src/pypostalwin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 10:51:20.000000 pypostalwin-0.0.4/pypostalwin/src/pypostalwin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-09 10:51:20.000000 pypostalwin-0.0.4/pypostalwin/src/pypostalwin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3281 2023-07-09 10:31:45.000000 pypostalwin-0.0.4/pypostalwin/src/pypostalwin.py
+-rw-rw-rw-   0        0        0       42 2023-07-09 10:51:20.922851 pypostalwin-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1400 2023-07-09 10:33:13.000000 pypostalwin-0.0.4/setup.py
```

### Comparing `pypostalwin-0.0.3/LICENSE` & `pypostalwin-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypostalwin-0.0.3/PKG-INFO` & `pypostalwin-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: pypostalwin
-Version: 0.0.3
+Version: 0.0.4
 Summary:  python package for libpostal wrapper only for windows
 Home-page: https://github.com/selva221724/pypostalwin
-Author: Tamil Selvan A V
+Author: Tamil Selvan A V and Dominic Mukilan
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: IPython
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
@@ -32,27 +31,27 @@
 
 
 ## About libpostal
 libpostal is a C library for parsing/normalizing street addresses around the world using statistical NLP and open data. The goal of this project is to understand location-based strings in every language, everywhere.
 
 ## Installation
 
-### 1. Build the libpostal in windows
-- Before usign the Python wrapper, you need to build the libpostal C library as a bundle which can be accessed by the python package. (still under development) 
+### 1. Build the libpostal in Windows
+- Before using the Python wrapper, you need to build the libpostal C library as a bundle which can be accessed by the python package. (still under development) 
 
 (OR)
 
 - Download and Install [MSYS2](https://www.msys2.org/)
 - You can use the libpostal prebuilt zipped file [Download here](https://drive.google.com/file/d/1fZUlyLFCGYD7l_PDM0NzD8pAo-ICrVVd/view?usp=sharing)  
 - Unpack the zip to C:\Workbench\libpostal\
-- If you dont have **Workbench** folder in C Drive, then create one. 
+- If you don't have **Workbench** folder in C Drive, then create one. 
 - Copy the zip inside the **Workbench** and unzip using [7zip](https://www.7-zip.org/download.html) 
 
-### 2 . Install the python wrapper 
-**Install using pip** . [Offical Python Package Here!!](https://pypi.org/project/pypostalwin/)
+### 2. Install the python wrapper 
+**Install using pip**. [Offical Python Package Here!!](https://pypi.org/project/pypostalwin/)
 ```shell
 pip install pypostalwin
 ```
 
 (OR)
 
 Clone this Repository. Run this from the root directory to install
@@ -67,16 +66,16 @@
 ```python
 import pypostalwin
 ```
 
 ### 1. Initialize Address Parser Object
 ```python
 parser = pypostalwin.AddressParser()
-parsedAddress = parser.runParser("The White House 1600 Pennsylvania Avenue NW, Washington, DC 20500, USA")
-print(parsedAddress)
+parsed_address = parser.parse_address("The White House 1600 Pennsylvania Avenue NW, Washington, DC 20500, USA")
+print(parsed_address)
 ```
 output
 ```sh
 [
   {'house': 'the white house'}, 
   {'house_number': '1600'},
   {'road': 'pennsylvania avenue nw'}, 
@@ -89,31 +88,29 @@
 ```
 **Note:** In a single runtime, the first-time parser.runParser() will take a few seconds to run since it is loading the models from libpostal in the backend process. Once it is loaded, the recurrent runs will be faster as usual. You need to use the same object instance to get the results faster.
 
 for eg:
 
 ```python
 parser = pypostalwin.AddressParser()
-parsedAddress1 = parser.runParser("The White House 1600") #only first time will take few seconds to load
-parsedAddress2 = parser.runParser("Washington, DC 20500, USA") #will be faster as usual
-parsedAddress3 = parser.runParser(" 20500, USA") #will be faster as usual
-parsedAddress4 = parser.runParser("Pennsylvania Avenue NW, Washington,") #will be faster as usual
+parsed_address1 = parser.parse_address("The White House 1600") #only first time will take few seconds to load
+parsed_address2 = parser.parse_address("Washington, DC 20500, USA") #will be faster as usual
+parsed_address3 = parser.parse_address(" 20500, USA") #will be faster as usual
+parsed_address4 = parser.parse_address("Pennsylvania Avenue NW, Washington,") #will be faster as usual
 ```
 ### 2. Expand the Address
 ```python
-expandAddress = parser.expandTheAddress("District Science Cntr, Kokkirakulam Rd, Tirunelveli, TamilNadu 627009")
-print(expandAddress)
+expanded_address = parser.expand_address("District Science Cntr, Kokkirakulam Rd, Tirunelveli, TamilNadu 627009")
+print(expanded_address)
 ```
 output
 ```sh
 ['district science center kokkirakulam road tirunelveli tamilnadu 627009',
  'district science connector kokkirakulam road tirunelveli tamilnadu 627009']
 ```
 
 
 ### 3. Terminate Address Parser Object
 ```python
-parser.terminateParser()
+parser.terminate_parser()
 ```
 
-
-
```

### Comparing `pypostalwin-0.0.3/pypostalwin/src/pypostalwin.egg-info/PKG-INFO` & `pypostalwin-0.0.4/pypostalwin/src/pypostalwin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: pypostalwin
-Version: 0.0.3
+Version: 0.0.4
 Summary:  python package for libpostal wrapper only for windows
 Home-page: https://github.com/selva221724/pypostalwin
-Author: Tamil Selvan A V
+Author: Tamil Selvan A V and Dominic Mukilan
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: IPython
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
@@ -32,27 +31,27 @@
 
 
 ## About libpostal
 libpostal is a C library for parsing/normalizing street addresses around the world using statistical NLP and open data. The goal of this project is to understand location-based strings in every language, everywhere.
 
 ## Installation
 
-### 1. Build the libpostal in windows
-- Before usign the Python wrapper, you need to build the libpostal C library as a bundle which can be accessed by the python package. (still under development) 
+### 1. Build the libpostal in Windows
+- Before using the Python wrapper, you need to build the libpostal C library as a bundle which can be accessed by the python package. (still under development) 
 
 (OR)
 
 - Download and Install [MSYS2](https://www.msys2.org/)
 - You can use the libpostal prebuilt zipped file [Download here](https://drive.google.com/file/d/1fZUlyLFCGYD7l_PDM0NzD8pAo-ICrVVd/view?usp=sharing)  
 - Unpack the zip to C:\Workbench\libpostal\
-- If you dont have **Workbench** folder in C Drive, then create one. 
+- If you don't have **Workbench** folder in C Drive, then create one. 
 - Copy the zip inside the **Workbench** and unzip using [7zip](https://www.7-zip.org/download.html) 
 
-### 2 . Install the python wrapper 
-**Install using pip** . [Offical Python Package Here!!](https://pypi.org/project/pypostalwin/)
+### 2. Install the python wrapper 
+**Install using pip**. [Offical Python Package Here!!](https://pypi.org/project/pypostalwin/)
 ```shell
 pip install pypostalwin
 ```
 
 (OR)
 
 Clone this Repository. Run this from the root directory to install
@@ -67,16 +66,16 @@
 ```python
 import pypostalwin
 ```
 
 ### 1. Initialize Address Parser Object
 ```python
 parser = pypostalwin.AddressParser()
-parsedAddress = parser.runParser("The White House 1600 Pennsylvania Avenue NW, Washington, DC 20500, USA")
-print(parsedAddress)
+parsed_address = parser.parse_address("The White House 1600 Pennsylvania Avenue NW, Washington, DC 20500, USA")
+print(parsed_address)
 ```
 output
 ```sh
 [
   {'house': 'the white house'}, 
   {'house_number': '1600'},
   {'road': 'pennsylvania avenue nw'}, 
@@ -89,31 +88,29 @@
 ```
 **Note:** In a single runtime, the first-time parser.runParser() will take a few seconds to run since it is loading the models from libpostal in the backend process. Once it is loaded, the recurrent runs will be faster as usual. You need to use the same object instance to get the results faster.
 
 for eg:
 
 ```python
 parser = pypostalwin.AddressParser()
-parsedAddress1 = parser.runParser("The White House 1600") #only first time will take few seconds to load
-parsedAddress2 = parser.runParser("Washington, DC 20500, USA") #will be faster as usual
-parsedAddress3 = parser.runParser(" 20500, USA") #will be faster as usual
-parsedAddress4 = parser.runParser("Pennsylvania Avenue NW, Washington,") #will be faster as usual
+parsed_address1 = parser.parse_address("The White House 1600") #only first time will take few seconds to load
+parsed_address2 = parser.parse_address("Washington, DC 20500, USA") #will be faster as usual
+parsed_address3 = parser.parse_address(" 20500, USA") #will be faster as usual
+parsed_address4 = parser.parse_address("Pennsylvania Avenue NW, Washington,") #will be faster as usual
 ```
 ### 2. Expand the Address
 ```python
-expandAddress = parser.expandTheAddress("District Science Cntr, Kokkirakulam Rd, Tirunelveli, TamilNadu 627009")
-print(expandAddress)
+expanded_address = parser.expand_address("District Science Cntr, Kokkirakulam Rd, Tirunelveli, TamilNadu 627009")
+print(expanded_address)
 ```
 output
 ```sh
 ['district science center kokkirakulam road tirunelveli tamilnadu 627009',
  'district science connector kokkirakulam road tirunelveli tamilnadu 627009']
 ```
 
 
 ### 3. Terminate Address Parser Object
 ```python
-parser.terminateParser()
+parser.terminate_parser()
 ```
 
-
-
```

### Comparing `pypostalwin-0.0.3/setup.py` & `pypostalwin-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypostalwin",  # This is the name of the package
-    version="0.0.3",  # The initial release version
-    author="Tamil Selvan A V",  # Full name of the author
+    version="0.0.4",  # The initial release version
+    author="Tamil Selvan A V and Dominic Mukilan",  # Full name of the author
     description=" python package for libpostal wrapper only for windows",
     url="https://github.com/selva221724/pypostalwin",
     license="MIT",
     include_package_data=True,
     long_description=long_description,  # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),  # List of all python modules to be installed
```

