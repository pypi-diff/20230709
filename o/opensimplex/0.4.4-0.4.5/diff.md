# Comparing `tmp/opensimplex-0.4.4.tar.gz` & `tmp/opensimplex-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensimplex-0.4.4.tar", last modified: Tue Jan  3 19:38:38 2023, max compression
+gzip compressed data, was "opensimplex-0.4.5.tar", last modified: Sun Jul  9 13:37:15 2023, max compression
```

## Comparing `opensimplex-0.4.4.tar` & `opensimplex-0.4.5.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2023-01-03 19:38:38.393266 opensimplex-0.4.4/
--rw-r--r--   0 lmas      (1001) lmas      (1001)     1074 2022-06-08 13:33:35.000000 opensimplex-0.4.4/LICENSE
--rw-r--r--   0 lmas      (1001) lmas      (1001)    10558 2023-01-03 19:38:38.393065 opensimplex-0.4.4/PKG-INFO
--rw-r--r--   0 lmas      (1001) lmas      (1001)     9906 2022-10-29 15:47:50.000000 opensimplex-0.4.4/README.md
-drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2023-01-03 19:38:38.391420 opensimplex-0.4.4/opensimplex/
--rw-r--r--   0 lmas      (1001) lmas      (1001)       62 2023-01-03 19:21:52.000000 opensimplex-0.4.4/opensimplex/__init__.py
--rw-r--r--   0 lmas      (1001) lmas      (1001)     5615 2022-08-05 16:56:16.000000 opensimplex-0.4.4/opensimplex/api.py
--rw-r--r--   0 lmas      (1001) lmas      (1001)     2651 2022-08-05 16:56:16.000000 opensimplex-0.4.4/opensimplex/constants.py
--rw-r--r--   0 lmas      (1001) lmas      (1001)    71171 2022-08-05 16:56:16.000000 opensimplex-0.4.4/opensimplex/internals.py
-drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2023-01-03 19:38:38.392292 opensimplex-0.4.4/opensimplex.egg-info/
--rw-r--r--   0 lmas      (1001) lmas      (1001)    10558 2023-01-03 19:38:37.000000 opensimplex-0.4.4/opensimplex.egg-info/PKG-INFO
--rw-r--r--   0 lmas      (1001) lmas      (1001)      402 2023-01-03 19:38:38.000000 opensimplex-0.4.4/opensimplex.egg-info/SOURCES.txt
--rw-r--r--   0 lmas      (1001) lmas      (1001)        1 2023-01-03 19:38:37.000000 opensimplex-0.4.4/opensimplex.egg-info/dependency_links.txt
--rw-r--r--   0 lmas      (1001) lmas      (1001)        1 2023-01-03 19:38:37.000000 opensimplex-0.4.4/opensimplex.egg-info/not-zip-safe
--rw-r--r--   0 lmas      (1001) lmas      (1001)       12 2023-01-03 19:38:38.000000 opensimplex-0.4.4/opensimplex.egg-info/requires.txt
--rw-r--r--   0 lmas      (1001) lmas      (1001)       18 2023-01-03 19:38:38.000000 opensimplex-0.4.4/opensimplex.egg-info/top_level.txt
--rw-r--r--   0 lmas      (1001) lmas      (1001)       38 2023-01-03 19:38:38.393316 opensimplex-0.4.4/setup.cfg
--rw-r--r--   0 lmas      (1001) lmas      (1001)     1051 2022-08-07 14:30:42.000000 opensimplex-0.4.4/setup.py
-drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2023-01-03 19:38:38.392640 opensimplex-0.4.4/tests/
--rw-r--r--   0 lmas      (1001) lmas      (1001)        0 2022-06-08 13:33:35.000000 opensimplex-0.4.4/tests/__init__.py
--rw-r--r--   0 lmas      (1001) lmas      (1001)     1420 2022-08-05 16:56:16.000000 opensimplex-0.4.4/tests/benchmark_opensimplex.py
--rw-r--r--   0 lmas      (1001) lmas      (1001)     3251 2022-10-14 07:57:33.000000 opensimplex-0.4.4/tests/test_opensimplex.py
+drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2023-07-09 13:37:15.344821 opensimplex-0.4.5/
+-rw-r--r--   0 lmas      (1001) lmas      (1001)     1074 2022-06-08 13:33:35.000000 opensimplex-0.4.5/LICENSE
+-rw-r--r--   0 lmas      (1001) lmas      (1001)       16 2023-04-02 17:34:20.000000 opensimplex-0.4.5/MANIFEST.in
+-rw-r--r--   0 lmas      (1001) lmas      (1001)    10793 2023-07-09 13:37:15.344512 opensimplex-0.4.5/PKG-INFO
+-rw-r--r--   0 lmas      (1001) lmas      (1001)    10141 2023-06-13 12:14:46.000000 opensimplex-0.4.5/README.md
+drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2023-07-09 13:37:15.342371 opensimplex-0.4.5/opensimplex/
+-rw-r--r--   0 lmas      (1001) lmas      (1001)       62 2023-04-02 17:37:23.000000 opensimplex-0.4.5/opensimplex/__init__.py
+-rw-r--r--   0 lmas      (1001) lmas      (1001)     5878 2023-02-18 14:27:39.000000 opensimplex-0.4.5/opensimplex/api.py
+-rw-r--r--   0 lmas      (1001) lmas      (1001)     2651 2022-08-05 16:56:16.000000 opensimplex-0.4.5/opensimplex/constants.py
+-rw-r--r--   0 lmas      (1001) lmas      (1001)    71171 2022-08-05 16:56:16.000000 opensimplex-0.4.5/opensimplex/internals.py
+drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2023-07-09 13:37:15.343320 opensimplex-0.4.5/opensimplex.egg-info/
+-rw-r--r--   0 lmas      (1001) lmas      (1001)    10793 2023-07-09 13:37:14.000000 opensimplex-0.4.5/opensimplex.egg-info/PKG-INFO
+-rw-r--r--   0 lmas      (1001) lmas      (1001)      459 2023-07-09 13:37:15.000000 opensimplex-0.4.5/opensimplex.egg-info/SOURCES.txt
+-rw-r--r--   0 lmas      (1001) lmas      (1001)        1 2023-07-09 13:37:14.000000 opensimplex-0.4.5/opensimplex.egg-info/dependency_links.txt
+-rw-r--r--   0 lmas      (1001) lmas      (1001)        1 2023-07-09 13:25:36.000000 opensimplex-0.4.5/opensimplex.egg-info/not-zip-safe
+-rw-r--r--   0 lmas      (1001) lmas      (1001)       12 2023-07-09 13:37:15.000000 opensimplex-0.4.5/opensimplex.egg-info/requires.txt
+-rw-r--r--   0 lmas      (1001) lmas      (1001)       18 2023-07-09 13:37:15.000000 opensimplex-0.4.5/opensimplex.egg-info/top_level.txt
+-rw-r--r--   0 lmas      (1001) lmas      (1001)       38 2023-07-09 13:37:15.344891 opensimplex-0.4.5/setup.cfg
+-rw-r--r--   0 lmas      (1001) lmas      (1001)     1051 2022-08-07 14:30:42.000000 opensimplex-0.4.5/setup.py
+drwxr-xr-x   0 lmas      (1001) lmas      (1001)        0 2023-07-09 13:37:15.344235 opensimplex-0.4.5/tests/
+-rw-r--r--   0 lmas      (1001) lmas      (1001)        0 2022-06-08 13:33:35.000000 opensimplex-0.4.5/tests/__init__.py
+-rw-r--r--   0 lmas      (1001) lmas      (1001)     1420 2022-08-05 16:56:16.000000 opensimplex-0.4.5/tests/benchmark_opensimplex.py
+-rw-r--r--   0 lmas      (1001) lmas      (1001)    12976 2022-08-05 16:56:16.000000 opensimplex-0.4.5/tests/numpy_shapes.npz
+-rw-r--r--   0 lmas      (1001) lmas      (1001)   235060 2022-06-08 13:33:35.000000 opensimplex-0.4.5/tests/samples.json.gz
+-rw-r--r--   0 lmas      (1001) lmas      (1001)     3401 2023-02-18 14:27:39.000000 opensimplex-0.4.5/tests/test_opensimplex.py
```

### Comparing `opensimplex-0.4.4/LICENSE` & `opensimplex-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opensimplex-0.4.4/PKG-INFO` & `opensimplex-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensimplex
-Version: 0.4.4
+Version: 0.4.5
 Summary: OpenSimplex is a noise generation function like Perlin or Simplex noise, but better.
 Home-page: https://github.com/lmas/opensimplex
 Download-URL: https://github.com/lmas/opensimplex/releases
 Author: Alex
 Author-email: opensimplex@larus.se
 License: MIT
 Keywords: opensimplex simplex noise 2D 3D 4D
