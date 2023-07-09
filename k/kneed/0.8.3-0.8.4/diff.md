# Comparing `tmp/kneed-0.8.3.tar.gz` & `tmp/kneed-0.8.4.tar.gz`

## Comparing `kneed-0.8.3.tar` & `kneed-0.8.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kneed-0.8.3/kneed/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kneed-0.8.3/kneed/_version.py
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 kneed-0.8.3/kneed/data_generator.py
--rw-r--r--   0        0        0    17708 2020-02-02 00:00:00.000000 kneed-0.8.3/kneed/knee_locator.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 kneed-0.8.3/kneed/shape_detector.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 kneed-0.8.3/tests/test_no_matplotlib.py
--rw-r--r--   0        0        0    15504 2020-02-02 00:00:00.000000 kneed-0.8.3/tests/test_sample.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 kneed-0.8.3/.gitignore
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 kneed-0.8.3/LICENSE
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 kneed-0.8.3/README.md
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 kneed-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 kneed-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 kneed-0.8.4/kneed/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kneed-0.8.4/kneed/_version.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 kneed-0.8.4/kneed/data_generator.py
+-rw-r--r--   0        0        0    17826 2020-02-02 00:00:00.000000 kneed-0.8.4/kneed/knee_locator.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 kneed-0.8.4/kneed/shape_detector.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 kneed-0.8.4/tests/test_no_matplotlib.py
+-rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 kneed-0.8.4/tests/test_sample.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 kneed-0.8.4/.gitignore
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 kneed-0.8.4/LICENSE
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 kneed-0.8.4/README.md
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 kneed-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 kneed-0.8.4/PKG-INFO
```

### Comparing `kneed-0.8.3/kneed/data_generator.py` & `kneed-0.8.4/kneed/data_generator.py`

 * *Files identical despite different names*

### Comparing `kneed-0.8.3/kneed/knee_locator.py` & `kneed-0.8.4/kneed/knee_locator.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,142 +7,143 @@
 VALID_CURVE = ["convex", "concave"]
 VALID_DIRECTION = ["increasing", "decreasing"]
 
 try:
     import matplotlib.pyplot as plt
 except ImportError:
     _has_matplotlib = False
-    _matplotlib_not_found_err = ModuleNotFoundError("This function needs Matplotlib to be executed. Please run command `pip install kneed[plot]` ")
+    _matplotlib_not_found_err = ModuleNotFoundError(
+        "This function needs Matplotlib to be executed. Please run command `pip install kneed[plot]` "
+    )
 else:
     _has_matplotlib = True
 
