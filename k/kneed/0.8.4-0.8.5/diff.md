# Comparing `tmp/kneed-0.8.4.tar.gz` & `tmp/kneed-0.8.5.tar.gz`

## Comparing `kneed-0.8.4.tar` & `kneed-0.8.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kneed-0.8.4/kneed/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kneed-0.8.4/kneed/_version.py
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 kneed-0.8.4/kneed/data_generator.py
--rw-r--r--   0        0        0    17826 2020-02-02 00:00:00.000000 kneed-0.8.4/kneed/knee_locator.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 kneed-0.8.4/kneed/shape_detector.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 kneed-0.8.4/tests/test_no_matplotlib.py
--rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 kneed-0.8.4/tests/test_sample.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 kneed-0.8.4/.gitignore
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 kneed-0.8.4/LICENSE
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 kneed-0.8.4/README.md
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 kneed-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 kneed-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kneed-0.8.5/kneed/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kneed-0.8.5/kneed/_version.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 kneed-0.8.5/kneed/data_generator.py
+-rw-r--r--   0        0        0    17714 2020-02-02 00:00:00.000000 kneed-0.8.5/kneed/knee_locator.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 kneed-0.8.5/kneed/shape_detector.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 kneed-0.8.5/tests/test_no_matplotlib.py
+-rw-r--r--   0        0        0    15521 2020-02-02 00:00:00.000000 kneed-0.8.5/tests/test_sample.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 kneed-0.8.5/.gitignore
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 kneed-0.8.5/LICENSE
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 kneed-0.8.5/README.md
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 kneed-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 kneed-0.8.5/PKG-INFO
```

### Comparing `kneed-0.8.4/kneed/data_generator.py` & `kneed-0.8.5/kneed/data_generator.py`

 * *Files identical despite different names*

### Comparing `kneed-0.8.4/kneed/knee_locator.py` & `kneed-0.8.5/kneed/knee_locator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 from scipy import interpolate
 from scipy.signal import argrelextrema
-import warnings
 from typing import Tuple, Optional, Iterable
 
 VALID_CURVE = ["convex", "concave"]
 VALID_DIRECTION = ["increasing", "decreasing"]
 
 try:
     import matplotlib.pyplot as plt
@@ -240,21 +239,18 @@
         return y
 
     def find_knee(
         self,
     ):
         """This function is called when KneeLocator is instantiated. It identifies the knee value and sets the instance attributes."""
         if not self.maxima_indices.size:
-            warnings.warn(
-                "No local maxima found in the difference curve\n"
-                "The line is probably not polynomial, try plotting\n"
-                "the difference curve with plt.plot(knee.x_difference, knee.y_difference)\n"
-                "Also check that you aren't mistakenly setting the curve argument",
-                RuntimeWarning,
-            )
+            # No local maxima found in the difference curve
+            # The line is probably not polynomial, try plotting
+            # the difference curve with plt.plot(knee.x_difference, knee.y_difference)
+            # Also check that you aren't mistakenly setting the curve argument
             return None, None
         # placeholder for which threshold region i is located in.
         maxima_threshold_index = 0
         minima_threshold_index = 0
         traversed_maxima = False
         # traverse the difference curve
         for i, x in enumerate(self.x_difference):
```

### Comparing `kneed-0.8.4/kneed/shape_detector.py` & `kneed-0.8.5/kneed/shape_detector.py`

 * *Files identical despite different names*

### Comparing `kneed-0.8.4/tests/test_no_matplotlib.py` & `kneed-0.8.5/tests/test_no_matplotlib.py`

 * *Files identical despite different names*

### Comparing `kneed-0.8.4/tests/test_sample.py` & `kneed-0.8.5/tests/test_sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,19 +286,20 @@
     """Test that the interp_method argument is valid."""
     x, y = dg.figure2()
     with pytest.raises(ValueError):
         kl = KneeLocator(x, y, interp_method="not_a_method")
 
 
 def test_x_equals_y():
-    """Test that a runtime warning is raised when no maxima are found"""
+    """Test that knee is None when no maxima are found"""
     x = range(10)
     y = [1] * len(x)
-    with pytest.warns(RuntimeWarning):
-        kl = KneeLocator(x, y)
+    kl = KneeLocator(x, y)
+    assert kl.knee is None
+
 
 
 def test_plot_knee_normalized():
     """Test that plotting is functional"""
     x, y = dg.figure2()
     kl = KneeLocator(x, y, S=1.0, curve="concave", interp_method="interp1d")
     num_figures_before = plt.gcf().number
```

### Comparing `kneed-0.8.4/LICENSE` & `kneed-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kneed-0.8.4/README.md` & `kneed-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `kneed-0.8.4/pyproject.toml` & `kneed-0.8.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kneed-0.8.4/PKG-INFO` & `kneed-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kneed
-Version: 0.8.4
+Version: 0.8.5
 Summary: Knee-point detection in Python
 Project-URL: Homepage, https://github.com/arvkevi/kneed
 Project-URL: Documentation, https://kneed.readthedocs.io/en/latest/
 Author-email: Kevin Arvai <arvkevi@gmail.com>
 License-File: LICENSE
 Keywords: elbow-method,knee-detection,system
 Classifier: Development Status :: 3 - Alpha
```

