# Comparing `tmp/pix2vec-0.1.2.tar.gz` & `tmp/pix2vec-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pix2vec-0.1.2.tar", last modified: Sun Jun 25 19:42:24 2023, max compression
+gzip compressed data, was "pix2vec-0.1.3.tar", last modified: Sun Jul  9 06:04:32 2023, max compression
```

## Comparing `pix2vec-0.1.2.tar` & `pix2vec-0.1.3.tar`

### file list

```diff
@@ -1,54 +1,58 @@
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/
--rw-r--r--   0 alf        (501) staff       (20)     6264 2023-06-25 19:42:24.000000 pix2vec-0.1.2/PKG-INFO
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/pix2vec.egg-info/
--rw-r--r--   0 alf        (501) staff       (20)     6264 2023-06-25 19:42:24.000000 pix2vec-0.1.2/pix2vec.egg-info/PKG-INFO
--rw-r--r--   0 alf        (501) staff       (20)        1 2023-06-21 09:26:55.000000 pix2vec-0.1.2/pix2vec.egg-info/not-zip-safe
--rw-r--r--   0 alf        (501) staff       (20)      874 2023-06-25 19:42:24.000000 pix2vec-0.1.2/pix2vec.egg-info/SOURCES.txt
--rw-r--r--   0 alf        (501) staff       (20)       46 2023-06-25 19:42:24.000000 pix2vec-0.1.2/pix2vec.egg-info/entry_points.txt
--rw-r--r--   0 alf        (501) staff       (20)        8 2023-06-25 19:42:24.000000 pix2vec-0.1.2/pix2vec.egg-info/top_level.txt
--rw-r--r--   0 alf        (501) staff       (20)        1 2023-06-25 19:42:24.000000 pix2vec-0.1.2/pix2vec.egg-info/dependency_links.txt
--rw-r--r--   0 alf        (501) staff       (20)     1564 2023-06-21 09:12:34.000000 pix2vec-0.1.2/LICENSE
--rw-r--r--   0 alf        (501) staff       (20)     3524 2023-06-22 08:52:00.000000 pix2vec-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 alf        (501) staff       (20)     2295 2023-06-21 09:12:34.000000 pix2vec-0.1.2/Makefile
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/tests/
--rw-r--r--   0 alf        (501) staff       (20)       37 2023-06-21 09:12:34.000000 pix2vec-0.1.2/tests/__init__.py
--rw-r--r--   0 alf        (501) staff       (20)      387 2023-06-21 09:12:34.000000 pix2vec-0.1.2/tests/test_pix2vec.py
--rw-r--r--   0 alf        (501) staff       (20)      262 2023-06-21 09:12:34.000000 pix2vec-0.1.2/MANIFEST.in
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/docs/
--rw-r--r--   0 alf        (501) staff       (20)      552 2023-06-23 21:34:41.000000 pix2vec-0.1.2/docs/index.rst
--rw-r--r--   0 alf        (501) staff       (20)       33 2023-06-21 09:12:34.000000 pix2vec-0.1.2/docs/contributing.rst
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/docs/images/
--rw-r--r--   0 alf        (501) staff       (20)   948490 2023-06-23 18:50:51.000000 pix2vec-0.1.2/docs/images/m3cube-c.png
--rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.2/docs/images/m3cube-a.png
--rw-r--r--   0 alf        (501) staff       (20)   337959 2023-06-23 23:06:07.000000 pix2vec-0.1.2/docs/images/m3-detail.png
--rw-r--r--   0 alf        (501) staff       (20)   339139 2023-06-23 23:06:07.000000 pix2vec-0.1.2/docs/images/m3-PixelValue.png
--rw-r--r--   0 alf        (501) staff       (20)      608 2023-06-21 09:12:34.000000 pix2vec-0.1.2/docs/Makefile
--rwxr-xr-x   0 alf        (501) staff       (20)     4876 2023-06-21 10:42:06.000000 pix2vec-0.1.2/docs/conf.py
--rw-r--r--   0 alf        (501) staff       (20)       58 2023-06-23 20:25:10.000000 pix2vec-0.1.2/docs/modules.rst
--rw-r--r--   0 alf        (501) staff       (20)      181 2023-06-21 14:04:55.000000 pix2vec-0.1.2/docs/usage.rst
--rw-r--r--   0 alf        (501) staff       (20)      805 2023-06-21 09:12:34.000000 pix2vec-0.1.2/docs/make.bat
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/docs/_build/
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/docs/_build/html/
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/docs/_build/html/_static/
--rw-r--r--   0 alf        (501) staff       (20)       90 2021-10-12 12:18:02.000000 pix2vec-0.1.2/docs/_build/html/_static/plus.png
--rw-r--r--   0 alf        (501) staff       (20)      286 2021-10-12 12:18:02.000000 pix2vec-0.1.2/docs/_build/html/_static/file.png
--rw-r--r--   0 alf        (501) staff       (20)       90 2021-10-12 12:18:02.000000 pix2vec-0.1.2/docs/_build/html/_static/minus.png
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/docs/_build/html/_images/
--rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.2/docs/_build/html/_images/m3cube-a.png
--rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.2/docs/history.rst
--rw-r--r--   0 alf        (501) staff       (20)     1114 2023-06-22 08:51:18.000000 pix2vec-0.1.2/docs/installation.rst
--rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.2/docs/authors.rst
--rw-r--r--   0 alf        (501) staff       (20)       27 2023-06-21 09:12:34.000000 pix2vec-0.1.2/docs/readme.rst
--rw-r--r--   0 alf        (501) staff       (20)      423 2023-06-23 20:25:10.000000 pix2vec-0.1.2/docs/pix2vec.rst
--rw-r--r--   0 alf        (501) staff       (20)     1583 2023-06-25 19:42:22.000000 pix2vec-0.1.2/setup.py
--rw-r--r--   0 alf        (501) staff       (20)      351 2023-06-25 19:40:58.000000 pix2vec-0.1.2/HISTORY.rst
--rw-r--r--   0 alf        (501) staff       (20)      268 2023-06-21 09:12:34.000000 pix2vec-0.1.2/tox.ini
--rw-r--r--   0 alf        (501) staff       (20)      212 2023-06-21 09:38:53.000000 pix2vec-0.1.2/AUTHORS.rst
--rw-r--r--   0 alf        (501) staff       (20)      379 2023-06-25 19:42:24.000000 pix2vec-0.1.2/setup.cfg
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/pix2vec/
--rw-r--r--   0 alf        (501) staff       (20)      202 2023-06-25 15:07:15.000000 pix2vec-0.1.2/pix2vec/__init__.py
--rw-r--r--   0 alf        (501) staff       (20)     2012 2023-06-23 21:09:46.000000 pix2vec-0.1.2/pix2vec/cli.py
--rw-r--r--   0 alf        (501) staff       (20)     8802 2023-06-23 21:01:11.000000 pix2vec-0.1.2/pix2vec/pix2vec.py
--rw-r--r--   0 alf        (501) staff       (20)     3946 2023-06-25 19:38:29.000000 pix2vec-0.1.2/README.rst
--rw-r--r--   0 alf        (501) staff       (20)      205 2023-06-21 10:32:57.000000 pix2vec-0.1.2/.readthedocs.yaml
--rw-r--r--   0 alf        (501) staff       (20)      185 2023-06-23 19:30:11.000000 pix2vec-0.1.2/requirements_dev.txt
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.056028 pix2vec-0.1.3/
+-rw-r--r--   0 alf        (501) staff       (20)     1204 2023-06-21 09:12:34.000000 pix2vec-0.1.3/.gitignore
+-rw-r--r--   0 alf        (501) staff       (20)      205 2023-06-21 10:32:57.000000 pix2vec-0.1.3/.readthedocs.yaml
+-rw-r--r--   0 alf        (501) staff       (20)      593 2023-07-09 06:02:38.000000 pix2vec-0.1.3/.zenodo.json
+-rw-r--r--   0 alf        (501) staff       (20)      212 2023-06-21 09:38:53.000000 pix2vec-0.1.3/AUTHORS.rst
+-rw-r--r--   0 alf        (501) staff       (20)      284 2023-07-07 14:13:32.000000 pix2vec-0.1.3/CITATION.cff
+-rw-r--r--   0 alf        (501) staff       (20)     3524 2023-06-22 08:52:00.000000 pix2vec-0.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 alf        (501) staff       (20)      429 2023-07-09 06:04:28.000000 pix2vec-0.1.3/HISTORY.rst
+-rw-r--r--   0 alf        (501) staff       (20)     1564 2023-06-21 09:12:34.000000 pix2vec-0.1.3/LICENSE
+-rw-r--r--   0 alf        (501) staff       (20)      262 2023-06-21 09:12:34.000000 pix2vec-0.1.3/MANIFEST.in
+-rw-r--r--   0 alf        (501) staff       (20)     2295 2023-06-21 09:12:34.000000 pix2vec-0.1.3/Makefile
+-rw-r--r--   0 alf        (501) staff       (20)     5430 2023-07-09 06:04:32.056266 pix2vec-0.1.3/PKG-INFO
+-rw-r--r--   0 alf        (501) staff       (20)     4034 2023-07-09 05:59:59.000000 pix2vec-0.1.3/README.rst
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.039224 pix2vec-0.1.3/docs/
+-rw-r--r--   0 alf        (501) staff       (20)      608 2023-06-21 09:12:34.000000 pix2vec-0.1.3/docs/Makefile
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.021183 pix2vec-0.1.3/docs/_build/
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.021665 pix2vec-0.1.3/docs/_build/html/
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.039730 pix2vec-0.1.3/docs/_build/html/_images/
+-rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.3/docs/_build/html/_images/m3cube-a.png
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.042428 pix2vec-0.1.3/docs/_build/html/_static/
+-rw-r--r--   0 alf        (501) staff       (20)      286 2021-10-12 12:18:02.000000 pix2vec-0.1.3/docs/_build/html/_static/file.png
+-rw-r--r--   0 alf        (501) staff       (20)       90 2021-10-12 12:18:02.000000 pix2vec-0.1.3/docs/_build/html/_static/minus.png
+-rw-r--r--   0 alf        (501) staff       (20)       90 2021-10-12 12:18:02.000000 pix2vec-0.1.3/docs/_build/html/_static/plus.png
+-rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.3/docs/authors.rst
+-rwxr-xr-x   0 alf        (501) staff       (20)     4876 2023-06-21 10:42:06.000000 pix2vec-0.1.3/docs/conf.py
+-rw-r--r--   0 alf        (501) staff       (20)       33 2023-06-21 09:12:34.000000 pix2vec-0.1.3/docs/contributing.rst
+-rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.3/docs/history.rst
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.047296 pix2vec-0.1.3/docs/images/
+-rw-r--r--   0 alf        (501) staff       (20)   339139 2023-06-23 23:06:07.000000 pix2vec-0.1.3/docs/images/m3-PixelValue.png
+-rw-r--r--   0 alf        (501) staff       (20)   337959 2023-06-23 23:06:07.000000 pix2vec-0.1.3/docs/images/m3-detail.png
+-rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.3/docs/images/m3cube-a.png
+-rw-r--r--   0 alf        (501) staff       (20)   948490 2023-06-23 18:50:51.000000 pix2vec-0.1.3/docs/images/m3cube-c.png
+-rw-r--r--   0 alf        (501) staff       (20)      552 2023-06-23 21:34:41.000000 pix2vec-0.1.3/docs/index.rst
+-rw-r--r--   0 alf        (501) staff       (20)     1114 2023-06-22 08:51:18.000000 pix2vec-0.1.3/docs/installation.rst
+-rw-r--r--   0 alf        (501) staff       (20)      805 2023-06-21 09:12:34.000000 pix2vec-0.1.3/docs/make.bat
+-rw-r--r--   0 alf        (501) staff       (20)       58 2023-06-23 20:25:10.000000 pix2vec-0.1.3/docs/modules.rst
+-rw-r--r--   0 alf        (501) staff       (20)      423 2023-06-23 20:25:10.000000 pix2vec-0.1.3/docs/pix2vec.rst
+-rw-r--r--   0 alf        (501) staff       (20)       27 2023-06-21 09:12:34.000000 pix2vec-0.1.3/docs/readme.rst
+-rw-r--r--   0 alf        (501) staff       (20)      181 2023-06-21 14:04:55.000000 pix2vec-0.1.3/docs/usage.rst
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.051509 pix2vec-0.1.3/pix2vec/
+-rw-r--r--   0 alf        (501) staff       (20)      404 2023-06-26 16:37:14.000000 pix2vec-0.1.3/pix2vec/__init__.py
+-rw-r--r--   0 alf        (501) staff       (20)     2086 2023-06-26 16:37:03.000000 pix2vec-0.1.3/pix2vec/cli.py
+-rw-r--r--   0 alf        (501) staff       (20)     8802 2023-06-23 21:01:11.000000 pix2vec-0.1.3/pix2vec/pix2vec.py
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.054669 pix2vec-0.1.3/pix2vec.egg-info/
+-rw-r--r--   0 alf        (501) staff       (20)     5430 2023-07-09 06:04:31.000000 pix2vec-0.1.3/pix2vec.egg-info/PKG-INFO
+-rw-r--r--   0 alf        (501) staff       (20)      928 2023-07-09 06:04:31.000000 pix2vec-0.1.3/pix2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 alf        (501) staff       (20)        1 2023-07-09 06:04:31.000000 pix2vec-0.1.3/pix2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 alf        (501) staff       (20)       45 2023-07-09 06:04:31.000000 pix2vec-0.1.3/pix2vec.egg-info/entry_points.txt
+-rw-r--r--   0 alf        (501) staff       (20)        1 2023-06-21 09:26:55.000000 pix2vec-0.1.3/pix2vec.egg-info/not-zip-safe
+-rw-r--r--   0 alf        (501) staff       (20)        8 2023-07-09 06:04:31.000000 pix2vec-0.1.3/pix2vec.egg-info/top_level.txt
+-rw-r--r--   0 alf        (501) staff       (20)       32 2023-06-23 19:30:18.000000 pix2vec-0.1.3/requirements.txt
+-rw-r--r--   0 alf        (501) staff       (20)      185 2023-06-23 19:30:11.000000 pix2vec-0.1.3/requirements_dev.txt
+-rw-r--r--   0 alf        (501) staff       (20)      379 2023-07-09 06:04:32.057340 pix2vec-0.1.3/setup.cfg
+-rw-r--r--   0 alf        (501) staff       (20)     1625 2023-07-09 05:51:07.000000 pix2vec-0.1.3/setup.py
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-07-09 06:04:32.055622 pix2vec-0.1.3/tests/
+-rw-r--r--   0 alf        (501) staff       (20)       37 2023-06-21 09:12:34.000000 pix2vec-0.1.3/tests/__init__.py
+-rw-r--r--   0 alf        (501) staff       (20)      387 2023-06-21 09:12:34.000000 pix2vec-0.1.3/tests/test_pix2vec.py
+-rw-r--r--   0 alf        (501) staff       (20)      268 2023-06-21 09:12:34.000000 pix2vec-0.1.3/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pix2vec-0.1.2/PKG-INFO` & `pix2vec-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,153 +1,160 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pix2vec
-Version: 0.1.2
-Summary: pix2vec produces a vector representation of planetary mapping spectrometers starting from hyperspectral an ISIS data cube
+Version: 0.1.3
+Summary: pix2vec produces a vector representation of planetary mapping spectrometers hyperspectral and camera ISIS data cube
 Home-page: https://github.com/afrigeri/pix2vec
 Author: Alessandro Frigeri
 Author-email: alessandro.frigeri@inaf.it
 License: GNU General Public License v3