+
 class KneeLocator(object):
     """
     Once instantiated, this class attempts to find the point of maximum
     curvature on a line. The knee is accessible via the `.knee` attribute.
 
     :param x: x values, must be the same length as y.
     :type x: 1D array of shape (`number_of_y_values`,) or list
     :param y: y values, must be the same length as x.
     :type y: 1D array of shape (`number_of_y_values`,) or list
-    :param S: Sensitivity, original paper suggests default of 1.0
+    :param S: Sensitivity, the number of minimum number of data points below the local distance maximum before calling a knee. The original paper suggests default of 1.0
     :type S: float
     :param curve: If 'concave', algorithm will detect knees. If 'convex', it
         will detect elbows.
     :type curve: str
     :param direction: one of {"increasing", "decreasing"}
     :type direction: str
     :param interp_method: one of {"interp1d", "polynomial"}
     :type interp_method: str
     :param online: kneed will correct old knee points if True, will return first knee if False
     :type online: bool
     :param polynomial_degree: The degree of the fitting polynomial. Only used when interp_method="polynomial". This argument is passed to numpy polyfit `deg` parameter.
     :type polynomial_degree: int
+    :ivar x: x values.
+    :vartype x: array-like
+    :ivar y: y values.
+    :vartype y: array-like
+    :ivar S: Sensitivity, original paper suggests default of 1.0
+    :vartype S: integer
+    :ivar curve: If 'concave', algorithm will detect knees. If 'convex', it
+        will detect elbows.
+    :vartype curve: str
+    :ivar direction: one of {"increasing", "decreasing"}
+    :vartype direction: str
+    :ivar interp_method: one of {"interp1d", "polynomial"}
+    :vartype interp_method: str
+    :ivar online: kneed will correct old knee points if True, will return first knee if False
+    :vartype online: str
+    :ivar polynomial_degree: The degree of the fitting polynomial. Only used when interp_method="polynomial". This argument is passed to numpy polyfit `deg` parameter.
+    :vartype polynomial_degree: int
+    :ivar N: The number of `x` values in the
+    :vartype N: integer
+    :ivar all_knees: A set containing all the x values of the identified knee points.
+    :vartype all_knees: set
+    :ivar all_norm_knees: A set containing all the normalized x values of the identified knee points.
+    :vartype all_norm_knees: set
+    :ivar all_knees_y: A list containing all the y values of the identified knee points.
+    :vartype all_knees_y: list
+    :ivar all_norm_knees_y: A list containing all the normalized y values of the identified knee points.
+    :vartype all_norm_knees_y: list
+    :ivar Ds_y: The y values from the fitted spline.
+    :vartype Ds_y: numpy array
+    :ivar x_normalized: The normalized x values.
+    :vartype x_normalized: numpy array
+    :ivar y_normalized: The normalized y values.
+    :vartype y_normalized: numpy array
+    :ivar x_difference: The x values of the difference curve.
+    :vartype x_difference: numpy array
+    :ivar y_difference: The y values of the difference curve.
+    :vartype y_difference: numpy array
+    :ivar maxima_indices: The indices of each of the maxima on the difference curve.
+    :vartype maxima_indices: numpy array
+    :ivar maxima_indices: The indices of each of the maxima on the difference curve.
+    :vartype maxima_indices: numpy array
+    :ivar x_difference_maxima: The x values from the difference curve where the local maxima are located.
+    :vartype x_difference_maxima: numpy array
+    :ivar y_difference_maxima: The y values from the difference curve where the local maxima are located.
+    :vartype y_difference_maxima: numpy array
+    :ivar minima_indices: The indices of each of the minima on the difference curve.
+    :vartype minima_indices: numpy array
+    :ivar minima_indices: The indices of each of the minima on the difference curve.
+    :vartype maxima_indices: numpy array
+    :ivar x_difference_minima: The x values from the difference curve where the local minima are located.
+    :vartype x_difference_minima: numpy array
+    :ivar y_difference_minima: The y values from the difference curve where the local minima are located.
+    :vartype y_difference_minima: numpy array
+    :ivar Tmx: The y values that correspond to the thresholds on the difference curve for determining the knee point.
+    :vartype Tmx: numpy array
+    :ivar knee: The x value of the knee point. None if no knee/elbow was detected.
+    :vartype knee: float
+    :ivar knee_y: The y value of the knee point. None if no knee/elbow was detected
+    :vartype knee_y: float
+    :ivar norm_knee: The normalized x value of the knee point. None if no knee/elbow was detected
+    :vartype norm_knee: float
+    :ivar norm_knee_y: The normalized y value of the knee point. None if no knee/elbow was detected
+    :vartype norm_knee_y: float
+    :ivar all_knees: The x values of all the identified knee points.
+    :vartype all_knees: set
+    :ivar all_knees_y: The y values of all the identified knee points.
+    :vartype all_knees: set
+    :ivar all_norm_knees: The normalized x values of all the identified knee points.
+    :vartype all_norm_knees: set
+    :ivar all_norm_knees_y: The normalized y values of all the identified knee points.
+    :vartype all_norm_knees: set
+    :ivar elbow: The x value of the elbow point (elbow and knee are interchangeable). None if no knee/elbow was detected
+    :vartype elbow: float
+    :ivar elbow_y: The y value of the knee point (elbow and knee are interchangeable). None if no knee/elbow was detected
+    :vartype elbow_y: float
+    :ivar norm_elbow: The normalized x value of the knee point (elbow and knee are interchangeable). None if no knee/elbow was detected
+    :vartype norm_knee: float
+    :ivar norm_elbow_y: The normalized y value of the knee point (elbow and knee are interchangeable). None if no knee/elbow was detected
+    :vartype norm_elbow_y: float
+    :ivar all_elbows: The x values of all the identified knee points (elbow and knee are interchangeable).
+    :vartype all_elbows: set
+    :ivar all_elbows_y: The y values of all the identified knee points (elbow and knee are interchangeable).
+    :vartype all_elbows: set
+    :ivar all_norm_elbows: The normalized x values of all the identified knee points (elbow and knee are interchangeable).
+    :vartype all_norm_elbows: set
+    :ivar all_norm_elbows_y: The normalized y values of all the identified knee points (elbow and knee are interchangeable).
+    :vartype all_norm_elbows: set
     """
 
     def __init__(
         self,
         x: Iterable[float],
         y: Iterable[float],
         S: float = 1.0,
         curve: str = "concave",
         direction: str = "increasing",
         interp_method: str = "interp1d",
         online: bool = False,
         polynomial_degree: int = 7,
     ):
