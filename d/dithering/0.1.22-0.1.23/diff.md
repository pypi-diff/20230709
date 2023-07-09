# Comparing `tmp/dithering-0.1.22.tar.gz` & `tmp/dithering-0.1.23.tar.gz`

## Comparing `dithering-0.1.22.tar` & `dithering-0.1.23.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 dithering-0.1.22/Cargo.toml
--rw-r--r--   0     1001      123     2805 2023-07-08 21:04:45.000000 dithering-0.1.22/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-07-08 21:04:45.000000 dithering-0.1.22/.gitignore
--rw-r--r--   0     1001      123     1067 2023-07-08 21:04:45.000000 dithering-0.1.22/LICENSE
--rw-r--r--   0     1001      123      758 2023-07-08 21:04:45.000000 dithering-0.1.22/README.md
--rw-r--r--   0     1001      123      103 2023-07-08 21:04:45.000000 dithering-0.1.22/dithering.pyi
--rw-r--r--   0     1001      123      369 2023-07-08 21:04:45.000000 dithering-0.1.22/pyproject.toml
--rw-r--r--   0     1001      123    57161 2023-07-08 21:04:45.000000 dithering-0.1.22/resources/BackyardML_logo.svg
--rw-r--r--   0     1001      123     8863 2023-07-08 21:04:45.000000 dithering-0.1.22/resources/dithering.png
--rw-r--r--   0     1001      123    57228 2023-07-08 21:04:45.000000 dithering-0.1.22/resources/dithering.svg
--rw-r--r--   0     1001      123      212 2023-07-08 21:04:45.000000 dithering-0.1.22/src/lib.rs
--rw-r--r--   0     1001      123       51 2023-07-08 21:04:45.000000 dithering-0.1.22/src/methods/mod.rs
--rw-r--r--   0     1001      123     1583 2023-07-08 21:04:45.000000 dithering-0.1.22/src/methods/ordered.rs
--rw-r--r--   0     1001      123     9356 2023-07-08 21:04:45.000000 dithering-0.1.22/Cargo.lock
--rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 dithering-0.1.22/PKG-INFO
+-rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 dithering-0.1.23/Cargo.toml
+-rw-r--r--   0     1001      123     2805 2023-07-09 20:18:15.000000 dithering-0.1.23/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-07-09 20:18:15.000000 dithering-0.1.23/.gitignore
+-rw-r--r--   0     1001      123     1067 2023-07-09 20:18:15.000000 dithering-0.1.23/LICENSE
+-rw-r--r--   0     1001      123      758 2023-07-09 20:18:15.000000 dithering-0.1.23/README.md
+-rw-r--r--   0     1001      123      103 2023-07-09 20:18:15.000000 dithering-0.1.23/dithering.pyi
+-rw-r--r--   0     1001      123      369 2023-07-09 20:18:15.000000 dithering-0.1.23/pyproject.toml
+-rw-r--r--   0     1001      123    57161 2023-07-09 20:18:15.000000 dithering-0.1.23/resources/BackyardML_logo.svg
+-rw-r--r--   0     1001      123     8863 2023-07-09 20:18:15.000000 dithering-0.1.23/resources/dithering.png
+-rw-r--r--   0     1001      123    57228 2023-07-09 20:18:15.000000 dithering-0.1.23/resources/dithering.svg
+-rw-r--r--   0     1001      123      212 2023-07-09 20:18:15.000000 dithering-0.1.23/src/lib.rs
+-rw-r--r--   0     1001      123       51 2023-07-09 20:18:15.000000 dithering-0.1.23/src/methods/mod.rs
+-rw-r--r--   0     1001      123     1662 2023-07-09 20:18:15.000000 dithering-0.1.23/src/methods/ordered.rs
+-rw-r--r--   0     1001      123     9356 2023-07-09 20:18:15.000000 dithering-0.1.23/Cargo.lock
+-rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 dithering-0.1.23/PKG-INFO
```

### Comparing `dithering-0.1.22/.github/workflows/CI.yml` & `dithering-0.1.23/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dithering-0.1.22/.gitignore` & `dithering-0.1.23/.gitignore`

 * *Files identical despite different names*

### Comparing `dithering-0.1.22/LICENSE` & `dithering-0.1.23/LICENSE`

 * *Files identical despite different names*

### Comparing `dithering-0.1.22/README.md` & `dithering-0.1.23/README.md`

 * *Files identical despite different names*

### Comparing `dithering-0.1.22/resources/BackyardML_logo.svg` & `dithering-0.1.23/resources/BackyardML_logo.svg`

 * *Files identical despite different names*

### Comparing `dithering-0.1.22/resources/dithering.png` & `dithering-0.1.23/resources/dithering.png`

 * *Files identical despite different names*

### Comparing `dithering-0.1.22/resources/dithering.svg` & `dithering-0.1.23/resources/dithering.svg`

 * *Files identical despite different names*

### Comparing `dithering-0.1.22/src/methods/ordered.rs` & `dithering-0.1.23/src/methods/ordered.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 use pyo3::prelude::*;
+use numpy::PyArray2;
 
 #[pyfunction]
 pub fn ordered_dither<'py>(
