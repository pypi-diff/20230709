# Comparing `tmp/sen2nbar-2023.3.0.tar.gz` & `tmp/sen2nbar-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sen2nbar-2023.3.0.tar", last modified: Tue Mar 21 09:09:14 2023, max compression
+gzip compressed data, was "dist/sen2nbar-2023.7.0.tar", last modified: Sun Jul  9 18:24:22 2023, max compression
```

## Comparing `sen2nbar-2023.3.0.tar` & `sen2nbar-2023.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-03-21 09:09:14.601156 sen2nbar-2023.3.0/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2023-03-21 08:42:48.000000 sen2nbar-2023.3.0/LICENSE
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-03-21 09:09:14.601156 sen2nbar-2023.3.0/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7217 2023-03-21 08:42:48.000000 sen2nbar-2023.3.0/README.md
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-03-21 09:09:14.601156 sen2nbar-2023.3.0/sen2nbar/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      194 2023-03-21 08:42:48.000000 sen2nbar-2023.3.0/sen2nbar/__init__.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      604 2023-03-21 08:42:48.000000 sen2nbar-2023.3.0/sen2nbar/axioms.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1679 2023-03-21 08:42:48.000000 sen2nbar-2023.3.0/sen2nbar/brdf.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2936 2023-03-21 08:42:48.000000 sen2nbar-2023.3.0/sen2nbar/c_factor.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     3695 2023-03-21 08:42:48.000000 sen2nbar-2023.3.0/sen2nbar/kernels.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     4340 2023-03-21 08:42:48.000000 sen2nbar-2023.3.0/sen2nbar/metadata.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7139 2023-03-21 08:42:48.000000 sen2nbar-2023.3.0/sen2nbar/nbar.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1558 2023-03-21 08:42:48.000000 sen2nbar-2023.3.0/sen2nbar/utils.py
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-03-21 09:09:14.601156 sen2nbar-2023.3.0/sen2nbar.egg-info/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-03-21 09:09:14.000000 sen2nbar-2023.3.0/sen2nbar.egg-info/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      339 2023-03-21 09:09:14.000000 sen2nbar-2023.3.0/sen2nbar.egg-info/SOURCES.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-03-21 09:09:14.000000 sen2nbar-2023.3.0/sen2nbar.egg-info/dependency_links.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      187 2023-03-21 09:09:14.000000 sen2nbar-2023.3.0/sen2nbar.egg-info/requires.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        9 2023-03-21 09:09:14.000000 sen2nbar-2023.3.0/sen2nbar.egg-info/top_level.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-03-21 09:09:14.601156 sen2nbar-2023.3.0/setup.cfg
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1404 2023-03-21 08:42:48.000000 sen2nbar-2023.3.0/setup.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-09 18:24:22.793621 sen2nbar-2023.7.0/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2023-07-09 13:18:33.000000 sen2nbar-2023.7.0/LICENSE
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-07-09 18:24:22.793621 sen2nbar-2023.7.0/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7217 2023-07-09 13:18:33.000000 sen2nbar-2023.7.0/README.md
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-09 18:24:22.790287 sen2nbar-2023.7.0/sen2nbar/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      194 2023-07-09 18:13:00.000000 sen2nbar-2023.7.0/sen2nbar/__init__.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      604 2023-07-09 13:18:34.000000 sen2nbar-2023.7.0/sen2nbar/axioms.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1679 2023-07-09 13:18:34.000000 sen2nbar-2023.7.0/sen2nbar/brdf.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2936 2023-07-09 13:18:34.000000 sen2nbar-2023.7.0/sen2nbar/c_factor.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     3695 2023-07-09 13:18:34.000000 sen2nbar-2023.7.0/sen2nbar/kernels.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     4340 2023-07-09 13:18:34.000000 sen2nbar-2023.7.0/sen2nbar/metadata.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7479 2023-07-09 18:12:35.000000 sen2nbar-2023.7.0/sen2nbar/nbar.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1558 2023-07-09 13:18:34.000000 sen2nbar-2023.7.0/sen2nbar/utils.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-09 18:24:22.793621 sen2nbar-2023.7.0/sen2nbar.egg-info/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-07-09 18:24:22.000000 sen2nbar-2023.7.0/sen2nbar.egg-info/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      339 2023-07-09 18:24:22.000000 sen2nbar-2023.7.0/sen2nbar.egg-info/SOURCES.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-07-09 18:24:22.000000 sen2nbar-2023.7.0/sen2nbar.egg-info/dependency_links.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)       94 2023-07-09 18:24:22.000000 sen2nbar-2023.7.0/sen2nbar.egg-info/requires.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        9 2023-07-09 18:24:22.000000 sen2nbar-2023.7.0/sen2nbar.egg-info/top_level.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-07-09 18:24:22.793621 sen2nbar-2023.7.0/setup.cfg
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1234 2023-07-09 18:12:52.000000 sen2nbar-2023.7.0/setup.py
```

### Comparing `sen2nbar-2023.3.0/LICENSE` & `sen2nbar-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.3.0/PKG-INFO` & `sen2nbar-2023.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sen2nbar
-Version: 2023.3.0
+Version: 2023.7.0
 Summary: Nadir BRDF Adjusted Reflectance (NBAR) for Sentinel-2 in Python
 Home-page: https://github.com/ESDS-Leipzig/sen2nbar
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sen2nbar Version: 2023.3.0 Summary: Nadir BRDF
+Metadata-Version: 2.1 Name: sen2nbar Version: 2023.7.0 Summary: Nadir BRDF
 Adjusted Reflectance (NBAR) for Sentinel-2 in Python Home-page: https://
 github.com/ESDS-Leipzig/sen2nbar Author: David Montero Loaiza Author-email:
 dml.mont@gmail.com License: MIT Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
                                     [cubo]