-        """
-        :ivar x: x values.
-        :vartype x: array-like
-        :ivar y: y values.
-        :vartype y: array-like
-        :ivar S: Sensitivity, original paper suggests default of 1.0
-        :vartype S: integer
-        :ivar curve: If 'concave', algorithm will detect knees. If 'convex', it
-            will detect elbows.
-        :vartype curve: str
-        :ivar direction: one of {"increasing", "decreasing"}
-        :vartype direction: str
-        :ivar interp_method: one of {"interp1d", "polynomial"}
-        :vartype interp_method: str
-        :ivar online: kneed will correct old knee points if True, will return first knee if False
-        :vartype online: str
-        :ivar polynomial_degree: The degree of the fitting polynomial. Only used when interp_method="polynomial". This argument is passed to numpy polyfit `deg` parameter.
-        :vartype polynomial_degree: int
-        :ivar N: The number of `x` values in the
-        :vartype N: integer
-        :ivar all_knees: A set containing all the x values of the identified knee points.
-        :vartype all_knees: set
-        :ivar all_norm_knees: A set containing all the normalized x values of the identified knee points.
-        :vartype all_norm_knees: set
-        :ivar all_knees_y: A list containing all the y values of the identified knee points.
-        :vartype all_knees_y: list
-        :ivar all_norm_knees_y: A list containing all the normalized y values of the identified knee points.
-        :vartype all_norm_knees_y: list
-        :ivar Ds_y: The y values from the fitted spline.
-        :vartype Ds_y: numpy array
-        :ivar x_normalized: The normalized x values.
-        :vartype x_normalized: numpy array
-        :ivar y_normalized: The normalized y values.
-        :vartype y_normalized: numpy array
-        :ivar x_difference: The x values of the difference curve.
-        :vartype x_difference: numpy array
-        :ivar y_difference: The y values of the difference curve.
-        :vartype y_difference: numpy array
-        :ivar maxima_indices: The indices of each of the maxima on the difference curve.
-        :vartype maxima_indices: numpy array
-        :ivar maxima_indices: The indices of each of the maxima on the difference curve.
-        :vartype maxima_indices: numpy array
-        :ivar x_difference_maxima: The x values from the difference curve where the local maxima are located.
-        :vartype x_difference_maxima: numpy array
-        :ivar y_difference_maxima: The y values from the difference curve where the local maxima are located.
-        :vartype y_difference_maxima: numpy array
-        :ivar minima_indices: The indices of each of the minima on the difference curve.
-        :vartype minima_indices: numpy array
-        :ivar minima_indices: The indices of each of the minima on the difference curve.
-        :vartype maxima_indices: numpy array
-        :ivar x_difference_minima: The x values from the difference curve where the local minima are located.
-        :vartype x_difference_minima: numpy array
-        :ivar y_difference_minima: The y values from the difference curve where the local minima are located.
-        :vartype y_difference_minima: numpy array
-        :ivar Tmx: The y values that correspond to the thresholds on the difference curve for determining the knee point.
-        :vartype Tmx: numpy array
-        :ivar knee: The x value of the knee point.
-        :vartype knee: float
-        :ivar knee_y: The y value of the knee point.
-        :vartype knee_y: float
-        :ivar norm_knee: The normalized x value of the knee point.
-        :vartype norm_knee: float
-        :ivar norm_knee_y: The normalized y value of the knee point.
-        :vartype norm_knee_y: float
-        :ivar all_knees: The x values of all the identified knee points.
-        :vartype all_knees: set
-        :ivar all_knees_y: The y values of all the identified knee points.
-        :vartype all_knees: set
-        :ivar all_norm_knees: The normalized x values of all the identified knee points.
-        :vartype all_norm_knees: set
-        :ivar all_norm_knees_y: The normalized y values of all the identified knee points.
-        :vartype all_norm_knees: set
-        :ivar elbow: The x value of the elbow point (elbow and knee are interchangeable).
-        :vartype elbow: float
-        :ivar elbow_y: The y value of the knee point (elbow and knee are interchangeable).
-        :vartype elbow_y: float
-        :ivar norm_elbow: The normalized x value of the knee point (elbow and knee are interchangeable).
-        :vartype norm_knee: float
-        :ivar norm_elbow_y: The normalized y value of the knee point (elbow and knee are interchangeable).
-        :vartype norm_elbow_y: float
-        :ivar all_elbows: The x values of all the identified knee points (elbow and knee are interchangeable).
-        :vartype all_elbows: set
-        :ivar all_elbows_y: The y values of all the identified knee points (elbow and knee are interchangeable).
-        :vartype all_elbows: set
-        :ivar all_norm_elbows: The normalized x values of all the identified knee points (elbow and knee are interchangeable).
-        :vartype all_norm_elbows: set
-        :ivar all_norm_elbowss_y: The normalized y values of all the identified knee points (elbow and knee are interchangeable).
-        :vartype all_norm_elbows: set
-        """
         # Step 0: Raw Input
         self.x = np.array(x)
         self.y = np.array(y)
         self.curve = curve
         self.direction = direction
         self.N = len(self.x)
         self.S = S
