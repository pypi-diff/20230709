# Comparing `tmp/cubo-0.1.0.tar.gz` & `tmp/cubo-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubo-0.1.0.tar", last modified: Thu Feb 16 09:49:15 2023, max compression
+gzip compressed data, was "cubo-2023.7.0.tar", last modified: Sun Jul  9 12:42:25 2023, max compression
```

## Comparing `cubo-0.1.0.tar` & `cubo-2023.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-02-16 09:49:15.719401 cubo-0.1.0/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2023-02-12 12:44:23.000000 cubo-0.1.0/LICENSE
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7383 2023-02-16 09:49:15.719401 cubo-0.1.0/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     6757 2023-02-14 14:16:54.000000 cubo-0.1.0/README.md
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-02-16 09:49:15.719401 cubo-0.1.0/cubo/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      175 2023-02-14 10:09:28.000000 cubo-0.1.0/cubo/__init__.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     4004 2023-02-15 12:24:19.000000 cubo-0.1.0/cubo/cubo.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2406 2023-02-13 17:03:14.000000 cubo-0.1.0/cubo/utils.py
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-02-16 09:49:15.719401 cubo-0.1.0/cubo.egg-info/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7383 2023-02-16 09:49:15.000000 cubo-0.1.0/cubo.egg-info/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      209 2023-02-16 09:49:15.000000 cubo-0.1.0/cubo.egg-info/SOURCES.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-02-16 09:49:15.000000 cubo-0.1.0/cubo.egg-info/dependency_links.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)       94 2023-02-16 09:49:15.000000 cubo-0.1.0/cubo.egg-info/requires.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        5 2023-02-16 09:49:15.000000 cubo-0.1.0/cubo.egg-info/top_level.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-02-16 09:49:15.719401 cubo-0.1.0/setup.cfg
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1354 2023-02-14 10:09:28.000000 cubo-0.1.0/setup.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-09 12:42:25.384298 cubo-2023.7.0/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2023-07-09 12:31:14.000000 cubo-2023.7.0/LICENSE
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7699 2023-07-09 12:42:25.384298 cubo-2023.7.0/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7050 2023-07-09 12:31:14.000000 cubo-2023.7.0/README.md
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-09 12:42:25.380965 cubo-2023.7.0/cubo/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      178 2023-07-09 12:33:10.000000 cubo-2023.7.0/cubo/__init__.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     4004 2023-07-09 12:31:14.000000 cubo-2023.7.0/cubo/cubo.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2401 2023-07-09 12:31:14.000000 cubo-2023.7.0/cubo/utils.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-09 12:42:25.384298 cubo-2023.7.0/cubo.egg-info/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7699 2023-07-09 12:42:25.000000 cubo-2023.7.0/cubo.egg-info/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      209 2023-07-09 12:42:25.000000 cubo-2023.7.0/cubo.egg-info/SOURCES.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-07-09 12:42:25.000000 cubo-2023.7.0/cubo.egg-info/dependency_links.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      110 2023-07-09 12:42:25.000000 cubo-2023.7.0/cubo.egg-info/requires.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        5 2023-07-09 12:42:25.000000 cubo-2023.7.0/cubo.egg-info/top_level.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-07-09 12:42:25.384298 cubo-2023.7.0/setup.cfg
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1340 2023-07-09 12:31:42.000000 cubo-2023.7.0/setup.py
```

### Comparing `cubo-0.1.0/LICENSE` & `cubo-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cubo-0.1.0/PKG-INFO` & `cubo-2023.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cubo
-Version: 0.1.0
+Version: 2023.7.0
 Summary: Easily create EO mini cubes from STAC in Python
 Home-page: https://github.com/davemlz/cubo
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -193,7 +194,15 @@
     query={"eo:cloud_cover": {"lt": 10}} # kwarg to pass
 )
 ```
 
 ## License
 
 The project is licensed under the MIT license.
+
+## Logo Attribution
+
+The logo and images were created using <a href="https://www.flaticon.com/free-icons/dice" title="dice icons">dice icons created by Freepik - Flaticon</a>.
+
+[![RSC4Earth](https://github.com/davemlz/cubo/raw/main/docs/_static/esds.png)](https://rsc4earth.de/authors/esds/)
+
+
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: cubo Version: 0.1.0 Summary: Easily create EO mini
-cubes from STAC in Python Home-page: https://github.com/davemlz/cubo Author:
-David Montero Loaiza Author-email: dml.mont@gmail.com License: MIT Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: License :: OSI Approved :: MIT
-License Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Description-Content-Type: text/markdown License-File:
-LICENSE
+Metadata-Version: 2.1 Name: cubo Version: 2023.7.0 Summary: Easily create EO
+mini cubes from STAC in Python Home-page: https://github.com/davemlz/cubo
+Author: David Montero Loaiza Author-email: dml.mont@gmail.com License: MIT
+Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
+text/markdown License-File: LICENSE
                                     [cubo]
                 Easily create EO mini cubes from STAC in Python
 [PyPI] [conda-forge] [Documentation_Status] [Tests] [License] [GitHub_Sponsors]
               [Buy_me_a_coffee] [Ko-fi] [Twitter] [Black] [isort]
 --- **GitHub**: [https://github.com/davemlz/cubo](https://github.com/davemlz/
 cubo) **Documentation**: [https://cubo.readthedocs.io/](https://
 cubo.readthedocs.io/) **PyPI**: [https://pypi.org/project/cubo/](https://
@@ -67,8 +67,11 @@
 collection="sentinel-s2-l2a-cogs", bands=["B05","B06","B07"], start_date="2020-
 01-01", end_date="2020-06-01", edge_size=128, resolution=20, stac="https://
 earth-search.aws.element84.com/v0" ) ``` ### Keywords for searching data You
 can pass `kwargs` to `pystac_client.Client.search()` if required: ```python da
 = cubo.create( lat=4.31, lon=-76.2, collection="sentinel-2-l2a", bands=
 ["B02","B03","B04"], start_date="2021-01-01", end_date="2021-06-10",
 edge_size=64, resolution=10, query={"eo:cloud_cover": {"lt": 10}} # kwarg to
-pass ) ``` ## License The project is licensed under the MIT license.
+pass ) ``` ## License The project is licensed under the MIT license. ## Logo
+Attribution The logo and images were created using dice_icons_created_by
+Freepik_-_Flaticon. [![RSC4Earth](https://github.com/davemlz/cubo/raw/main/
+docs/_static/esds.png)](https://rsc4earth.de/authors/esds/)
```

