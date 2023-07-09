# Comparing `tmp/image_func-1.0.8.tar.gz` & `tmp/image_func-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_func-1.0.8.tar", last modified: Sun Jul  9 11:29:50 2023, max compression
+gzip compressed data, was "image_func-1.0.9.tar", last modified: Sun Jul  9 11:52:34 2023, max compression
```

## Comparing `image_func-1.0.8.tar` & `image_func-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 11:29:50.532254 image_func-1.0.8/
--rw-rw-rw-   0        0        0     1477 2023-07-08 13:23:55.000000 image_func-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      577 2023-07-09 11:29:50.528266 image_func-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-09 11:29:50.505814 image_func-1.0.8/image_func/
--rw-rw-rw-   0        0        0     1653 2023-07-09 11:27:13.000000 image_func-1.0.8/image_func/__init__.py
--rw-rw-rw-   0        0        0     1653 2023-07-09 11:24:06.000000 image_func-1.0.8/image_func/a.py
-drwxrwxrwx   0        0        0        0 2023-07-09 11:29:50.526270 image_func-1.0.8/image_func.egg-info/
--rw-rw-rw-   0        0        0      577 2023-07-09 11:29:50.000000 image_func-1.0.8/image_func.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-07-09 11:29:50.000000 image_func-1.0.8/image_func.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 11:29:50.000000 image_func-1.0.8/image_func.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-07-09 11:29:50.000000 image_func-1.0.8/image_func.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-09 11:29:50.000000 image_func-1.0.8/image_func.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 11:29:50.532254 image_func-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      793 2023-07-09 11:29:45.000000 image_func-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 11:52:34.783587 image_func-1.0.9/
+-rw-rw-rw-   0        0        0     1477 2023-07-08 13:23:55.000000 image_func-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      577 2023-07-09 11:52:34.782588 image_func-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-09 11:52:34.766631 image_func-1.0.9/image_func/
+-rw-rw-rw-   0        0        0     2046 2023-07-09 11:52:11.000000 image_func-1.0.9/image_func/__init__.py
+-rw-rw-rw-   0        0        0     2048 2023-07-09 11:52:13.000000 image_func-1.0.9/image_func/a.py
+drwxrwxrwx   0        0        0        0 2023-07-09 11:52:34.780593 image_func-1.0.9/image_func.egg-info/
+-rw-rw-rw-   0        0        0      577 2023-07-09 11:52:34.000000 image_func-1.0.9/image_func.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-07-09 11:52:34.000000 image_func-1.0.9/image_func.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 11:52:34.000000 image_func-1.0.9/image_func.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-09 11:52:34.000000 image_func-1.0.9/image_func.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-09 11:52:34.000000 image_func-1.0.9/image_func.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 11:52:34.783587 image_func-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      793 2023-07-09 11:52:30.000000 image_func-1.0.9/setup.py
```

### Comparing `image_func-1.0.8/LICENSE.txt` & `image_func-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `image_func-1.0.8/PKG-INFO` & `image_func-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_func
-Version: 1.0.8
+Version: 1.0.9
 Summary: A module for image processing
 Author: Armankhanvsit
 Author-email: armanpconly@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `image_func-1.0.8/image_func/__init__.py` & `image_func-1.0.9/image_func/a.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,8 +40,22 @@
 
     # Calculate magnitude spectrum
     magnitude_spectrum = 20 * np.log(cv2.magnitude(dft_shift[:, :, 0], dft_shift[:, :, 1]) + 1)
 
     # Reconstruct the image using inverse Fourier transform
     result = cv2.magnitude(cv2.idft(np.fft.ifftshift(dft_shift))[:, :, 0], cv2.idft(np.fft.ifftshift(dft_shift))[:, :, 1])
 
-    return optimalImg, magnitude_spectrum, result
+    return optimalImg, magnitude_spectrum, result
+
+
+def apply_log_transform(image_path, output_path):
+    # Read the image
+    img = cv2.imread(image_path)
+
+    # Apply log transform
+    log_transformed = 255 * np.log(1 + img.astype(np.float32)) / np.log(1 + np.max(img))
+
+    # Convert the data type
+    log_transformed = log_transformed.astype(np.uint8)
+
+    # Save the output image
+    cv2.imwrite(output_path, log_transformed)
```

### Comparing `image_func-1.0.8/image_func/a.py` & `image_func-1.0.9/image_func/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,8 +40,21 @@
 
     # Calculate magnitude spectrum
     magnitude_spectrum = 20 * np.log(cv2.magnitude(dft_shift[:, :, 0], dft_shift[:, :, 1]) + 1)
 
     # Reconstruct the image using inverse Fourier transform
     result = cv2.magnitude(cv2.idft(np.fft.ifftshift(dft_shift))[:, :, 0], cv2.idft(np.fft.ifftshift(dft_shift))[:, :, 1])
 
-    return optimalImg, magnitude_spectrum, result
+    return optimalImg, magnitude_spectrum, result
+
+def apply_log_transform(image_path, output_path):
+    # Read the image
+    img = cv2.imread(image_path)
+
+    # Apply log transform
+    log_transformed = 255 * np.log(1 + img.astype(np.float32)) / np.log(1 + np.max(img))
+
+    # Convert the data type
+    log_transformed = log_transformed.astype(np.uint8)
+
+    # Save the output image
+    cv2.imwrite(output_path, log_transformed)
```

### Comparing `image_func-1.0.8/image_func.egg-info/PKG-INFO` & `image_func-1.0.9/image_func.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-func
-Version: 1.0.8
+Version: 1.0.9
 Summary: A module for image processing
 Author: Armankhanvsit
 Author-email: armanpconly@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `image_func-1.0.8/setup.py` & `image_func-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='image_func',
-    version='1.0.8',
+    version='1.0.9',
     author='Armankhanvsit',
     author_email='armanpconly@gmail.com',
     description='A module for image processing',
     long_description='A module for image processing using numpy, PIL, scipy, and matplotlib.',
     packages=['image_func'],
     install_requires=[
         'numpy',
```