-Description: ===============
-        pix2vec
-        ===============
-        *Geospatial Vector Representation of Planetary Remote Sensing Hyperspectral Data*
-        
-        ---------------------------------
-        
-        
-        .. image:: https://img.shields.io/pypi/v/pix2vec.svg
-                :target: https://pypi.python.org/pypi/pix2vec
-        
-        .. image:: https://readthedocs.org/projects/pix2vec/badge/?version=latest
-                :target: https://pix2vec.readthedocs.io/en/latest/?version=latest
-                :alt: Documentation Status
-        
-        pix2vec: Vector Representation of Planetary Hyperspectral Data Cubes
-        
-        
-        * Free software: GNU General Public License v3
-        * Documentation: https://pix2vec.readthedocs.io.
-        
-        
-        Features
-        --------
-        
-        * Produces a vector representation of the raster representation of HSI data 'cubes' generated by ISIS
-        
-        Requirements
-        ------------
-        
-        * a relatively recent `Integrated Software for Imagers and Spectrometers (ISIS) <https://isis.astrogeology.usgs.gov>`_ installation and the `kalasiris <https://github.com/rbeyer/kalasiris>`_ module (which will be installed automatically).
-         
-        Cite in your work
-        -------------------
-        
-        Frigeri, A. and Hare, T. 2023. Geospatial Vector Representation of 
-        Planetary Mapping Spectrometer Data. 6th Planetay Data Workshop, Flagstaff, Arizona 26-28th June 2023, Abstract #7088.::
-        
-         @INPROCEEDINGS{FrigeriHare2023,
-               author = {{Frigeri}, A. and {Hare}, T.},
-                title = "{Geospatial Vector Representation of Planetary Mapping Spectrometer Data}",
-            booktitle = {6th Planetay Data Workshop},
-                 year = 2023,
-               series = {LPI},
-                month = jun,
-                  eid = {7088},
-                pages = {7088}
-         }
-        
-        
-        installation
-        ------------
-        
-        within a working ISIS environment, run::
-        
-            pip install pix2vect
-        
-        
-        
-        pix2vec in brief
-        -----------------
-        
-        `pix2vect` requires spice-initialized ISIS cubes (see `spiceinit`).  
-        
-        Let's start with an hyperspectral cube from the The Moon Mineralogy Mapper (M3), the NASA spectrometer onboard  Chandrayaan-1 mission to the Moon::
-        
-            (ISIS) $ pix2vec -i -c M3G20090103T084105_V03_L1B.cub 
-            pix2vect - 2023 Alessandro Frigeri - Istituto Nazionale di Astrofisica
-            Cube Type:M3 samples:304 lines:11739 file:M3G20090103T084105_V03_L1B.cub
-        
-        now we create a vector GIS file representing the geometry of the sensor's pixel on the lunar surface::
-        
-            pix2vec -c M3G20090103T084105_V03_L1B.cub -s 1,150 -l 3050,3200 -o M3G20090103T084105_V03_L1B_subset.gpkg 
-        
-        the vector file can then be loaded in your favorite GIS, and we can plot the file with a `PixelValue` greyscale:
-        
-        .. image:: /docs/images/m3-PixelValue.png
-                :alt: M3-PixelValue
-                :width: 600
-        
-        each ground pixel element holds information that can be accessed:
-        
-        .. image:: /docs/images/m3-detail.png
-                :alt: M3-subcube
-                :width: 600
-        
-        for each ground-projected pixel, you now have access to these fields::
-        
-        	Filename Sample Line PixelValue RightAscension Declination 
-        	PlanetocentricLatitude PlanetographicLatitude PositiveEast360Longitude 
-        	PositiveEast180Longitude PositiveWest360Longitude PositiveWest180Longitude 
-        	BodyFixedCoordinateX BodyFixedCoordinateY BodyFixedCoordinateZ LocalRadius 
-        	SampleResolution LineResolution SpacecraftPositionX SpacecraftPositionY 
-        	SpacecraftPositionZ SpacecraftAzimuth SlantDistance TargetCenterDistance 
-        	SubSpacecraftLatitude SubSpacecraftLongitude SpacecraftAltitude OffNadirAngle 
-        	SubSpacecraftGroundAzimuth SunPositionX SunPositionY SunPositionZ 
-        	SubSolarAzimuth SolarDistance SubSolarLatitude SubSolarLongitude 
-        	SubSolarGroundAzimuth Phase Incidence Emission NorthAzimuth EphemerisTime UTC 
-        	LocalSolarTime SolarLongitude LookDirectionBodyFixedX LookDirectionBodyFixedY 
-        	LookDirectionBodyFixedZ LookDirectionJ2000X LookDirectionJ2000Y 
-        	LookDirectionJ2000Z LookDirectionCameraX LookDirectionCameraY 
-        	LookDirectionCameraZ ObliqueDetectorResolution ObliquePixelResolution 
-        	ObliqueLineResolution ObliqueSampleResolution Error
-        
-        
-        Documentation
-        -------------
-        
-        Documentation is available at https://pix2vec.readthedocs.io
-        
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.2 (2023-06-25)
-        ------------------
-        
-        * added complete support for Mars and Moon IAU spatial reference systems
-        * version presented at the 6th Planetary Data Workshop in Flagstaff, Arizona
-        
-        0.1.1 (2023-06-23)
-        ------------------
-        
-        * added complete set of fields.
-        
-        0.1.0 (2023-06-21)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: pix2vec
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+===============
+pix2vec
+===============
+*Geospatial Vector Representation of Planetary Remote Sensing Hyperspectral Data*
+
+---------------------------------
+
+
+.. image:: https://img.shields.io/pypi/v/pix2vec.svg
+        :target: https://pypi.python.org/pypi/pix2vec
+
+.. image:: https://readthedocs.org/projects/pix2vec/badge/?version=latest
+        :target: https://pix2vec.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+pix2vec: Vector Representation of Planetary Hyperspectral Data Cubes
+
+
+* Free software: GNU General Public License v3
+* Documentation: https://pix2vec.readthedocs.io.
+
+
+Features
+--------
+
+* Produces a vector representation of the raster representation of HSI data 'cubes' generated by ISIS
+
+Requirements
+------------
+
+* a relatively recent `Integrated Software for Imagers and Spectrometers (ISIS) <https://isis.astrogeology.usgs.gov>`_ installation and the `kalasiris <https://github.com/rbeyer/kalasiris>`_ module (which will be installed automatically).
+ 
+Cite in your work
+-------------------
+
+Frigeri, A. and Hare, T. 2023. Geospatial Vector Representation of 
+Planetary Mapping Spectrometer Data. 6th Planetay Data Workshop, Flagstaff, Arizona 26-28th June 2023, Abstract #7088.::
+
+ @INPROCEEDINGS{FrigeriHare2023,
+       author = {{Frigeri}, A. and {Hare}, T.},
+        title = "{Geospatial Vector Representation of Planetary Mapping Spectrometer Data}",
+    booktitle = {6th Planetay Data Workshop},
+         year = 2023,
+       series = {LPI},
+        month = jun,
+          eid = {7088},
+        pages = {7088}
+ }
+
+
+installation
+------------
+
+within a working ISIS environment, run::
+
+    pip install pix2vect
+
+
+
+pix2vec in brief
+-----------------
+
+`pix2vect` requires spice-initialized ISIS cubes (see `spiceinit`).  
+
+Let's start with an hyperspectral cube from the The Moon Mineralogy Mapper (M3), the NASA spectrometer onboard  Chandrayaan-1 mission to the Moon::
+
+    (ISIS) $ pix2vec -i -c M3G20090103T084105_V03_L1B.cub 
+    pix2vect - 2023 Alessandro Frigeri - Istituto Nazionale di Astrofisica
+    Cube Type:M3 samples:304 lines:11739 file:M3G20090103T084105_V03_L1B.cub
+
+now we create a vector GIS file representing the geometry of the sensor's pixel on the lunar surface::
+
+    pix2vec -c M3G20090103T084105_V03_L1B.cub -s 1,150 -l 3050,3200 -o M3G20090103T084105_V03_L1B_subset.gpkg 
+
+the vector file can then be loaded in your favorite GIS, and we can plot the file with a `PixelValue` greyscale:
+
+.. image:: https://github.com/afrigeri/pix2vec/raw/main/docs/images/m3-PixelValue.png
+        :alt: M3-PixelValue
+        :width: 600
+
+each ground pixel element holds information that can be accessed:
+
+.. image:: https://github.com/afrigeri/pix2vec/raw/main/docs/images/m3-detail.png
+        :alt: M3-subcube
+        :width: 600
+
+for each ground-projected pixel, you now have access to these fields::
+
+	Filename Sample Line PixelValue RightAscension Declination 
+	PlanetocentricLatitude PlanetographicLatitude PositiveEast360Longitude 
+	PositiveEast180Longitude PositiveWest360Longitude PositiveWest180Longitude 
+	BodyFixedCoordinateX BodyFixedCoordinateY BodyFixedCoordinateZ LocalRadius 
+	SampleResolution LineResolution SpacecraftPositionX SpacecraftPositionY 
+	SpacecraftPositionZ SpacecraftAzimuth SlantDistance TargetCenterDistance 
+	SubSpacecraftLatitude SubSpacecraftLongitude SpacecraftAltitude OffNadirAngle 
+	SubSpacecraftGroundAzimuth SunPositionX SunPositionY SunPositionZ 
+	SubSolarAzimuth SolarDistance SubSolarLatitude SubSolarLongitude 
+	SubSolarGroundAzimuth Phase Incidence Emission NorthAzimuth EphemerisTime UTC 
+	LocalSolarTime SolarLongitude LookDirectionBodyFixedX LookDirectionBodyFixedY 
+	LookDirectionBodyFixedZ LookDirectionJ2000X LookDirectionJ2000Y 
+	LookDirectionJ2000Z LookDirectionCameraX LookDirectionCameraY 
+	LookDirectionCameraZ ObliqueDetectorResolution ObliquePixelResolution 
+	ObliqueLineResolution ObliqueSampleResolution Error
+
+
+Documentation
+-------------
+
+Documentation is available at https://pix2vec.readthedocs.io
+
+
+
+=======
+History
+=======
+
+0.1.3 (2023-07-08)
+------------------
+
+* fixed image link and typos in docs.
+
+0.1.2 (2023-06-25)
+------------------
+
+* added complete support for Mars and Moon IAU spatial reference systems
+* version presented at the 6th Planetary Data Workshop in Flagstaff, Arizona
+
+0.1.1 (2023-06-23)
+------------------
+
+* added complete set of fields.
+
+0.1.0 (2023-06-21)
+------------------
+
+* First release on PyPI.
```

### Comparing `pix2vec-0.1.2/pix2vec.egg-info/PKG-INFO` & `pix2vec-0.1.3/pix2vec.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,153 +1,160 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pix2vec
-Version: 0.1.2
-Summary: pix2vec produces a vector representation of planetary mapping spectrometers starting from hyperspectral an ISIS data cube
+Version: 0.1.3
+Summary: pix2vec produces a vector representation of planetary mapping spectrometers hyperspectral and camera ISIS data cube
 Home-page: https://github.com/afrigeri/pix2vec
 Author: Alessandro Frigeri
 Author-email: alessandro.frigeri@inaf.it
 License: GNU General Public License v3