```

### Comparing `sen2nbar-2023.3.0/README.md` & `sen2nbar-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.3.0/sen2nbar/axioms.py` & `sen2nbar-2023.7.0/sen2nbar/axioms.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.3.0/sen2nbar/brdf.py` & `sen2nbar-2023.7.0/sen2nbar/brdf.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.3.0/sen2nbar/c_factor.py` & `sen2nbar-2023.7.0/sen2nbar/c_factor.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.3.0/sen2nbar/kernels.py` & `sen2nbar-2023.7.0/sen2nbar/kernels.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.3.0/sen2nbar/metadata.py` & `sen2nbar-2023.7.0/sen2nbar/metadata.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.3.0/sen2nbar/nbar.py` & `sen2nbar-2023.7.0/sen2nbar/nbar.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,52 +10,56 @@
 
 from .axioms import bands
 from .c_factor import c_factor_from_item, c_factor_from_metadata
 from .metadata import get_processing_baseline
 from .utils import _extrapolate_c_factor
 
 
-def nbar_SAFE(path: str, cog: bool = True, quiet: bool = False) -> None:
+def nbar_SAFE(
+    path: str, cog: bool = True, to_int: bool = False, quiet: bool = False
+) -> None:
     """Computes the Nadir BRDF Adjusted Reflectance (NBAR) using the SAFE path.
 
     If the processing baseline is greater than 04.00, the DN values are automatically
     shifted before computing NBAR. All images are saved in the SAFE path inside the folder
     NBAR.
 
     Parameters
     ----------
     path : str
         SAFE path.
     cog : bool, default = True
         Whether to save the images as Cloud Optimized GeoTIFF (COG).
+    to_int : bool, default = False
+        Whether to convert the NBAR output to integer.
     quiet : bool, default = False
         Whether to show progress.
 
     Returns
     -------
     None
     """
     # Whether to save as COG
     if cog:
         driver = "COG"
     else:
         driver = None
 
     # NBAR folder to store the images
-    nbar_output_path = f"{path}/NBAR/"
+    nbar_output_path = os.path.join(path, "NBAR")
 
     # Create folder inside the SAFE path
     if not os.path.exists(nbar_output_path):
         os.makedirs(nbar_output_path)
 
     # Metadata file
-    metadata = glob(f"{path}/GRANULE/*/MTD_TL.xml")[0]
+    metadata = glob(os.path.join(path, "GRANULE", "*", "MTD_TL.xml"))[0]
 
     # Processing baseline
-    PROCESSING_BASELINE = get_processing_baseline(f"{path}/MTD_MSIL2A.xml")
+    PROCESSING_BASELINE = get_processing_baseline(os.path.join(path, "MTD_MSIL2A.xml"))
 
     # Whether to shift the DN values
     # After 04.00 all DN values are shifted by 1000
     harmonize = PROCESSING_BASELINE >= 4.0
 
     # Compute c-factor
     c = c_factor_from_metadata(metadata)