-    _py: Python<'py>,
+    py: Python<'py>,
     image: Vec<Vec<u8>>,
     matrix: Vec<Vec<u8>>,
-) -> Vec<Vec<u8>> {
+) -> PyResult<&'py PyArray2<u8>> {
 
     let img_height = image.len();
     let img_width = image[0].len();
 
     let dither_height = matrix.len();
     let dither_width = matrix[0].len();
 
     let mut result: Vec<Vec<u8>> = Vec::with_capacity(img_height);
 
     (0..img_height).for_each(|y| {
         let mut row: Vec<u8> = Vec::with_capacity(img_width);
         (0..img_width).for_each(|x| {
-            let old_pixel = image[y][x]; // Fix the order of indices
-            let d_val = matrix[y % dither_height][x % dither_width]; // Fix the order of indices
+            let old_pixel = image[y][x];
+            let d_val = matrix[y % dither_height][x % dither_width];
             row.push(if old_pixel < d_val { 0 } else { 255 });
         });
         result.push(row);
     });
+    let d = PyArray2::from_vec2(py, &result).unwrap();
 
-    result
+    Ok(d)
 }
 
 #[cfg(test)]
 mod tests {
+
+    use numpy::array;
+
     use super::*;
 
     #[test]
     fn test_ordered_dither() {
         pyo3::prepare_freethreaded_python();
         Python::with_gil(|py| {
         // Test input data
@@ -44,22 +49,22 @@
         ];
         let matrix = vec![
             vec![100, 50],
             vec![75, 125],
         ];
 
         // Expected output
-        let expected_result = vec![
-            vec![255, 255, 255],
-            vec![0, 0, 255],
-            vec![255, 255, 0],
+        let expected_result = array![
+            [255, 255, 255],
+            [0, 0, 255],
+            [255, 255, 0],
         ];
 
         // Call the function
-        let result = ordered_dither(py, image, matrix);
+        let result = ordered_dither(py, image, matrix).unwrap();
         
         // Assert the result
-        assert_eq!(result, expected_result);
+        assert_eq!(&result.readonly().as_array(), expected_result);
         });
         
     }
 }
```

### Comparing `dithering-0.1.22/Cargo.lock` & `dithering-0.1.23/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "dithering"
-version = "0.1.22"
+version = "0.1.23"
 dependencies = [
  "numpy",
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
```

### Comparing `dithering-0.1.22/PKG-INFO` & `dithering-0.1.23/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dithering
-Version: 0.1.22
+Version: 0.1.23
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Efficient implementations of various image dithering methods.
 Home-Page: https://backyardml.github.io/
 Author: Patrik Larsson <patrik@backyardml.se>
```

