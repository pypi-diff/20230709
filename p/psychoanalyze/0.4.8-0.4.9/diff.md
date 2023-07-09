# Comparing `tmp/psychoanalyze-0.4.8.tar.gz` & `tmp/psychoanalyze-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.4.8.tar", max compression
+gzip compressed data, was "psychoanalyze-0.4.9.tar", max compression
```

## Comparing `psychoanalyze-0.4.8.tar` & `psychoanalyze-0.4.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-07-09 14:01:22.388987 psychoanalyze-0.4.8/LICENSE
--rw-r--r--   0        0        0     1184 2023-07-09 14:01:22.388987 psychoanalyze-0.4.8/README.md
--rw-r--r--   0        0        0     1350 2023-07-09 14:02:41.258006 psychoanalyze-0.4.8/psychoanalyze/__init__.py
--rw-r--r--   0        0        0      749 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/analysis/__init__.py
--rw-r--r--   0        0        0     1281 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/analysis/bayes.py
--rw-r--r--   0        0        0     1113 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/analysis/ecdf.py
--rw-r--r--   0        0        0     2294 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/analysis/strength_duration.py
--rw-r--r--   0        0        0     2366 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/analysis/weber.py
--rw-r--r--   0        0        0     1643 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/__init__.py
--rw-r--r--   0        0        0     8278 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/blocks.py
--rw-r--r--   0        0        0     7675 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/points.py
--rw-r--r--   0        0        0     2861 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/sessions.py
--rw-r--r--   0        0        0      834 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/stimulus.py
--rw-r--r--   0        0        0     1671 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/subjects.py
--rw-r--r--   0        0        0     4936 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/trials.py
--rw-r--r--   0        0        0     3462 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/types.py
--rw-r--r--   0        0        0     1582 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/plot.py
--rw-r--r--   0        0        0     1511 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/sigmoids.py
--rw-r--r--   0        0        0     1985 2023-07-09 14:02:41.258006 psychoanalyze-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     2796 1970-01-01 00:00:00.000000 psychoanalyze-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-09 20:02:37.718055 psychoanalyze-0.4.9/LICENSE
+-rw-r--r--   0        0        0     1184 2023-07-09 20:02:37.718055 psychoanalyze-0.4.9/README.md
+-rw-r--r--   0        0        0     1350 2023-07-09 20:04:14.410827 psychoanalyze-0.4.9/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0      749 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/analysis/__init__.py
+-rw-r--r--   0        0        0     1281 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/analysis/bayes.py
+-rw-r--r--   0        0        0     1113 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/analysis/ecdf.py
+-rw-r--r--   0        0        0     2294 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/analysis/strength_duration.py
+-rw-r--r--   0        0        0     2366 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/analysis/weber.py
+-rw-r--r--   0        0        0     1643 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/__init__.py
+-rw-r--r--   0        0        0     8278 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/blocks.py
+-rw-r--r--   0        0        0     7903 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/points.py
+-rw-r--r--   0        0        0     2861 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/sessions.py
+-rw-r--r--   0        0        0      834 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/stimulus.py
+-rw-r--r--   0        0        0     1671 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/subjects.py
+-rw-r--r--   0        0        0     4936 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/trials.py
+-rw-r--r--   0        0        0     3462 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/data/types.py
+-rw-r--r--   0        0        0     1582 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     1511 2023-07-09 20:02:37.806109 psychoanalyze-0.4.9/psychoanalyze/sigmoids.py
+-rw-r--r--   0        0        0     1985 2023-07-09 20:04:14.410827 psychoanalyze-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     2796 1970-01-01 00:00:00.000000 psychoanalyze-0.4.9/PKG-INFO
```

### Comparing `psychoanalyze-0.4.8/LICENSE` & `psychoanalyze-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/README.md` & `psychoanalyze-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/psychoanalyze/__init__.py` & `psychoanalyze-0.4.9/psychoanalyze/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/psychoanalyze/analysis/__init__.py` & `psychoanalyze-0.4.9/psychoanalyze/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/psychoanalyze/analysis/bayes.py` & `psychoanalyze-0.4.9/psychoanalyze/analysis/bayes.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/psychoanalyze/analysis/ecdf.py` & `psychoanalyze-0.4.9/psychoanalyze/analysis/ecdf.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/psychoanalyze/analysis/strength_duration.py` & `psychoanalyze-0.4.9/psychoanalyze/analysis/strength_duration.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/psychoanalyze/analysis/weber.py` & `psychoanalyze-0.4.9/psychoanalyze/analysis/weber.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/psychoanalyze/data/__init__.py` & `psychoanalyze-0.4.9/psychoanalyze/data/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/psychoanalyze/data/blocks.py` & `psychoanalyze-0.4.9/psychoanalyze/data/blocks.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/psychoanalyze/data/points.py` & `psychoanalyze-0.4.9/psychoanalyze/data/points.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,36 +130,42 @@
     )
 
 
 def hits(
     n: pd.Series,
     threshold: float = 0.0,
     scale: float = 1.0,
+    guess_rate: float = 0.0,
+    lapse_rate: float = 0.0,
 ) -> pd.Series:
     """Sample list of n hits from a list of intensity values."""
