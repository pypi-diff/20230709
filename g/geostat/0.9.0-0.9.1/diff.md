# Comparing `tmp/geostat-0.9.0.tar.gz` & `tmp/geostat-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geostat-0.9.0.tar", last modified: Tue May 30 04:31:41 2023, max compression
+gzip compressed data, was "geostat-0.9.1.tar", last modified: Sun Jul  9 03:18:35 2023, max compression
```

## Comparing `geostat-0.9.0.tar` & `geostat-0.9.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-05-30 04:31:41.238866 geostat-0.9.0/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    11357 2023-04-25 00:54:47.000000 geostat-0.9.0/LICENSE
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-05-30 04:31:41.238866 geostat-0.9.0/PKG-INFO
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      687 2023-04-25 00:54:47.000000 geostat-0.9.0/README.md
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      679 2023-05-30 04:29:49.000000 geostat-0.9.0/pyproject.toml
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      926 2023-05-30 04:31:41.238866 geostat-0.9.0/setup.cfg
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-05-30 04:31:41.234866 geostat-0.9.0/src/
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-05-30 04:31:41.234866 geostat-0.9.0/src/geostat/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      268 2023-05-30 04:29:31.000000 geostat-0.9.0/src/geostat/__init__.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    20973 2023-05-30 00:23:01.000000 geostat-0.9.0/src/geostat/kernel.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    25489 2023-04-25 00:54:47.000000 geostat-0.9.0/src/geostat/krige.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3658 2023-04-25 05:30:44.000000 geostat-0.9.0/src/geostat/mean.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2620 2023-04-25 00:54:47.000000 geostat-0.9.0/src/geostat/mesh.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2557 2023-04-25 00:54:47.000000 geostat-0.9.0/src/geostat/metric.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    22135 2023-05-30 00:28:09.000000 geostat-0.9.0/src/geostat/model.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3081 2023-05-30 04:22:25.000000 geostat-0.9.0/src/geostat/op.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3163 2023-05-30 00:23:13.000000 geostat-0.9.0/src/geostat/param.py
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-05-30 04:31:41.234866 geostat-0.9.0/src/geostat.egg-info/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-05-30 04:31:41.000000 geostat-0.9.0/src/geostat.egg-info/PKG-INFO
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      616 2023-05-30 04:31:41.000000 geostat-0.9.0/src/geostat.egg-info/SOURCES.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)        1 2023-05-30 04:31:41.000000 geostat-0.9.0/src/geostat.egg-info/dependency_links.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      143 2023-05-30 04:31:41.000000 geostat-0.9.0/src/geostat.egg-info/requires.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)        8 2023-05-30 04:31:41.000000 geostat-0.9.0/src/geostat.egg-info/top_level.txt
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-05-30 04:31:41.238866 geostat-0.9.0/tests/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     4635 2023-04-25 05:30:44.000000 geostat-0.9.0/tests/test_antiderivative.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3732 2023-04-25 05:30:44.000000 geostat-0.9.0/tests/test_delta.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     5731 2023-04-25 05:30:44.000000 geostat-0.9.0/tests/test_gp.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     1147 2023-04-25 00:54:47.000000 geostat-0.9.0/tests/test_krige.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3507 2023-04-25 05:30:44.000000 geostat-0.9.0/tests/test_mcmc.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      768 2023-04-25 00:54:47.000000 geostat-0.9.0/tests/test_mesh.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2625 2023-04-25 05:30:44.000000 geostat-0.9.0/tests/test_metric.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2582 2023-04-25 05:30:44.000000 geostat-0.9.0/tests/test_multigp.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     1393 2023-05-30 00:23:01.000000 geostat-0.9.0/tests/test_quadstack.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3761 2023-04-25 05:30:44.000000 geostat-0.9.0/tests/test_trend.py
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-07-09 03:18:35.648020 geostat-0.9.1/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    11357 2023-04-25 00:54:47.000000 geostat-0.9.1/LICENSE
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    14208 2023-07-09 03:18:35.648020 geostat-0.9.1/PKG-INFO
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      687 2023-04-25 00:54:47.000000 geostat-0.9.1/README.md
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      957 2023-07-09 03:18:17.000000 geostat-0.9.1/pyproject.toml
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)       38 2023-07-09 03:18:35.648020 geostat-0.9.1/setup.cfg
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-07-09 03:18:35.644020 geostat-0.9.1/src/
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-07-09 03:18:35.644020 geostat-0.9.1/src/geostat/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      268 2023-07-09 03:07:36.000000 geostat-0.9.1/src/geostat/__init__.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    20973 2023-05-30 00:23:01.000000 geostat-0.9.1/src/geostat/kernel.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    25489 2023-04-25 00:54:47.000000 geostat-0.9.1/src/geostat/krige.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3658 2023-04-25 05:30:44.000000 geostat-0.9.1/src/geostat/mean.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2620 2023-04-25 00:54:47.000000 geostat-0.9.1/src/geostat/mesh.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2557 2023-04-25 00:54:47.000000 geostat-0.9.1/src/geostat/metric.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    25340 2023-07-09 03:05:58.000000 geostat-0.9.1/src/geostat/model.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3081 2023-07-08 21:32:35.000000 geostat-0.9.1/src/geostat/op.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3163 2023-07-08 21:32:35.000000 geostat-0.9.1/src/geostat/param.py
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-07-09 03:18:35.644020 geostat-0.9.1/src/geostat.egg-info/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    14208 2023-07-09 03:18:35.000000 geostat-0.9.1/src/geostat.egg-info/PKG-INFO
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      625 2023-07-09 03:18:35.000000 geostat-0.9.1/src/geostat.egg-info/SOURCES.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)        1 2023-07-09 03:18:35.000000 geostat-0.9.1/src/geostat.egg-info/dependency_links.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      145 2023-07-09 03:18:35.000000 geostat-0.9.1/src/geostat.egg-info/requires.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)        8 2023-07-09 03:18:35.000000 geostat-0.9.1/src/geostat.egg-info/top_level.txt
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-07-09 03:18:35.648020 geostat-0.9.1/tests/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     4635 2023-04-25 05:30:44.000000 geostat-0.9.1/tests/test_antiderivative.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3732 2023-04-25 05:30:44.000000 geostat-0.9.1/tests/test_delta.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     5731 2023-07-08 23:36:44.000000 geostat-0.9.1/tests/test_gp.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     1147 2023-04-25 00:54:47.000000 geostat-0.9.1/tests/test_krige.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3507 2023-04-25 05:30:44.000000 geostat-0.9.1/tests/test_mcmc.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      768 2023-04-25 00:54:47.000000 geostat-0.9.1/tests/test_mesh.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2625 2023-04-25 05:30:44.000000 geostat-0.9.1/tests/test_metric.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2582 2023-04-25 05:30:44.000000 geostat-0.9.1/tests/test_multigp.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     1274 2023-07-09 00:54:51.000000 geostat-0.9.1/tests/test_pair.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     1393 2023-05-30 00:23:01.000000 geostat-0.9.1/tests/test_quadstack.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3761 2023-04-25 05:30:44.000000 geostat-0.9.1/tests/test_trend.py
```

### Comparing `geostat-0.9.0/LICENSE` & `geostat-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/PKG-INFO` & `geostat-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: geostat
-Version: 0.9.0
+Version: 0.9.1
 Summary: Model spatial data with Gaussian processes