-Description: ===============
-        pix2vec
-        ===============
-        *Geospatial Vector Representation of Planetary Remote Sensing Hyperspectral Data*
-        
-        ---------------------------------
-        
-        
-        .. image:: https://img.shields.io/pypi/v/pix2vec.svg
-                :target: https://pypi.python.org/pypi/pix2vec
-        
-        .. image:: https://readthedocs.org/projects/pix2vec/badge/?version=latest
-                :target: https://pix2vec.readthedocs.io/en/latest/?version=latest
-                :alt: Documentation Status
-        
-        pix2vec: Vector Representation of Planetary Hyperspectral Data Cubes
-        
-        
-        * Free software: GNU General Public License v3
-        * Documentation: https://pix2vec.readthedocs.io.
-        
-        
-        Features
-        --------
-        
-        * Produces a vector representation of the raster representation of HSI data 'cubes' generated by ISIS
-        
-        Requirements
-        ------------
-        
-        * a relatively recent `Integrated Software for Imagers and Spectrometers (ISIS) <https://isis.astrogeology.usgs.gov>`_ installation and the `kalasiris <https://github.com/rbeyer/kalasiris>`_ module (which will be installed automatically).
-         
-        Cite in your work
-        -------------------
-        
-        Frigeri, A. and Hare, T. 2023. Geospatial Vector Representation of 
-        Planetary Mapping Spectrometer Data. 6th Planetay Data Workshop, Flagstaff, Arizona 26-28th June 2023, Abstract #7088.::
-        
-         @INPROCEEDINGS{FrigeriHare2023,
-               author = {{Frigeri}, A. and {Hare}, T.},
-                title = "{Geospatial Vector Representation of Planetary Mapping Spectrometer Data}",
-            booktitle = {6th Planetay Data Workshop},
-                 year = 2023,
-               series = {LPI},
-                month = jun,
-                  eid = {7088},
-                pages = {7088}
-         }
-        
-        
-        installation
-        ------------
-        
-        within a working ISIS environment, run::
-        
-            pip install pix2vect
-        
-        
-        
-        pix2vec in brief
-        -----------------
-        
-        `pix2vect` requires spice-initialized ISIS cubes (see `spiceinit`).  
-        
-        Let's start with an hyperspectral cube from the The Moon Mineralogy Mapper (M3), the NASA spectrometer onboard  Chandrayaan-1 mission to the Moon::
-        
-            (ISIS) $ pix2vec -i -c M3G20090103T084105_V03_L1B.cub 
-            pix2vect - 2023 Alessandro Frigeri - Istituto Nazionale di Astrofisica
-            Cube Type:M3 samples:304 lines:11739 file:M3G20090103T084105_V03_L1B.cub
-        
-        now we create a vector GIS file representing the geometry of the sensor's pixel on the lunar surface::
-        
-            pix2vec -c M3G20090103T084105_V03_L1B.cub -s 1,150 -l 3050,3200 -o M3G20090103T084105_V03_L1B_subset.gpkg 
-        
-        the vector file can then be loaded in your favorite GIS, and we can plot the file with a `PixelValue` greyscale:
-        
-        .. image:: /docs/images/m3-PixelValue.png
-                :alt: M3-PixelValue
-                :width: 600
-        
-        each ground pixel element holds information that can be accessed:
-        
-        .. image:: /docs/images/m3-detail.png
-                :alt: M3-subcube
-                :width: 600
-        
-        for each ground-projected pixel, you now have access to these fields::
-        
-        	Filename Sample Line PixelValue RightAscension Declination 
-        	PlanetocentricLatitude PlanetographicLatitude PositiveEast360Longitude 
-        	PositiveEast180Longitude PositiveWest360Longitude PositiveWest180Longitude 
-        	BodyFixedCoordinateX BodyFixedCoordinateY BodyFixedCoordinateZ LocalRadius 
-        	SampleResolution LineResolution SpacecraftPositionX SpacecraftPositionY 
-        	SpacecraftPositionZ SpacecraftAzimuth SlantDistance TargetCenterDistance 
-        	SubSpacecraftLatitude SubSpacecraftLongitude SpacecraftAltitude OffNadirAngle 
-        	SubSpacecraftGroundAzimuth SunPositionX SunPositionY SunPositionZ 
-        	SubSolarAzimuth SolarDistance SubSolarLatitude SubSolarLongitude 
-        	SubSolarGroundAzimuth Phase Incidence Emission NorthAzimuth EphemerisTime UTC 
-        	LocalSolarTime SolarLongitude LookDirectionBodyFixedX LookDirectionBodyFixedY 
-        	LookDirectionBodyFixedZ LookDirectionJ2000X LookDirectionJ2000Y 
-        	LookDirectionJ2000Z LookDirectionCameraX LookDirectionCameraY 
-        	LookDirectionCameraZ ObliqueDetectorResolution ObliquePixelResolution 
-        	ObliqueLineResolution ObliqueSampleResolution Error
-        
-        
-        Documentation
-        -------------
-        
-        Documentation is available at https://pix2vec.readthedocs.io
-        
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.2 (2023-06-25)
-        ------------------
-        
-        * added complete support for Mars and Moon IAU spatial reference systems
-        * version presented at the 6th Planetary Data Workshop in Flagstaff, Arizona
-        
-        0.1.1 (2023-06-23)
-        ------------------
-        
-        * added complete set of fields.
-        
-        0.1.0 (2023-06-21)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: pix2vec
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+===============
+pix2vec
+===============
+*Geospatial Vector Representation of Planetary Remote Sensing Hyperspectral Data*
+
+---------------------------------
+
+
+.. image:: https://img.shields.io/pypi/v/pix2vec.svg
+        :target: https://pypi.python.org/pypi/pix2vec
+
+.. image:: https://readthedocs.org/projects/pix2vec/badge/?version=latest
+        :target: https://pix2vec.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+pix2vec: Vector Representation of Planetary Hyperspectral Data Cubes
+
+
+* Free software: GNU General Public License v3
+* Documentation: https://pix2vec.readthedocs.io.
+
+
+Features
+--------
+
+* Produces a vector representation of the raster representation of HSI data 'cubes' generated by ISIS
+
+Requirements
+------------
+
+* a relatively recent `Integrated Software for Imagers and Spectrometers (ISIS) <https://isis.astrogeology.usgs.gov>`_ installation and the `kalasiris <https://github.com/rbeyer/kalasiris>`_ module (which will be installed automatically).
+ 
+Cite in your work
+-------------------
+
+Frigeri, A. and Hare, T. 2023. Geospatial Vector Representation of 
+Planetary Mapping Spectrometer Data. 6th Planetay Data Workshop, Flagstaff, Arizona 26-28th June 2023, Abstract #7088.::
+
+ @INPROCEEDINGS{FrigeriHare2023,
+       author = {{Frigeri}, A. and {Hare}, T.},
+        title = "{Geospatial Vector Representation of Planetary Mapping Spectrometer Data}",
+    booktitle = {6th Planetay Data Workshop},
+         year = 2023,
+       series = {LPI},
+        month = jun,
+          eid = {7088},
+        pages = {7088}
+ }
+
+
+installation
+------------
+
+within a working ISIS environment, run::
+
+    pip install pix2vect
+
+
+
+pix2vec in brief
+-----------------
+
+`pix2vect` requires spice-initialized ISIS cubes (see `spiceinit`).  
+
+Let's start with an hyperspectral cube from the The Moon Mineralogy Mapper (M3), the NASA spectrometer onboard  Chandrayaan-1 mission to the Moon::
+
+    (ISIS) $ pix2vec -i -c M3G20090103T084105_V03_L1B.cub 
+    pix2vect - 2023 Alessandro Frigeri - Istituto Nazionale di Astrofisica
+    Cube Type:M3 samples:304 lines:11739 file:M3G20090103T084105_V03_L1B.cub
+
+now we create a vector GIS file representing the geometry of the sensor's pixel on the lunar surface::
+
+    pix2vec -c M3G20090103T084105_V03_L1B.cub -s 1,150 -l 3050,3200 -o M3G20090103T084105_V03_L1B_subset.gpkg 
+
+the vector file can then be loaded in your favorite GIS, and we can plot the file with a `PixelValue` greyscale:
+
+.. image:: https://github.com/afrigeri/pix2vec/raw/main/docs/images/m3-PixelValue.png
+        :alt: M3-PixelValue
+        :width: 600
+
+each ground pixel element holds information that can be accessed:
+
+.. image:: https://github.com/afrigeri/pix2vec/raw/main/docs/images/m3-detail.png
+        :alt: M3-subcube
+        :width: 600
+
+for each ground-projected pixel, you now have access to these fields::
+
+	Filename Sample Line PixelValue RightAscension Declination 
+	PlanetocentricLatitude PlanetographicLatitude PositiveEast360Longitude 
+	PositiveEast180Longitude PositiveWest360Longitude PositiveWest180Longitude 
+	BodyFixedCoordinateX BodyFixedCoordinateY BodyFixedCoordinateZ LocalRadius 
+	SampleResolution LineResolution SpacecraftPositionX SpacecraftPositionY 
+	SpacecraftPositionZ SpacecraftAzimuth SlantDistance TargetCenterDistance 
+	SubSpacecraftLatitude SubSpacecraftLongitude SpacecraftAltitude OffNadirAngle 
+	SubSpacecraftGroundAzimuth SunPositionX SunPositionY SunPositionZ 
+	SubSolarAzimuth SolarDistance SubSolarLatitude SubSolarLongitude 
+	SubSolarGroundAzimuth Phase Incidence Emission NorthAzimuth EphemerisTime UTC 
+	LocalSolarTime SolarLongitude LookDirectionBodyFixedX LookDirectionBodyFixedY 
+	LookDirectionBodyFixedZ LookDirectionJ2000X LookDirectionJ2000Y 
+	LookDirectionJ2000Z LookDirectionCameraX LookDirectionCameraY 
+	LookDirectionCameraZ ObliqueDetectorResolution ObliquePixelResolution 
+	ObliqueLineResolution ObliqueSampleResolution Error
+
+
+Documentation
+-------------
+
+Documentation is available at https://pix2vec.readthedocs.io
+
+
+
+=======
+History
+=======
+
+0.1.3 (2023-07-08)
+------------------
+
+* fixed image link and typos in docs.
+
+0.1.2 (2023-06-25)
+------------------
+
+* added complete support for Mars and Moon IAU spatial reference systems
+* version presented at the 6th Planetary Data Workshop in Flagstaff, Arizona
+
+0.1.1 (2023-06-23)
+------------------
+
+* added complete set of fields.
+
+0.1.0 (2023-06-21)
+------------------
+
+* First release on PyPI.
```

### Comparing `pix2vec-0.1.2/pix2vec.egg-info/SOURCES.txt` & `pix2vec-0.1.3/pix2vec.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+.gitignore
 .readthedocs.yaml