### Comparing `cubo-0.1.0/README.md` & `cubo-2023.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -175,7 +175,13 @@
     query={"eo:cloud_cover": {"lt": 10}} # kwarg to pass
 )
 ```
 
 ## License
 
 The project is licensed under the MIT license.
+
+## Logo Attribution
+
+The logo and images were created using <a href="https://www.flaticon.com/free-icons/dice" title="dice icons">dice icons created by Freepik - Flaticon</a>.
+
+[![RSC4Earth](https://github.com/davemlz/cubo/raw/main/docs/_static/esds.png)](https://rsc4earth.de/authors/esds/)
```

#### html2text {}

```diff
@@ -58,8 +58,11 @@
 collection="sentinel-s2-l2a-cogs", bands=["B05","B06","B07"], start_date="2020-
 01-01", end_date="2020-06-01", edge_size=128, resolution=20, stac="https://
 earth-search.aws.element84.com/v0" ) ``` ### Keywords for searching data You
 can pass `kwargs` to `pystac_client.Client.search()` if required: ```python da
 = cubo.create( lat=4.31, lon=-76.2, collection="sentinel-2-l2a", bands=
 ["B02","B03","B04"], start_date="2021-01-01", end_date="2021-06-10",
 edge_size=64, resolution=10, query={"eo:cloud_cover": {"lt": 10}} # kwarg to
-pass ) ``` ## License The project is licensed under the MIT license.
+pass ) ``` ## License The project is licensed under the MIT license. ## Logo
+Attribution The logo and images were created using dice_icons_created_by
+Freepik_-_Flaticon. [![RSC4Earth](https://github.com/davemlz/cubo/raw/main/
+docs/_static/esds.png)](https://rsc4earth.de/authors/esds/)
```