-Home-page: https://code.usgs.gov/mjstephens/geostat
-Author: Michael J. Stephens, Will Chang
 Author-email: "Michael J. Stephens" <mjstephens@usgs.gov>, Will Chang <will@hypergradient.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -207,17 +205,17 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/whdc/geostat
 Keywords: geospatial,spatial,interpolation,gaussian process,krige,kriging
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
+Provides-Extra: extras
 License-File: LICENSE
 
 # geostat
 
 ## Disclaimer
 
 This software is preliminary or provisional and is subject to revision. It is being provided to meet the need for timely best science. The software has not received final approval by the U.S. Geological Survey (USGS). No warranty, expressed or implied, is made by the USGS or the U.S. Government as to the functionality of the software and related material nor shall the fact of release constitute any such warranty. The software is provided on the condition that neither the USGS nor the U.S. Government shall be held liable for any damages resulting from the authorized or unauthorized use of the software.
```

### Comparing `geostat-0.9.0/README.md` & `geostat-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/src/geostat/kernel.py` & `geostat-0.9.1/src/geostat/kernel.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/src/geostat/krige.py` & `geostat-0.9.1/src/geostat/krige.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/src/geostat/mean.py` & `geostat-0.9.1/src/geostat/mean.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/src/geostat/mesh.py` & `geostat-0.9.1/src/geostat/mesh.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/src/geostat/metric.py` & `geostat-0.9.1/src/geostat/metric.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/src/geostat/model.py` & `geostat-0.9.1/src/geostat/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -439,15 +439,15 @@
         # Restore order if things were permuted.
         if cats is not None:
             revperm = np.argsort(perm)
             locs, vals, cats = locs[revperm], vals[revperm], cats[revperm]
 
         return replace(self, locs=locs, vals=vals, cats=cats)
 