+.zenodo.json
 AUTHORS.rst
+CITATION.cff
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
+requirements.txt
 requirements_dev.txt
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/authors.rst
 docs/conf.py
```

### Comparing `pix2vec-0.1.2/LICENSE` & `pix2vec-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.2/CONTRIBUTING.rst` & `pix2vec-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.2/Makefile` & `pix2vec-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.2/docs/index.rst` & `pix2vec-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.2/docs/images/m3cube-c.png` & `pix2vec-0.1.3/docs/images/m3cube-c.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.2/docs/images/m3cube-a.png` & `pix2vec-0.1.3/docs/_build/html/_images/m3cube-a.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.2/docs/images/m3-detail.png` & `pix2vec-0.1.3/docs/images/m3-detail.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.2/docs/images/m3-PixelValue.png` & `pix2vec-0.1.3/docs/images/m3-PixelValue.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.2/docs/Makefile` & `pix2vec-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.2/docs/conf.py` & `pix2vec-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.2/docs/make.bat` & `pix2vec-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.2/docs/_build/html/_images/m3cube-a.png` & `pix2vec-0.1.3/docs/images/m3cube-a.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.2/docs/installation.rst` & `pix2vec-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.2/setup.py` & `pix2vec-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,26 +26,27 @@
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
-    description="pix2vec produces a vector representation of planetary mapping spectrometers starting from hyperspectral an ISIS data cube",
+    description="pix2vec produces a vector representation of planetary mapping spectrometers hyperspectral and camera ISIS data cube",
     entry_points={
         'console_scripts': [
             'pix2vec=pix2vec.cli:main',
         ],
     },
     install_requires=requirements,
     license="GNU General Public License v3",
     long_description=readme + '\n\n' + history,
