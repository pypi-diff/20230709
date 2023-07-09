# Comparing `tmp/psychoanalyze-0.4.7.tar.gz` & `tmp/psychoanalyze-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.4.7.tar", max compression
+gzip compressed data, was "psychoanalyze-0.4.8.tar", max compression
```

## Comparing `psychoanalyze-0.4.7.tar` & `psychoanalyze-0.4.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-07-09 13:22:22.800537 psychoanalyze-0.4.7/LICENSE
--rw-r--r--   0        0        0     1184 2023-07-09 13:22:22.800537 psychoanalyze-0.4.7/README.md
--rw-r--r--   0        0        0     1350 2023-07-09 13:23:42.584736 psychoanalyze-0.4.7/psychoanalyze/__init__.py
--rw-r--r--   0        0        0      749 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/analysis/__init__.py
--rw-r--r--   0        0        0     1281 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/analysis/bayes.py
--rw-r--r--   0        0        0     1113 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/analysis/ecdf.py
--rw-r--r--   0        0        0     2294 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/analysis/strength_duration.py
--rw-r--r--   0        0        0     2366 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/analysis/weber.py
--rw-r--r--   0        0        0     1643 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/__init__.py
--rw-r--r--   0        0        0     8278 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/blocks.py
--rw-r--r--   0        0        0     7675 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/points.py
--rw-r--r--   0        0        0     2861 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/sessions.py
--rw-r--r--   0        0        0      834 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/stimulus.py
--rw-r--r--   0        0        0     1671 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/subjects.py
--rw-r--r--   0        0        0     4936 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/trials.py
--rw-r--r--   0        0        0     3462 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/data/types.py
--rw-r--r--   0        0        0     1582 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/plot.py
--rw-r--r--   0        0        0     1511 2023-07-09 13:22:22.876537 psychoanalyze-0.4.7/psychoanalyze/sigmoids.py
--rw-r--r--   0        0        0     1985 2023-07-09 13:23:42.584736 psychoanalyze-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     2796 1970-01-01 00:00:00.000000 psychoanalyze-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-09 14:01:22.388987 psychoanalyze-0.4.8/LICENSE
+-rw-r--r--   0        0        0     1184 2023-07-09 14:01:22.388987 psychoanalyze-0.4.8/README.md
+-rw-r--r--   0        0        0     1350 2023-07-09 14:02:41.258006 psychoanalyze-0.4.8/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0      749 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/analysis/__init__.py
+-rw-r--r--   0        0        0     1281 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/analysis/bayes.py
+-rw-r--r--   0        0        0     1113 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/analysis/ecdf.py
+-rw-r--r--   0        0        0     2294 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/analysis/strength_duration.py
+-rw-r--r--   0        0        0     2366 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/analysis/weber.py
+-rw-r--r--   0        0        0     1643 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/__init__.py
+-rw-r--r--   0        0        0     8278 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/blocks.py
+-rw-r--r--   0        0        0     7675 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/points.py
+-rw-r--r--   0        0        0     2861 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/sessions.py
+-rw-r--r--   0        0        0      834 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/stimulus.py
+-rw-r--r--   0        0        0     1671 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/subjects.py
+-rw-r--r--   0        0        0     4936 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/trials.py
+-rw-r--r--   0        0        0     3462 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/data/types.py
+-rw-r--r--   0        0        0     1582 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     1511 2023-07-09 14:01:22.460988 psychoanalyze-0.4.8/psychoanalyze/sigmoids.py
+-rw-r--r--   0        0        0     1985 2023-07-09 14:02:41.258006 psychoanalyze-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     2796 1970-01-01 00:00:00.000000 psychoanalyze-0.4.8/PKG-INFO
```

### Comparing `psychoanalyze-0.4.7/LICENSE` & `psychoanalyze-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/README.md` & `psychoanalyze-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/__init__.py` & `psychoanalyze-0.4.8/psychoanalyze/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/analysis/__init__.py` & `psychoanalyze-0.4.8/psychoanalyze/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/analysis/bayes.py` & `psychoanalyze-0.4.8/psychoanalyze/analysis/bayes.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/analysis/ecdf.py` & `psychoanalyze-0.4.8/psychoanalyze/analysis/ecdf.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/analysis/strength_duration.py` & `psychoanalyze-0.4.8/psychoanalyze/analysis/strength_duration.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/analysis/weber.py` & `psychoanalyze-0.4.8/psychoanalyze/analysis/weber.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/data/__init__.py` & `psychoanalyze-0.4.8/psychoanalyze/data/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/data/blocks.py` & `psychoanalyze-0.4.8/psychoanalyze/data/blocks.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/data/points.py` & `psychoanalyze-0.4.8/psychoanalyze/data/points.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/data/sessions.py` & `psychoanalyze-0.4.8/psychoanalyze/data/sessions.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/data/stimulus.py` & `psychoanalyze-0.4.8/psychoanalyze/data/stimulus.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/data/subjects.py` & `psychoanalyze-0.4.8/psychoanalyze/data/subjects.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/data/trials.py` & `psychoanalyze-0.4.8/psychoanalyze/data/trials.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/data/types.py` & `psychoanalyze-0.4.8/psychoanalyze/data/types.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/plot.py` & `psychoanalyze-0.4.8/psychoanalyze/plot.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/psychoanalyze/sigmoids.py` & `psychoanalyze-0.4.8/psychoanalyze/sigmoids.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.4.7/pyproject.toml` & `psychoanalyze-0.4.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.4.7"
+version = "0.4.8"
 description = "A Pythonic analysis package for psychophysics data"
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.4"
```

### Comparing `psychoanalyze-0.4.7/PKG-INFO` & `psychoanalyze-0.4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.4.7
+Version: 0.4.8
 Summary: A Pythonic analysis package for psychophysics data
 License: GPL-3.0-or-later
 Author: Ty Schlichenmeyer
 Author-email: t.schlic@wustl.edu
 Requires-Python: ==3.11.4
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

