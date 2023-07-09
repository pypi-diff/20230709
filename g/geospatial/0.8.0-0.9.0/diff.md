# Comparing `tmp/geospatial-0.8.0.tar.gz` & `tmp/geospatial-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geospatial-0.8.0.tar", last modified: Mon Apr 24 04:35:12 2023, max compression
+gzip compressed data, was "geospatial-0.9.0.tar", last modified: Sun Jul  9 02:30:37 2023, max compression
```

## Comparing `geospatial-0.8.0.tar` & `geospatial-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:35:12.863001 geospatial-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-24 04:35:01.000000 geospatial-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-24 04:35:01.000000 geospatial-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-24 04:35:12.863001 geospatial-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-24 04:35:01.000000 geospatial-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:35:12.863001 geospatial-0.8.0/geospatial/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-24 04:35:01.000000 geospatial-0.8.0/geospatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-24 04:35:01.000000 geospatial-0.8.0/geospatial/geospatial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:35:12.863001 geospatial-0.8.0/geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-24 04:35:12.000000 geospatial-0.8.0/geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-24 04:35:12.000000 geospatial-0.8.0/geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 04:35:12.000000 geospatial-0.8.0/geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 04:35:12.000000 geospatial-0.8.0/geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-24 04:35:12.000000 geospatial-0.8.0/geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 04:35:12.000000 geospatial-0.8.0/geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-24 04:35:01.000000 geospatial-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 04:35:12.863001 geospatial-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-24 04:35:01.000000 geospatial-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:30:37.450127 geospatial-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-09 02:30:24.000000 geospatial-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-09 02:30:24.000000 geospatial-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-09 02:30:37.450127 geospatial-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-09 02:30:24.000000 geospatial-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:30:37.450127 geospatial-0.9.0/geospatial/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-09 02:30:24.000000 geospatial-0.9.0/geospatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-09 02:30:24.000000 geospatial-0.9.0/geospatial/geospatial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 02:30:37.450127 geospatial-0.9.0/geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-09 02:30:37.000000 geospatial-0.9.0/geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-09 02:30:37.000000 geospatial-0.9.0/geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-09 02:30:37.000000 geospatial-0.9.0/geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 02:30:37.000000 geospatial-0.9.0/geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-09 02:30:37.000000 geospatial-0.9.0/geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 02:30:37.000000 geospatial-0.9.0/geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-09 02:30:24.000000 geospatial-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-09 02:30:37.450127 geospatial-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-09 02:30:24.000000 geospatial-0.9.0/setup.py
```

### Comparing `geospatial-0.8.0/LICENSE` & `geospatial-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geospatial-0.8.0/PKG-INFO` & `geospatial-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geospatial
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python package for installing commonly used packages for geospatial analysis and data visualization with only one command.
 Home-page: https://github.com/opengeos/geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: geospatial
 Classifier: Intended Audience :: Developers
```

### Comparing `geospatial-0.8.0/README.md` & `geospatial-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `geospatial-0.8.0/geospatial.egg-info/PKG-INFO` & `geospatial-0.9.0/geospatial.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geospatial
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python package for installing commonly used packages for geospatial analysis and data visualization with only one command.
 Home-page: https://github.com/opengeos/geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: geospatial
 Classifier: Intended Audience :: Developers
```

### Comparing `geospatial-0.8.0/geospatial.egg-info/dependency_links.txt` & `geospatial-0.9.0/requirements.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,64 @@
 # --find-links https://girder.github.io/large_image_wheels GDAL
 # cartopy; platform_platform != "Windows"
 bokeh
 cenpy
 contextily
+cubo
 dask-geopandas
 datashader
 earthengine-api
 earthpy
 easystac
 eemont
 # eomaps
 eoreader
+fiona
 folium>=0.12.1
-geemap>=0.13.7
-gemgis
+geemap>=0.24.0
+# gemgis
 geoalchemy2
 geocube
 geopandas
+geotiff
 # geosnap
 # geoviews
 h3
-here-map-widget-for-jupyter
 hvplot
 ipygany
 ipyleaflet
 ipyvtklink
 keplergl
 laspy
-leafmap>=0.9.3
+leafmap>=0.22.0
 # lidar
-localtileserver>=0.5.8
+localtileserver>=0.6.1
 mapboxgl
+mapclassify
 mapwidget
 # movingpandas
 mss
 netcdf4
+networkx
 odc-stac
 osmnx
 owslib
 panel
 palettable
 planetary-computer
 plotly
 proplot
 psycopg2
 pydeck