-    def predict(self, locs2, cats2=None, subsample=None, reduce=None, tracker=None):
+    def predict(self, locs2, cats2=None, *, subsample=None, reduce=None, tracker=None, pair=False):
         '''
         Performs GP predictions of the mean and variance.
         Has support for batch predictions for large data sets.
         '''
 
         assert subsample is None or self.parameter_sample_size is not None, \
             '`subsample` is only valid with sampled parameters'
@@ -458,104 +458,201 @@
         assert subsample is None or reduce is None, \
             '`subsample` and `reduce` cannot both be given'
 
         if tracker is None: tracker = lambda x: x
 
         assert self.locs.shape[-1] == locs2.shape[-1], 'Mismatch in location dimentions'
         if cats2 is not None:
-            assert cats2.shape == locs2.shape[:-1], 'Mismatched shapes in cats and locs'
+            assert cats2.shape == locs2.shape[:1], 'Mismatched shapes in cats and locs'
 
         def interpolate_batch(A11i, locs1, vals1diff, cats1, locs2, cats2, parameters):
+            """
+            Inputs:
+              locs1.shape = [N1, K]
+              vals1diff.shape = [N1]
+              cats1.shape = [N1]
+              locs2.shape = [N2, K]
+              cats2.shape = [N2]
+
+            Outputs:
+              u2_mean.shape = [N2]
+              u2_var.shape = [N2]
+            """
 
             N1 = len(locs1) # Number of measurements.
 
             # Permute datapoints if cats is given.
             if cats2 is not None:
                 perm = np.argsort(cats2)
                 locs2, cats2 = locs2[perm], cats2[perm]
 
             _, A12 = gp_covariance2(
                 self.gp,
                 tf.constant(locs1, dtype=tf.float32),
-                None if cats1 is None else tf.constant(cats1, dtype=tf.int32),
+                tf.constant(cats1, dtype=tf.int32),
                 tf.constant(locs2, dtype=tf.float32),
-                None if cats2 is None else tf.constant(cats2, dtype=tf.int32),
+                tf.constant(cats2, dtype=tf.int32),
                 N1,
                 parameters)
 
             m2, A22 = gp_covariance(
                 self.gp,
                 tf.constant(locs2, dtype=tf.float32),
-                None if cats2 is None else tf.constant(cats2, dtype=tf.int32),
+                tf.constant(cats2, dtype=tf.int32),
                 parameters)
 
             # Restore order if things were permuted.
             if cats2 is not None:
                 revperm = np.argsort(perm)
                 m2 = tf.gather(m2, revperm)
                 A12 = tf.gather(A12, revperm, axis=-1)
                 A22 = tf.gather(tf.gather(A22, revperm), revperm, axis=-1)
 
             u2_mean = m2 + tf.einsum('ab,a->b', A12, tf.einsum('ab,b->a', A11i, vals1diff))
             u2_var = tf.linalg.diag_part(A22) -  tf.einsum('ab,ab->b', A12, tf.matmul(A11i, A12))
 
             return u2_mean, u2_var
 
