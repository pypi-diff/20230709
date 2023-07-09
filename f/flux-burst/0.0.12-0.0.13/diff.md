# Comparing `tmp/flux-burst-0.0.12.tar.gz` & `tmp/flux-burst-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-burst-0.0.12.tar", last modified: Tue Jul  4 01:36:56 2023, max compression
+gzip compressed data, was "flux-burst-0.0.13.tar", last modified: Sun Jul  9 17:00:05 2023, max compression
```

## Comparing `flux-burst-0.0.12.tar` & `flux-burst-0.0.13.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:36:56.450937 flux-burst-0.0.12/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-23 19:26:31.000000 flux-burst-0.0.12/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-23 19:26:31.000000 flux-burst-0.0.12/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      313 2023-06-23 19:45:55.000000 flux-burst-0.0.12/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-23 19:26:31.000000 flux-burst-0.0.12/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-04 01:36:56.450937 flux-burst-0.0.12/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3880 2023-07-03 07:21:31.000000 flux-burst-0.0.12/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:36:56.446937 flux-burst-0.0.12/flux_burst.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-04 01:36:55.000000 flux-burst-0.0.12/flux_burst.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      744 2023-07-04 01:36:56.000000 flux-burst-0.0.12/flux_burst.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-04 01:36:55.000000 flux-burst-0.0.12/flux_burst.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2023-07-04 01:36:55.000000 flux-burst-0.0.12/flux_burst.egg-info/entry_points.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:17:14.000000 flux-burst-0.0.12/flux_burst.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      177 2023-07-04 01:36:55.000000 flux-burst-0.0.12/flux_burst.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       10 2023-07-04 01:36:55.000000 flux-burst-0.0.12/flux_burst.egg-info/top_level.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:36:56.446937 flux-burst-0.0.12/fluxburst/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       62 2023-06-23 19:45:55.000000 flux-burst-0.0.12/fluxburst/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8590 2023-07-04 01:36:48.000000 flux-burst-0.0.12/fluxburst/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      746 2023-07-01 06:52:00.000000 flux-burst-0.0.12/fluxburst/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7534 2023-07-03 07:21:31.000000 flux-burst-0.0.12/fluxburst/handles.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:36:56.450937 flux-burst-0.0.12/fluxburst/kubernetes/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      209 2023-07-01 06:52:00.000000 flux-burst-0.0.12/fluxburst/kubernetes/README.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-07-01 06:52:00.000000 flux-burst-0.0.12/fluxburst/kubernetes/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5200 2023-07-04 01:36:48.000000 flux-burst-0.0.12/fluxburst/kubernetes/cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8931 2023-07-04 01:36:48.000000 flux-burst-0.0.12/fluxburst/kubernetes/plugins.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6127 2023-06-23 19:43:36.000000 flux-burst-0.0.12/fluxburst/logger.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2831 2023-07-04 00:51:56.000000 flux-burst-0.0.12/fluxburst/plugins.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      365 2023-06-24 04:45:23.000000 flux-burst-0.0.12/fluxburst/selectors.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      444 2023-06-24 04:45:23.000000 flux-burst-0.0.12/fluxburst/sorting.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-04 01:36:56.450937 flux-burst-0.0.12/fluxburst/utils/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      540 2023-06-23 19:26:33.000000 flux-burst-0.0.12/fluxburst/utils/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6250 2023-07-04 01:36:48.000000 flux-burst-0.0.12/fluxburst/utils/fileio.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1692 2023-06-23 19:41:30.000000 flux-burst-0.0.12/fluxburst/utils/misc.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3188 2023-06-23 19:45:55.000000 flux-burst-0.0.12/fluxburst/utils/terminal.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1263 2023-07-04 01:36:48.000000 flux-burst-0.0.12/fluxburst/version.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 19:26:31.000000 flux-burst-0.0.12/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      210 2023-07-04 01:36:56.450937 flux-burst-0.0.12/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3578 2023-07-01 06:52:00.000000 flux-burst-0.0.12/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-09 17:00:05.259153 flux-burst-0.0.13/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-23 19:26:31.000000 flux-burst-0.0.13/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-23 19:26:31.000000 flux-burst-0.0.13/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      313 2023-06-23 19:45:55.000000 flux-burst-0.0.13/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-23 19:26:31.000000 flux-burst-0.0.13/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-09 17:00:05.259153 flux-burst-0.0.13/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3880 2023-07-03 07:21:31.000000 flux-burst-0.0.13/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-09 17:00:05.259153 flux-burst-0.0.13/flux_burst.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-09 17:00:04.000000 flux-burst-0.0.13/flux_burst.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      744 2023-07-09 17:00:05.000000 flux-burst-0.0.13/flux_burst.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-09 17:00:04.000000 flux-burst-0.0.13/flux_burst.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2023-07-09 17:00:04.000000 flux-burst-0.0.13/flux_burst.egg-info/entry_points.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:17:14.000000 flux-burst-0.0.13/flux_burst.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      177 2023-07-09 17:00:04.000000 flux-burst-0.0.13/flux_burst.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       10 2023-07-09 17:00:04.000000 flux-burst-0.0.13/flux_burst.egg-info/top_level.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-09 17:00:05.259153 flux-burst-0.0.13/fluxburst/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       62 2023-06-23 19:45:55.000000 flux-burst-0.0.13/fluxburst/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8590 2023-07-04 01:36:48.000000 flux-burst-0.0.13/fluxburst/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      746 2023-07-01 06:52:00.000000 flux-burst-0.0.13/fluxburst/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7538 2023-07-09 17:00:01.000000 flux-burst-0.0.13/fluxburst/handles.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-09 17:00:05.259153 flux-burst-0.0.13/fluxburst/kubernetes/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      209 2023-07-01 06:52:00.000000 flux-burst-0.0.13/fluxburst/kubernetes/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-07-01 06:52:00.000000 flux-burst-0.0.13/fluxburst/kubernetes/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5200 2023-07-04 01:36:48.000000 flux-burst-0.0.13/fluxburst/kubernetes/cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8953 2023-07-09 17:00:01.000000 flux-burst-0.0.13/fluxburst/kubernetes/plugins.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6127 2023-06-23 19:43:36.000000 flux-burst-0.0.13/fluxburst/logger.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2831 2023-07-04 00:51:56.000000 flux-burst-0.0.13/fluxburst/plugins.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      365 2023-07-09 16:49:50.000000 flux-burst-0.0.13/fluxburst/selectors.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      444 2023-06-24 04:45:23.000000 flux-burst-0.0.13/fluxburst/sorting.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-09 17:00:05.259153 flux-burst-0.0.13/fluxburst/utils/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      540 2023-06-23 19:26:33.000000 flux-burst-0.0.13/fluxburst/utils/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6250 2023-07-04 01:36:48.000000 flux-burst-0.0.13/fluxburst/utils/fileio.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1692 2023-06-23 19:41:30.000000 flux-burst-0.0.13/fluxburst/utils/misc.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3188 2023-06-23 19:45:55.000000 flux-burst-0.0.13/fluxburst/utils/terminal.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1263 2023-07-09 17:00:01.000000 flux-burst-0.0.13/fluxburst/version.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 19:26:31.000000 flux-burst-0.0.13/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      210 2023-07-09 17:00:05.259153 flux-burst-0.0.13/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3578 2023-07-01 06:52:00.000000 flux-burst-0.0.13/setup.py
```

### Comparing `flux-burst-0.0.12/LICENSE` & `flux-burst-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.12/NOTICE` & `flux-burst-0.0.13/NOTICE`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.12/PKG-INFO` & `flux-burst-0.0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst
-Version: 0.0.12
+Version: 0.0.13
 Summary: Flux module that enables burstable plugins.
 Home-page: https://github.com/converged-computing/flux-burst
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flux-burst Version: 0.0.12 Summary: Flux module
+Metadata-Version: 2.1 Name: flux-burst Version: 0.0.13 Summary: Flux module
 that enables burstable plugins. Home-page: https://github.com/converged-
 computing/flux-burst Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting Platform: UNKNOWN Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
```