### Comparing `cubo-0.1.0/cubo/cubo.py` & `cubo-2023.7.0/cubo/cubo.py`

 * *Files identical despite different names*

### Comparing `cubo-0.1.0/cubo/utils.py` & `cubo-2023.7.0/cubo/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,8 +84,8 @@
 
     # Create latlon BBox
     bbox_latlon = {
         "type": "Polygon",
         "coordinates": [polygon_latlon],
     }
 
-    return (bbox_utm, bbox_latlon, utm_coords, f"EPSG:{epsg}")
+    return (bbox_utm, bbox_latlon, utm_coords, int(epsg))
```

### Comparing `cubo-0.1.0/cubo.egg-info/PKG-INFO` & `cubo-2023.7.0/cubo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cubo
-Version: 0.1.0
+Version: 2023.7.0
 Summary: Easily create EO mini cubes from STAC in Python
 Home-page: https://github.com/davemlz/cubo
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -193,7 +194,15 @@
     query={"eo:cloud_cover": {"lt": 10}} # kwarg to pass
 )
 ```
 
 ## License
 
 The project is licensed under the MIT license.
+
+## Logo Attribution
+
+The logo and images were created using <a href="https://www.flaticon.com/free-icons/dice" title="dice icons">dice icons created by Freepik - Flaticon</a>.
+
+[![RSC4Earth](https://github.com/davemlz/cubo/raw/main/docs/_static/esds.png)](https://rsc4earth.de/authors/esds/)
+
+
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: cubo Version: 0.1.0 Summary: Easily create EO mini
-cubes from STAC in Python Home-page: https://github.com/davemlz/cubo Author:
-David Montero Loaiza Author-email: dml.mont@gmail.com License: MIT Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: License :: OSI Approved :: MIT
-License Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Description-Content-Type: text/markdown License-File:
-LICENSE
+Metadata-Version: 2.1 Name: cubo Version: 2023.7.0 Summary: Easily create EO
+mini cubes from STAC in Python Home-page: https://github.com/davemlz/cubo
+Author: David Montero Loaiza Author-email: dml.mont@gmail.com License: MIT
+Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
+text/markdown License-File: LICENSE
                                     [cubo]
                 Easily create EO mini cubes from STAC in Python
 [PyPI] [conda-forge] [Documentation_Status] [Tests] [License] [GitHub_Sponsors]
               [Buy_me_a_coffee] [Ko-fi] [Twitter] [Black] [isort]
 --- **GitHub**: [https://github.com/davemlz/cubo](https://github.com/davemlz/
 cubo) **Documentation**: [https://cubo.readthedocs.io/](https://
 cubo.readthedocs.io/) **PyPI**: [https://pypi.org/project/cubo/](https://
@@ -67,8 +67,11 @@
 collection="sentinel-s2-l2a-cogs", bands=["B05","B06","B07"], start_date="2020-
 01-01", end_date="2020-06-01", edge_size=128, resolution=20, stac="https://
 earth-search.aws.element84.com/v0" ) ``` ### Keywords for searching data You
 can pass `kwargs` to `pystac_client.Client.search()` if required: ```python da
 = cubo.create( lat=4.31, lon=-76.2, collection="sentinel-2-l2a", bands=
 ["B02","B03","B04"], start_date="2021-01-01", end_date="2021-06-10",
 edge_size=64, resolution=10, query={"eo:cloud_cover": {"lt": 10}} # kwarg to
-pass ) ``` ## License The project is licensed under the MIT license.
+pass ) ``` ## License The project is licensed under the MIT license. ## Logo
+Attribution The logo and images were created using dice_icons_created_by
+Freepik_-_Flaticon. [![RSC4Earth](https://github.com/davemlz/cubo/raw/main/
+docs/_static/esds.png)](https://rsc4earth.de/authors/esds/)
```