@@ -67,18 +71,22 @@
     pbar = tqdm(bands.items(), disable=quiet)
 
     # Compute NBAR per band
     for band, resolution in pbar:
         pbar.set_description(f"Processing {band}")
 
         # Image file
-        img_path = glob(f"{path}/GRANULE/*/IMG_DATA/*/*_{band}_{resolution}m.jp2")[0]
+        img_path = glob(
+            os.path.join(
+                path, "GRANULE", "*", "IMG_DATA", "*", f"*_{band}_{resolution}m.jp2"
+            )
+        )[0]
 
         # Rename filename to tif extension
-        filename = img_path.split("/")[-1].replace("jp2", "tif")
+        filename = os.path.split(img_path)[1].replace("jp2", "tif")
 
         # Open image and convert zeros to nan
         img = rioxarray.open_rasterio(img_path)
         img = img.where(lambda x: x > 0, other=np.nan)
 
         # Harmonize
         if harmonize:
@@ -88,16 +96,19 @@
         interpolated = c.sel(band=band).interp(
             y=img.y, x=img.x, method="linear", kwargs={"fill_value": "extrapolate"}
         )
 
         # Compute the NBAR
         img = img * interpolated
 
+        if to_int:
+            img = img.round().astype("int16")
+
         # Save the image
-        img.rio.to_raster(f"{nbar_output_path}{filename}", driver=driver)
+        img.rio.to_raster(os.path.join(nbar_output_path, filename), driver=driver)
 
     pbar.set_description(f"Done")
 
     # Show the path where the images were saved
     if not quiet:
         print(f"Saved to {nbar_output_path}")
 
@@ -245,12 +256,13 @@
     xarray.DataArray
         NBAR data array.
     """
     # Get info from the cubo data array
     stac = da.attrs["stac"]
     collection = da.attrs["collection"]
     epsg = da.attrs["epsg"]
+    epsg = f"epsg:{epsg}"
 
     # Compute NBAR
     da = nbar_stac(da, stac, collection, epsg, quiet)
 
     return da
```

### Comparing `sen2nbar-2023.3.0/sen2nbar/utils.py` & `sen2nbar-2023.7.0/sen2nbar/utils.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.3.0/sen2nbar.egg-info/PKG-INFO` & `sen2nbar-2023.7.0/sen2nbar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sen2nbar
-Version: 2023.3.0
+Version: 2023.7.0
 Summary: Nadir BRDF Adjusted Reflectance (NBAR) for Sentinel-2 in Python
 Home-page: https://github.com/ESDS-Leipzig/sen2nbar
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sen2nbar Version: 2023.3.0 Summary: Nadir BRDF
+Metadata-Version: 2.1 Name: sen2nbar Version: 2023.7.0 Summary: Nadir BRDF
 Adjusted Reflectance (NBAR) for Sentinel-2 in Python Home-page: https://
 github.com/ESDS-Leipzig/sen2nbar Author: David Montero Loaiza Author-email:
 dml.mont@gmail.com License: MIT Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
                                     [cubo]
```

### Comparing `sen2nbar-2023.3.0/setup.py` & `sen2nbar-2023.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,39 +10,32 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
     name="sen2nbar",
-    version="2023.3.0",
+    version="2023.7.0",
     url="https://github.com/ESDS-Leipzig/sen2nbar",
     license="MIT",
     author="David Montero Loaiza",
     author_email="dml.mont@gmail.com",
     description="Nadir BRDF Adjusted Reflectance (NBAR) for Sentinel-2 in Python",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=("tests",)),
     package_data={"sen2nbar": ["data/*.json"]},
     install_requires=[
-        "cubo",
-        "dask>=2022.02.0",
-        "numpy",
-        "pandas",
-        "planetary_computer>=0.4.9",
+        "cubo>=2023.7.0",
         "pystac",
-        "pystac_client",
         "rasterio>=1.3.6",
         "requests",
         "rioxarray>=0.13.4",
         "scipy>=1.10.1",
-        "stackstac>=0.4.3",
         "tqdm",
-        "xarray>=2023.2.0",
         "xmltodict",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.9",
```