@@ -234,15 +235,17 @@
             elif curve == "convex":
                 y = y.max() - y
         elif direction == "increasing" and curve == "convex":
             y = np.flip(y.max() - y)
 
         return y
 
-    def find_knee(self,):
+    def find_knee(
+        self,
+    ):
         """This function is called when KneeLocator is instantiated. It identifies the knee value and sets the instance attributes."""
         if not self.maxima_indices.size:
             warnings.warn(
                 "No local maxima found in the difference curve\n"
                 "The line is probably not polynomial, try plotting\n"
                 "the difference curve with plt.plot(knee.x_difference, knee.y_difference)\n"
                 "Also check that you aren't mistakenly setting the curve argument",
@@ -304,20 +307,26 @@
                 self.all_norm_knees.add(norm_knee)
 
                 # if detecting in offline mode, return the first knee found
                 if self.online is False:
                     return knee, norm_knee
 
         if self.all_knees == set():
-            warnings.warn("No knee/elbow found")
+            # No knee was found
             return None, None
 
         return knee, norm_knee
 
-    def plot_knee_normalized(self, figsize: Optional[Tuple[int, int]] = None, title: str = "Normalized Knee Point", xlabel: Optional[str] = None, ylabel: Optional[str] = None):
+    def plot_knee_normalized(
+        self,
+        figsize: Optional[Tuple[int, int]] = None,
+        title: str = "Normalized Knee Point",
+        xlabel: Optional[str] = None,
+        ylabel: Optional[str] = None,
+    ):
         """Plot the normalized curve, the difference curve (x_difference, y_normalized) and the knee, if it exists.
 
         :param figsize: Optional[Tuple[int, int]
             The figure size of the plot. Example (12, 8)
         :param title: str
             Title of the visualization, defaults to "Normalized Knee Point"
         :param xlabel: Optional[str]
@@ -352,15 +361,21 @@
             plt.ylim()[0],
             plt.ylim()[1],
             linestyles="--",
             label="knee/elbow",
         )
         plt.legend(loc="best")
 
-    def plot_knee(self, figsize: Optional[Tuple[int, int]] = None, title: str = "Knee Point", xlabel: Optional[str] = None, ylabel: Optional[str] = None):
+    def plot_knee(
+        self,
+        figsize: Optional[Tuple[int, int]] = None,
+        title: str = "Knee Point",
+        xlabel: Optional[str] = None,
+        ylabel: Optional[str] = None,
+    ):
         """
         Plot the curve and the knee, if it exists
 
         :param figsize: Optional[Tuple[int, int]
             The figure size of the plot. Example (12, 8)
         :param title: str
             Title of the visualization, defaults to "Knee Point"
```

### Comparing `kneed-0.8.3/kneed/shape_detector.py` & `kneed-0.8.4/kneed/shape_detector.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,13 +8,13 @@
     :return: direction("increasing" or "decreasing") and curve type("concave" or "convex")
     """
 
     p = np.polyfit(x, y, deg=1)
     x1, x2 = int(len(x) * 0.2), int(len(x) * 0.8)
     q = np.mean(y[x1:x2]) - np.mean(x[x1:x2] * p[0] + p[1])
     if p[0] > 0 and q > 0:
-        return 'increasing', 'concave'
+        return "increasing", "concave"
     if p[0] > 0 and q <= 0:
-        return 'increasing', 'convex'
+        return "increasing", "convex"
     if p[0] <= 0 and q > 0:
-        return 'decreasing', 'concave'
-    return 'decreasing', 'convex'
+        return "decreasing", "concave"
+    return "decreasing", "convex"
```

### Comparing `kneed-0.8.3/tests/test_no_matplotlib.py` & `kneed-0.8.4/tests/test_no_matplotlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,13 +6,14 @@
 def test_plot_knee_normalized():
     """Test that error is raised when matplotlib is not installed"""
     with pytest.raises(ModuleNotFoundError):
         x, y = dg.figure2()
         kl = KneeLocator(x, y, S=1.0, curve="concave", interp_method="interp1d")
         kl.plot_knee_normalized()
 
+
 def test_plot_knee():
     """Test that error is raised when matplotlib is not installed"""
     with pytest.raises(ModuleNotFoundError):
         x, y = dg.figure2()
         kl = KneeLocator(x, y, S=1.0, curve="concave", interp_method="interp1d")
         kl.plot_knee()
```

### Comparing `kneed-0.8.3/tests/test_sample.py` & `kneed-0.8.4/tests/test_sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -518,37 +518,44 @@
             94.0,
             95.0,
             96.0,
             97.0,
             98.0,
         ]
     )
-    kl = KneeLocator(x, y, curve="convex", direction="increasing", online=True,)
+    kl = KneeLocator(
+        x,
+        y,
+        curve="convex",
+        direction="increasing",
+        online=True,
+    )
     assert kl.knee == 73
 
+
 def test_valid_curve_direction():
     """Test that arguments to curve and direction are valid"""
     with pytest.raises(ValueError):
         kl = KneeLocator(range(3), [1, 3, 5], curve="bad curve")
 
     with pytest.raises(ValueError):
         kl = KneeLocator(range(3), [1, 3, 5], direction="bad direction")
 
 
 def test_find_shape():
     """Test that find_shape can detect the right shape of curve line"""
     x, y = dg.concave_increasing()
     direction, curve = find_shape(x, y)
-    assert direction == 'increasing'
-    assert curve == 'concave'
+    assert direction == "increasing"
+    assert curve == "concave"
     x, y = dg.concave_decreasing()
     direction, curve = find_shape(x, y)
-    assert direction == 'decreasing'
-    assert curve == 'concave'
+    assert direction == "decreasing"
+    assert curve == "concave"
     x, y = dg.convex_decreasing()
     direction, curve = find_shape(x, y)
-    assert direction == 'decreasing'
-    assert curve == 'convex'
+    assert direction == "decreasing"
+    assert curve == "convex"
     x, y = dg.convex_increasing()
     direction, curve = find_shape(x, y)
-    assert direction == 'increasing'
-    assert curve == 'convex'
+    assert direction == "increasing"
+    assert curve == "convex"
```

### Comparing `kneed-0.8.3/LICENSE` & `kneed-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kneed-0.8.3/README.md` & `kneed-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `kneed-0.8.3/pyproject.toml` & `kneed-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kneed-0.8.3/PKG-INFO` & `kneed-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kneed
-Version: 0.8.3
+Version: 0.8.4
 Summary: Knee-point detection in Python
 Project-URL: Homepage, https://github.com/arvkevi/kneed
 Project-URL: Documentation, https://kneed.readthedocs.io/en/latest/
 Author-email: Kevin Arvai <arvkevi@gmail.com>
 License-File: LICENSE
 Keywords: elbow-method,knee-detection,system
 Classifier: Development Status :: 3 - Alpha
```