@@ -39,14 +39,16 @@
 [Simplex]: https://en.wikipedia.org/wiki/Simplex_noise
 [original code]: https://gist.github.com/KdotJPG/b1270127455a94ac5d19
 
 ## Status
 
 The `master` branch contains the latest code (possibly unstable),
 with automatic tests running for **Python 3.8, 3.9, 3.10 on Linux, MacOS and Windows**.
+**FreeBSD** is also supported, though it's only locally tested as Github Actions
+don't offer FreeBSD support.
 
 Please refer to the [version tags] for the latest stable version.
 
 [version tags]: https://github.com/lmas/opensimplex/tags
 
 
 Updates for **v0.4+**:
@@ -111,14 +113,22 @@
 **random_seed()**
 
     Works just like seed(), except it uses the system time (in ns) as a seed value.
     Not guaranteed to be random so use at your own risk.
 
     random_seed()
 
+**get_seed()**
+
+    Return the value used to seed the initial state.
+    :return: seed as integer
+
+    >>> get_seed()
+    3
+
 **opensimplex.noise2(x, y)**
 
     Generate 2D OpenSimplex noise from X,Y coordinates.
     :param x: x coordinate as float
     :param y: y coordinate as float
     :return:  generated 2D noise as float, between -1.0 and 1.0