-pygis>=0.3.1
+pygis>=0.6.0
 pyntcloud
-# pysal
+pyproj
+pysal
+pyshp
+pystac-client
 # pyvista
 radiant-mlhub
 rasterio
 rasterstats
 rio-cogeo
 rioxarray
 s2cloudless
@@ -61,11 +68,17 @@
 shapely
 simplekml
 sliderule
 spyndex
 sqlalchemy
 stackstac
 # tropycal
+usgs
+whitebox
+whiteboxgui
+wxee
+xarray
+xarray_leaflet
 xarray-spatial
+# xcube; python_version >= '3.9'
 # xmovie
-wxee
-
+xyzservices
```

### Comparing `geospatial-0.8.0/geospatial.egg-info/requires.txt` & `geospatial-0.9.0/geospatial.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 bokeh
 cenpy
 contextily
+cubo
 dask-geopandas
 datashader
 earthengine-api
 earthpy
 easystac
 eemont
 eoreader
+fiona
 folium>=0.12.1
-geemap>=0.13.7
-gemgis
+geemap>=0.24.0
 geoalchemy2
 geocube
 geopandas
+geotiff
 h3
-here-map-widget-for-jupyter
 hvplot
 ipygany
 ipyleaflet
 ipyvtklink
 keplergl
 laspy
-leafmap>=0.9.3
-localtileserver>=0.5.8
+leafmap>=0.22.0
+localtileserver>=0.6.1
 mapboxgl
+mapclassify
 mapwidget
 mss
 netcdf4
+networkx
 odc-stac
 osmnx
 owslib
 panel
 palettable
 planetary-computer
 plotly
 proplot
 psycopg2
 pydeck
-pygis>=0.3.1
+pygis>=0.6.0
 pyntcloud
+pyproj
+pysal
+pyshp
+pystac-client
 radiant-mlhub
 rasterio
 rasterstats
 rio-cogeo
 rioxarray
 s2cloudless
 sarpy
@@ -51,9 +58,15 @@
 sentinelsat
 shapely
 simplekml
 sliderule
 spyndex
 sqlalchemy
 stackstac
-xarray-spatial
+usgs
+whitebox
+whiteboxgui
 wxee
+xarray
+xarray_leaflet
+xarray-spatial
+xyzservices
```

### Comparing `geospatial-0.8.0/requirements.txt` & `geospatial-0.9.0/geospatial.egg-info/dependency_links.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,64 @@
 # --find-links https://girder.github.io/large_image_wheels GDAL
 # cartopy; platform_platform != "Windows"
 bokeh
 cenpy
 contextily
+cubo
 dask-geopandas
 datashader
 earthengine-api
 earthpy
 easystac
 eemont
 # eomaps
 eoreader
+fiona
 folium>=0.12.1
-geemap>=0.13.7
-gemgis
+geemap>=0.24.0
+# gemgis
 geoalchemy2
 geocube
 geopandas
+geotiff
 # geosnap
 # geoviews
 h3
-here-map-widget-for-jupyter
 hvplot
 ipygany
 ipyleaflet
 ipyvtklink
 keplergl
 laspy
-leafmap>=0.9.3
+leafmap>=0.22.0
 # lidar
-localtileserver>=0.5.8
+localtileserver>=0.6.1
 mapboxgl
+mapclassify
 mapwidget
 # movingpandas
 mss
 netcdf4
+networkx
 odc-stac
 osmnx
 owslib
 panel
 palettable
 planetary-computer
 plotly
 proplot
 psycopg2
 pydeck
-pygis>=0.3.1
+pygis>=0.6.0
 pyntcloud
-# pysal
+pyproj
+pysal
+pyshp
+pystac-client
 # pyvista
 radiant-mlhub
 rasterio
 rasterstats
 rio-cogeo
 rioxarray
 s2cloudless
@@ -61,10 +68,18 @@
 shapely
 simplekml
 sliderule
 spyndex
 sqlalchemy
 stackstac
 # tropycal
+usgs
+whitebox
+whiteboxgui
+wxee
+xarray
+xarray_leaflet
 xarray-spatial
+# xcube; python_version >= '3.9'
 # xmovie
-wxee
+xyzservices
+
```

### Comparing `geospatial-0.8.0/setup.py` & `geospatial-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,10 +47,10 @@
     keywords='geospatial',
     name='geospatial',
     packages=find_packages(include=['geospatial', 'geospatial.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/opengeos/geospatial',
-    version='0.8.0',
+    version='0.9.0',
     zip_safe=False,
 )
```