+    long_description_content_type="text/x-rst",
     include_package_data=True,
     keywords='pix2vec',
     name='pix2vec',
     packages=find_packages(include=['pix2vec', 'pix2vec.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/afrigeri/pix2vec',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

### Comparing `pix2vec-0.1.2/pix2vec/cli.py` & `pix2vec-0.1.3/pix2vec/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,17 @@
     parser = argparse.ArgumentParser()
 	
     parser.add_argument('-c','--cube', required=True)
     parser.add_argument('-o','--output',help='geopackage GIS output file')
     parser.add_argument('-l', '--lines',help='the range of lines to be included in the output file\n \
 	                                          e.g. 1,10 to set line 1 to 10 (extreme included)')
     parser.add_argument('-s', '--samples',help='the range of samples to be included in the output file')
+    parser.add_argument('-i', '--info', action='store_true', dest='info',help='reports info about the \n\
+	                                 cube ')
     parser.add_argument('-d', '--debug')
-    parser.add_argument('-i', '--info', action='store_true', dest='info')
 	
     args = parser.parse_args()
 
     #print("Arguments: " + str(args._))
     print("pix2vect - 2023 Alessandro Frigeri - Istituto Nazionale di Astrofisica")
     #return 0
```

### Comparing `pix2vec-0.1.2/pix2vec/pix2vec.py` & `pix2vec-0.1.3/pix2vec/pix2vec.py`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.2/README.rst` & `pix2vec-0.1.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -70,21 +70,21 @@
 
 now we create a vector GIS file representing the geometry of the sensor's pixel on the lunar surface::
 
     pix2vec -c M3G20090103T084105_V03_L1B.cub -s 1,150 -l 3050,3200 -o M3G20090103T084105_V03_L1B_subset.gpkg 
 
 the vector file can then be loaded in your favorite GIS, and we can plot the file with a `PixelValue` greyscale:
 
-.. image:: /docs/images/m3-PixelValue.png
+.. image:: https://github.com/afrigeri/pix2vec/raw/main/docs/images/m3-PixelValue.png
         :alt: M3-PixelValue
         :width: 600
 
 each ground pixel element holds information that can be accessed:
 
-.. image:: /docs/images/m3-detail.png
+.. image:: https://github.com/afrigeri/pix2vec/raw/main/docs/images/m3-detail.png
         :alt: M3-subcube
         :width: 600
 
 for each ground-projected pixel, you now have access to these fields::
 
 	Filename Sample Line PixelValue RightAscension Declination 
 	PlanetocentricLatitude PlanetographicLatitude PositiveEast360Longitude
```