```

### Comparing `opensimplex-0.4.4/README.md` & `opensimplex-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 [Simplex]: https://en.wikipedia.org/wiki/Simplex_noise
 [original code]: https://gist.github.com/KdotJPG/b1270127455a94ac5d19
 
 ## Status
 
 The `master` branch contains the latest code (possibly unstable),
 with automatic tests running for **Python 3.8, 3.9, 3.10 on Linux, MacOS and Windows**.
+**FreeBSD** is also supported, though it's only locally tested as Github Actions
+don't offer FreeBSD support.
 
 Please refer to the [version tags] for the latest stable version.
 
 [version tags]: https://github.com/lmas/opensimplex/tags
 
 
 Updates for **v0.4+**:
@@ -93,14 +95,22 @@
 **random_seed()**
 
     Works just like seed(), except it uses the system time (in ns) as a seed value.
     Not guaranteed to be random so use at your own risk.
 
     random_seed()
 
+**get_seed()**
+
+    Return the value used to seed the initial state.
+    :return: seed as integer
+
+    >>> get_seed()
+    3
+
 **opensimplex.noise2(x, y)**
 
     Generate 2D OpenSimplex noise from X,Y coordinates.
     :param x: x coordinate as float
     :param y: y coordinate as float
     :return:  generated 2D noise as float, between -1.0 and 1.0
```

### Comparing `opensimplex-0.4.4/opensimplex/api.py` & `opensimplex-0.4.5/opensimplex/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,24 @@
     Not guaranteed to be random so use at your own risk.
 
     >>> random_seed()
     """
     seed(time.time_ns())
 
 
+def get_seed() -> int:
+    """
+    Return the value used to seed the initial state.
+    :return: seed as integer
+
+    >>> get_seed()
+    3
+    """
+    return _default.get_seed()
+
 def noise2(x: float, y: float) -> float:
     """
     Generate 2D OpenSimplex noise from X,Y coordinates.
     :param x: x coordinate as float
     :param y: y coordinate as float
     :return:  generated 2D noise as float, between -1.0 and 1.0
 
@@ -139,14 +149,18 @@
 
 ################################################################################
 
 # This class is provided for backwards compatibility and might disappear in the future. Use at your own risk.
 class OpenSimplex(object):
     def __init__(self, seed: int) -> None:
         self._perm, self._perm_grad_index3 = _init(seed)