### Comparing `flux-burst-0.0.12/README.md` & `flux-burst-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.12/flux_burst.egg-info/PKG-INFO` & `flux-burst-0.0.13/flux_burst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst
-Version: 0.0.12
+Version: 0.0.13
 Summary: Flux module that enables burstable plugins.
 Home-page: https://github.com/converged-computing/flux-burst
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flux-burst Version: 0.0.12 Summary: Flux module
+Metadata-Version: 2.1 Name: flux-burst Version: 0.0.13 Summary: Flux module
 that enables burstable plugins. Home-page: https://github.com/converged-
 computing/flux-burst Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting Platform: UNKNOWN Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
```

### Comparing `flux-burst-0.0.12/flux_burst.egg-info/SOURCES.txt` & `flux-burst-0.0.13/flux_burst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.12/fluxburst/client.py` & `flux-burst-0.0.13/fluxburst/client.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.12/fluxburst/defaults.py` & `flux-burst-0.0.13/fluxburst/defaults.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.12/fluxburst/handles.py` & `flux-burst-0.0.13/fluxburst/handles.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,18 +183,18 @@
 
     def update_jobspec(self, job):
         """
         Update a jobspec via the kvs
         """
         import flux.job
 
-        # Update the KVS (is this possible)?
-        # This doesn't currently work, so not doing anything :)
+        # This is a workaround because updating the attribute directly
+        # does not stick yet.
         kvs = flux.job.job_kvs(self.handle, job["id"])