+    p = logistic.cdf(n.index.to_numpy(), threshold, scale)
+    psi = guess_rate + (1.0 - guess_rate - lapse_rate) * p
     return pd.Series(
         np.random.default_rng().binomial(
             n,
-            logistic.cdf(n.index.to_numpy(), threshold, scale),
+            psi,
             len(n),
         ),
         index=n.index,
         name="Hits",
     )
 
 
-def generate(
+def generate(  # noqa: PLR0913
     n_trials: int,
     options: list[float],
     threshold: float = 0.0,
     slope: float = 1.0,
+    guess_rate: float = 0.0,
+    lapse_rate: float = 0.0,
 ) -> pd.DataFrame:
     """Generate points-level data."""
     n = generate_n(n_trials, options)
-    _hits = hits(n, threshold, slope)
+    _hits = hits(n, threshold, slope, guess_rate, lapse_rate)
     points = pd.concat([n, _hits], axis=1)
     _hit_rate = hit_rate(points)
     return pd.concat([points, _hit_rate], axis=1)
 
 
 def generate_point(n: int, p: float) -> int:
     """Sample n hits from n trials and probability p from binomial dist."""
```

### Comparing `psychoanalyze-0.4.8/psychoanalyze/data/sessions.py` & `psychoanalyze-0.4.9/psychoanalyze/data/sessions.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/psychoanalyze/data/stimulus.py` & `psychoanalyze-0.4.9/psychoanalyze/data/stimulus.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/psychoanalyze/data/subjects.py` & `psychoanalyze-0.4.9/psychoanalyze/data/subjects.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/psychoanalyze/data/trials.py` & `psychoanalyze-0.4.9/psychoanalyze/data/trials.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/psychoanalyze/data/types.py` & `psychoanalyze-0.4.9/psychoanalyze/data/types.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/psychoanalyze/plot.py` & `psychoanalyze-0.4.9/psychoanalyze/plot.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/psychoanalyze/sigmoids.py` & `psychoanalyze-0.4.9/psychoanalyze/sigmoids.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.8/pyproject.toml` & `psychoanalyze-0.4.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.4.8"
+version = "0.4.9"
 description = "A Pythonic analysis package for psychophysics data"
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.4"
```

### Comparing `psychoanalyze-0.4.8/PKG-INFO` & `psychoanalyze-0.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.4.8
+Version: 0.4.9
 Summary: A Pythonic analysis package for psychophysics data
 License: GPL-3.0-or-later
 Author: Ty Schlichenmeyer
 Author-email: t.schlic@wustl.edu
 Requires-Python: ==3.11.4
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