-        def interpolate(locs1, vals1, cats1, locs2, cats2, parameters):
+        def interpolate_pair_batch(A11i, locs1, vals1diff, cats1, locs2, cats2, parameters):
+            """
+            Inputs:
+              locs1.shape = [N1, K]
+              vals1diff.shape = [N1]
+              cats1.shape = [N1]
+              locs2.shape = [N2, 2, K]
+              cats2.shape = [N2]
+
+            Outputs:
+              u2_mean.shape = [N2, 2]
+              u2_var.shape = [N2, 2, 2]
+            """
+
+            N1 = len(locs1) # Number of measurements.
+            N2 = len(locs2) # Number of prediction pairs.
+
+            # Permute datapoints if cats is given.
+            perm = np.argsort(cats2)
+            locs2, cats2 = locs2[perm], cats2[perm]
+
+            _, A12 = gp_covariance2(
+                self.gp,
+                tf.constant(locs1, dtype=tf.float32),
+                tf.constant(cats1, dtype=tf.int32),
+                tf.constant(locs2[:, 0, :], dtype=tf.float32),
+                tf.constant(cats2, dtype=tf.int32),
+                N1,
+                parameters)
+
+            _, A13 = gp_covariance2(
+                self.gp,
+                tf.constant(locs1, dtype=tf.float32),
+                tf.constant(cats1, dtype=tf.int32),
+                tf.constant(locs2[:, 1, :], dtype=tf.float32),
+                tf.constant(cats2, dtype=tf.int32),
+                N1,
+                parameters)
+
+            m2, A22 = gp_covariance(
+                self.gp,
+                tf.constant(locs2[:, 0, :], dtype=tf.float32),
+                tf.constant(cats2, dtype=tf.int32),
+                parameters)
+
+            m3, A33 = gp_covariance(
+                self.gp,
+                tf.constant(locs2[:, 1, :], dtype=tf.float32),
+                tf.constant(cats2, dtype=tf.int32),
+                parameters)
+
+            _, A23 = gp_covariance2(
+                self.gp,
+                tf.constant(locs2[:, 0, :], dtype=tf.float32),
+                tf.constant(cats2, dtype=tf.int32),
+                tf.constant(locs2[:, 1, :], dtype=tf.float32),
+                tf.constant(cats2, dtype=tf.int32),
+                N2,
+                parameters)
+
+            # Reassemble into more useful shapes.
+
+            A12 = tf.stack([A12, A13], axis=-1) # [N1, N2, 2]
+
+            m2 = tf.stack([m2, m3], axis=-1) # [N2, 2]
+
+            A22 = tf.linalg.diag_part(A22)
+            A33 = tf.linalg.diag_part(A33)
+            A23 = tf.linalg.diag_part(A23)
+            A22 = tf.stack([tf.stack([A22, A23], axis=-1), tf.stack([A23, A33], axis=-1)], axis=-2) # [N2, 2, 2]
+
+            # Restore order if things were permuted.
+            revperm = np.argsort(perm)
+            m2 = tf.gather(m2, revperm)
+            A12 = tf.gather(A12, revperm, axis=1)
+            A22 = tf.gather(A22, revperm)
+
+            u2_mean = m2 + tf.einsum('abc,a->bc', A12, tf.einsum('ab,b->a', A11i, vals1diff))
+            u2_var = A22 - tf.einsum('abc,abd->bcd', A12, tf.einsum('ae,ebd->abd', A11i, A12))
+
+            return u2_mean, u2_var
+
+        def interpolate(locs1, vals1, cats1, locs2, cats2, parameters, pair=False):
             # Interpolate in batches.
             batch_size = self.locs.shape[0] // 2
 
             for_gp = []
-            locs2r = locs2.reshape([-1, locs2.shape[-1]])
-            if cats2 is not None:
-                cats2r = cats2.ravel()
-            else:
-                cats2r = np.zeros_like(locs2r[..., 0], np.int32)
 
-            for start in np.arange(0, len(locs2r), batch_size):
+            if cats2 is None:
+                cats2 = np.zeros(locs2.shape[:1], np.int32)
+
+            for start in np.arange(0, len(locs2), batch_size):
                 stop = start + batch_size
-                subset = locs2r[start:stop], cats2r[start:stop]
+                subset = locs2[start:stop], cats2[start:stop]
                 for_gp.append(subset)
 
             # Permute datapoints if cats is given.
             if cats1 is not None:
                 perm = np.argsort(cats1)
                 locs1, vals1, cats1 = locs1[perm], vals1[perm], cats1[perm]
+            else:
+                perm = None
+                cats1 = np.zeros_like(locs1[..., 0], np.int32)
 
             m1, A11 = gp_covariance(
                 self.gp,
                 tf.constant(locs1, dtype=tf.float32),
-                None if cats1 is None else tf.constant(cats1, dtype=tf.int32),
+                tf.constant(cats1, dtype=tf.int32),
                 parameters)
 
             A11i = tf.linalg.inv(A11)
 
             u2_mean_s = []
             u2_var_s = []
 
+            f = interpolate_pair_batch if pair else interpolate_batch
+
             for locs_subset, cats_subset in for_gp:
-                u2_mean, u2_var = interpolate_batch(A11i, locs1, vals1 - m1, cats1, locs_subset, cats_subset, parameters)
+                u2_mean, u2_var = f(A11i, locs1, vals1 - m1, cats1, locs_subset, cats_subset, parameters)
                 u2_mean = u2_mean.numpy()
                 u2_var = u2_var.numpy()
                 u2_mean_s.append(u2_mean)
                 u2_var_s.append(u2_var)
 
-            u2_mean = np.concatenate(u2_mean_s).reshape(locs2.shape[:-1])
-            u2_var = np.concatenate(u2_var_s).reshape(locs2.shape[:-1])
+            u2_mean = np.concatenate(u2_mean_s)
+            u2_var = np.concatenate(u2_var_s)
 
             return u2_mean, u2_var
 
         if self.parameter_sample_size is None:
-            m, v = interpolate(self.locs, self.vals, self.cats, locs2, cats2, self.parameters)
+            m, v = interpolate(self.locs, self.vals, self.cats, locs2, cats2, self.parameters, pair)
         elif reduce == 'median':
             p = tf.nest.map_structure(lambda x: np.quantile(x, 0.5, axis=0).astype(np.float32), self.parameters)