-        kvs["jobspec"] = job["spec"]
+        kvs[kvs.key_at("jobspec")] = job["spec"]
         kvs.commit()
         return kvs
 
     def list_jobs(self):
         """
         List actual jobs from the flux.job module
         """
```

### Comparing `flux-burst-0.0.12/fluxburst/kubernetes/cluster.py` & `flux-burst-0.0.13/fluxburst/kubernetes/cluster.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.12/fluxburst/kubernetes/plugins.py` & `flux-burst-0.0.13/fluxburst/kubernetes/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         Given some set of scheduled jobs, run bursting.
 
         If request_burst is True, a specific number of tasks and size
         must be provided to request a cluster in advance (that jobs can
         be run on).
         """
         # Exit early if no jobs to burst
-        if not self.jobs:
+        if not self.jobs and not request_burst:
             logger.info(f"Plugin {self.name} has no jobs to burst.")
             return
 
         # If we have requested a burst, tasks and size are required
         if request_burst and (not tasks or not nodes):
             logger.warning("Burst requests require nodes and tasks.")
             return
```

### Comparing `flux-burst-0.0.12/fluxburst/logger.py` & `flux-burst-0.0.13/fluxburst/logger.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.12/fluxburst/plugins.py` & `flux-burst-0.0.13/fluxburst/plugins.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.12/fluxburst/utils/__init__.py` & `flux-burst-0.0.13/fluxburst/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.12/fluxburst/utils/fileio.py` & `flux-burst-0.0.13/fluxburst/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.12/fluxburst/utils/misc.py` & `flux-burst-0.0.13/fluxburst/utils/misc.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.12/fluxburst/utils/terminal.py` & `flux-burst-0.0.13/fluxburst/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.12/fluxburst/version.py` & `flux-burst-0.0.13/fluxburst/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.12"
+__version__ = "0.0.13"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "flux-burst"
 PACKAGE_URL = "https://github.com/converged-computing/flux-burst"
 KEYWORDS = "cloud, flux-framework, flux, bursting"
 DESCRIPTION = "Flux module that enables burstable plugins."
 LICENSE = "LICENSE"
```

### Comparing `flux-burst-0.0.12/setup.py` & `flux-burst-0.0.13/setup.py`

 * *Files identical despite different names*