+        self._seed = seed
+
+    def get_seed(self) -> int:
+        return self._seed
 
     def noise2(self, x: float, y: float) -> float:
         return _noise2(x, y, self._perm)
 
     def noise2array(self, x: np.ndarray, y: np.ndarray) -> np.ndarray:
         return _noise2a(x, y, self._perm)
```

### Comparing `opensimplex-0.4.4/opensimplex/constants.py` & `opensimplex-0.4.5/opensimplex/constants.py`

 * *Files identical despite different names*

### Comparing `opensimplex-0.4.4/opensimplex/internals.py` & `opensimplex-0.4.5/opensimplex/internals.py`

 * *Files identical despite different names*

### Comparing `opensimplex-0.4.4/opensimplex.egg-info/PKG-INFO` & `opensimplex-0.4.5/opensimplex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensimplex
-Version: 0.4.4
+Version: 0.4.5
 Summary: OpenSimplex is a noise generation function like Perlin or Simplex noise, but better.
 Home-page: https://github.com/lmas/opensimplex
 Download-URL: https://github.com/lmas/opensimplex/releases
 Author: Alex
 Author-email: opensimplex@larus.se
 License: MIT
 Keywords: opensimplex simplex noise 2D 3D 4D
@@ -39,14 +39,16 @@
 [Simplex]: https://en.wikipedia.org/wiki/Simplex_noise
 [original code]: https://gist.github.com/KdotJPG/b1270127455a94ac5d19
 
 ## Status
 
 The `master` branch contains the latest code (possibly unstable),
 with automatic tests running for **Python 3.8, 3.9, 3.10 on Linux, MacOS and Windows**.
+**FreeBSD** is also supported, though it's only locally tested as Github Actions
+don't offer FreeBSD support.
 
 Please refer to the [version tags] for the latest stable version.
 
 [version tags]: https://github.com/lmas/opensimplex/tags
 
 
 Updates for **v0.4+**:
@@ -111,14 +113,22 @@
 **random_seed()**
 
     Works just like seed(), except it uses the system time (in ns) as a seed value.
     Not guaranteed to be random so use at your own risk.
 
     random_seed()
 
+**get_seed()**
+
+    Return the value used to seed the initial state.
+    :return: seed as integer
+
+    >>> get_seed()
+    3
+
 **opensimplex.noise2(x, y)**
 
     Generate 2D OpenSimplex noise from X,Y coordinates.
     :param x: x coordinate as float
     :param y: y coordinate as float
     :return:  generated 2D noise as float, between -1.0 and 1.0
```

### Comparing `opensimplex-0.4.4/setup.py` & `opensimplex-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `opensimplex-0.4.4/tests/benchmark_opensimplex.py` & `opensimplex-0.4.5/tests/benchmark_opensimplex.py`

 * *Files identical despite different names*

### Comparing `opensimplex-0.4.4/tests/test_opensimplex.py` & `opensimplex-0.4.5/tests/test_opensimplex.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,19 @@
     def test_seeds(self):
         for row in test_seeds:
             simplex.seed(row[0])
             n = simplex.noise2(0.5, 0.5)
             if n != row[1]:
                 self.fail("got %s, expected %s (using seed %s)" % (n, row[1], row[0]))
 
+        got = simplex.get_seed()
+        want = test_seeds[-1][0]
+        if got != want:
+            self.fail("got %s, expected %s" % (got, want))
+
     def load_samples(self):
         for line in gzip.open("tests/samples.json.gz"):
             # Python3: need to decode the line as it's a bytes object and json
             # will only work on strings!
             yield json.loads(line.decode("utf-8"))
 
     def test_samples(self):
@@ -49,15 +54,15 @@
             elif len(s) == 4:
                 expected = s[3]
                 actual = simplex.noise3(s[0], s[1], s[2])
             elif len(s) == 5:
                 expected = s[4]
                 actual = simplex.noise4(s[0], s[1], s[2], s[3])
             else:
-                self.fail("Unexpected sample size: " + str(len(s)))
+                self.fail("unexpected sample size: " + str(len(s)))
             self.assertEqual(expected, actual)
 
     def test_arrays(self):
         # Small sample size for now, using primes for array sizes (or each test run will take too long).
         rng = np.random.default_rng(seed=0)
         ix, iy, iz, iw = rng.random(11), rng.random(7), rng.random(5), rng.random(3)
         simplex.seed(0)
```