-            m, v = interpolate(self.locs, self.vals, self.cats, locs2, cats2, p)
+            m, v = interpolate(self.locs, self.vals, self.cats, locs2, cats2, p, pair)
         elif reduce == 'mean':
             p = tf.nest.map_structure(lambda x: x.mean(axis=0).astype(np.float32), self.parameters)
-            m, v = interpolate(self.locs, self.vals, self.cats, locs2, cats2, p)
+            m, v = interpolate(self.locs, self.vals, self.cats, locs2, cats2, p, pair)
         else:
             samples = self.parameter_sample_size
 
             if subsample is not None:
                 assert subsample <= samples, '`subsample` may not exceed sample size'
             else:
                 subsample = samples
@@ -565,14 +662,14 @@
             pick = np.concatenate([[True], a[1:] >= a[:-1]])
             parameters = tf.nest.map_structure(lambda x: x[pick], self.parameters)
 
             # Make a prediction for each sample.
             results = []
             for i in tracker(range(subsample)):
                 p = tf.nest.map_structure(lambda x: x[i], parameters)
-                results.append(interpolate(self.locs, self.vals, self.cats, locs2, cats2, p))
+                results.append(interpolate(self.locs, self.vals, self.cats, locs2, cats2, p, pair))
 
             mm, vv = [np.stack(x) for x in zip(*results)]
             m = mm.mean(axis=0)
             v = (np.square(mm) + vv).mean(axis=0) - np.square(m)
 
         return m, v
```

### Comparing `geostat-0.9.0/src/geostat/op.py` & `geostat-0.9.1/src/geostat/op.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/src/geostat/param.py` & `geostat-0.9.1/src/geostat/param.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/src/geostat.egg-info/PKG-INFO` & `geostat-0.9.1/src/geostat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: geostat
-Version: 0.9.0
+Version: 0.9.1
 Summary: Model spatial data with Gaussian processes
-Home-page: https://code.usgs.gov/mjstephens/geostat
-Author: Michael J. Stephens, Will Chang
 Author-email: "Michael J. Stephens" <mjstephens@usgs.gov>, Will Chang <will@hypergradient.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -207,17 +205,17 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/whdc/geostat
 Keywords: geospatial,spatial,interpolation,gaussian process,krige,kriging
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
+Provides-Extra: extras
 License-File: LICENSE
 
 # geostat
 
 ## Disclaimer
 
 This software is preliminary or provisional and is subject to revision. It is being provided to meet the need for timely best science. The software has not received final approval by the U.S. Geological Survey (USGS). No warranty, expressed or implied, is made by the USGS or the U.S. Government as to the functionality of the software and related material nor shall the fact of release constitute any such warranty. The software is provided on the condition that neither the USGS nor the U.S. Government shall be held liable for any damages resulting from the authorized or unauthorized use of the software.
```

### Comparing `geostat-0.9.0/src/geostat.egg-info/SOURCES.txt` & `geostat-0.9.1/src/geostat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 src/geostat/__init__.py
 src/geostat/kernel.py
 src/geostat/krige.py
 src/geostat/mean.py
 src/geostat/mesh.py
 src/geostat/metric.py
 src/geostat/model.py
@@ -20,9 +19,10 @@
 tests/test_delta.py
 tests/test_gp.py
 tests/test_krige.py
 tests/test_mcmc.py
 tests/test_mesh.py
 tests/test_metric.py
 tests/test_multigp.py
+tests/test_pair.py
 tests/test_quadstack.py
 tests/test_trend.py
```

### Comparing `geostat-0.9.0/tests/test_antiderivative.py` & `geostat-0.9.1/tests/test_antiderivative.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/tests/test_delta.py` & `geostat-0.9.1/tests/test_delta.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/tests/test_gp.py` & `geostat-0.9.1/tests/test_gp.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/tests/test_krige.py` & `geostat-0.9.1/tests/test_krige.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/tests/test_mcmc.py` & `geostat-0.9.1/tests/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/tests/test_mesh.py` & `geostat-0.9.1/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/tests/test_metric.py` & `geostat-0.9.1/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/tests/test_multigp.py` & `geostat-0.9.1/tests/test_multigp.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/tests/test_quadstack.py` & `geostat-0.9.1/tests/test_quadstack.py`

 * *Files identical despite different names*

### Comparing `geostat-0.9.0/tests/test_trend.py` & `geostat-0.9.1/tests/test_trend.py`

 * *Files identical despite different names*

