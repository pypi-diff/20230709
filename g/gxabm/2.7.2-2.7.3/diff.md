# Comparing `tmp/gxabm-2.7.2.tar.gz` & `tmp/gxabm-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gxabm-2.7.2.tar", last modified: Sat Jun 24 18:45:00 2023, max compression
+gzip compressed data, was "gxabm-2.7.3.tar", last modified: Sun Jul  9 21:01:55 2023, max compression
```

## Comparing `gxabm-2.7.2.tar` & `gxabm-2.7.3.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-24 18:45:00.049835 gxabm-2.7.2/
--rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.7.2/MANIFEST.in
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-24 18:45:00.049650 gxabm-2.7.2/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.7.2/README.md
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-24 18:45:00.040247 gxabm-2.7.2/abm/
--rw-r--r--   0 suderman   (502) staff       (20)        6 2023-06-24 18:44:37.000000 gxabm-2.7.2/abm/VERSION
--rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.7.2/abm/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)     8374 2023-05-01 01:43:54.000000 gxabm-2.7.2/abm/__main__.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-24 18:45:00.046479 gxabm-2.7.2/abm/lib/
--rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.7.2/abm/lib/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)    19882 2023-06-13 14:43:19.000000 gxabm-2.7.2/abm/lib/benchmark.py
--rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.7.2/abm/lib/cloudlaunch.py
--rw-r--r--   0 suderman   (502) staff       (20)     9068 2023-06-13 14:43:19.000000 gxabm-2.7.2/abm/lib/common.py
--rw-r--r--   0 suderman   (502) staff       (20)     5433 2023-06-24 18:27:14.000000 gxabm-2.7.2/abm/lib/config.py
--rw-r--r--   0 suderman   (502) staff       (20)     7902 2023-06-13 14:43:19.000000 gxabm-2.7.2/abm/lib/dataset.py
--rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-29 03:35:40.000000 gxabm-2.7.2/abm/lib/experiment.py
--rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.7.2/abm/lib/folder.py
--rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.7.2/abm/lib/helm.py
--rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.7.2/abm/lib/histories.yml
--rw-r--r--   0 suderman   (502) staff       (20)    11689 2023-06-24 18:44:37.000000 gxabm-2.7.2/abm/lib/history.py
--rw-r--r--   0 suderman   (502) staff       (20)     1217 2023-05-01 01:43:54.000000 gxabm-2.7.2/abm/lib/invocation.py
--rw-r--r--   0 suderman   (502) staff       (20)     5049 2023-06-20 16:56:58.000000 gxabm-2.7.2/abm/lib/job.py
--rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.7.2/abm/lib/kubectl.py
--rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.7.2/abm/lib/library.py
--rw-r--r--   0 suderman   (502) staff       (20)    12347 2023-06-13 14:43:19.000000 gxabm-2.7.2/abm/lib/menu.yml
--rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.7.2/abm/lib/users.py
--rw-r--r--   0 suderman   (502) staff       (20)     7817 2023-05-01 01:43:54.000000 gxabm-2.7.2/abm/lib/workflow.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-24 18:45:00.047428 gxabm-2.7.2/gxabm.egg-info/
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-24 18:44:59.000000 gxabm-2.7.2/gxabm.egg-info/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)      691 2023-06-24 18:44:59.000000 gxabm-2.7.2/gxabm.egg-info/SOURCES.txt
--rw-r--r--   0 suderman   (502) staff       (20)        1 2023-06-24 18:44:59.000000 gxabm-2.7.2/gxabm.egg-info/dependency_links.txt
--rw-r--r--   0 suderman   (502) staff       (20)       49 2023-06-24 18:44:59.000000 gxabm-2.7.2/gxabm.egg-info/entry_points.txt
--rw-r--r--   0 suderman   (502) staff       (20)       48 2023-06-24 18:44:59.000000 gxabm-2.7.2/gxabm.egg-info/requires.txt
--rw-r--r--   0 suderman   (502) staff       (20)        9 2023-06-24 18:44:59.000000 gxabm-2.7.2/gxabm.egg-info/top_level.txt
--rw-r--r--   0 suderman   (502) staff       (20)       38 2023-06-24 18:45:00.049888 gxabm-2.7.2/setup.cfg
--rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.7.2/setup.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-24 18:45:00.049060 gxabm-2.7.2/test/
--rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.7.2/test/__init__.py
--rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.7.2/test/check_tools.py
--rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.7.2/test/metrics.py
--rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.7.2/test/test_environments.py
--rw-r--r--   0 suderman   (502) staff       (20)      718 2023-06-04 14:10:38.000000 gxabm-2.7.2/test/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-09 21:01:55.936751 gxabm-2.7.3/
+-rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.7.3/MANIFEST.in
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-07-09 21:01:55.936564 gxabm-2.7.3/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.7.3/README.md
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-09 21:01:55.927479 gxabm-2.7.3/abm/
+-rw-r--r--   0 suderman   (502) staff       (20)        6 2023-07-09 21:01:19.000000 gxabm-2.7.3/abm/VERSION
+-rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.7.3/abm/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)     8374 2023-05-01 01:43:54.000000 gxabm-2.7.3/abm/__main__.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-09 21:01:55.932971 gxabm-2.7.3/abm/lib/
+-rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.7.3/abm/lib/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)    19884 2023-07-09 21:01:19.000000 gxabm-2.7.3/abm/lib/benchmark.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.7.3/abm/lib/cloudlaunch.py
+-rw-r--r--   0 suderman   (502) staff       (20)     9068 2023-06-26 20:05:31.000000 gxabm-2.7.3/abm/lib/common.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5433 2023-07-09 20:57:14.000000 gxabm-2.7.3/abm/lib/config.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7902 2023-07-09 20:57:14.000000 gxabm-2.7.3/abm/lib/dataset.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-29 03:35:40.000000 gxabm-2.7.3/abm/lib/experiment.py
+-rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.7.3/abm/lib/folder.py
+-rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.7.3/abm/lib/helm.py
+-rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.7.3/abm/lib/histories.yml
+-rw-r--r--   0 suderman   (502) staff       (20)    11689 2023-07-09 20:57:14.000000 gxabm-2.7.3/abm/lib/history.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1217 2023-05-01 01:43:54.000000 gxabm-2.7.3/abm/lib/invocation.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5049 2023-06-26 20:05:31.000000 gxabm-2.7.3/abm/lib/job.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.7.3/abm/lib/kubectl.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.7.3/abm/lib/library.py
+-rw-r--r--   0 suderman   (502) staff       (20)    12347 2023-06-26 20:05:31.000000 gxabm-2.7.3/abm/lib/menu.yml
+-rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.7.3/abm/lib/users.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7817 2023-05-01 01:43:54.000000 gxabm-2.7.3/abm/lib/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-09 21:01:55.933883 gxabm-2.7.3/gxabm.egg-info/
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-07-09 21:01:55.000000 gxabm-2.7.3/gxabm.egg-info/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)      715 2023-07-09 21:01:55.000000 gxabm-2.7.3/gxabm.egg-info/SOURCES.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        1 2023-07-09 21:01:55.000000 gxabm-2.7.3/gxabm.egg-info/dependency_links.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       49 2023-07-09 21:01:55.000000 gxabm-2.7.3/gxabm.egg-info/entry_points.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       48 2023-07-09 21:01:55.000000 gxabm-2.7.3/gxabm.egg-info/requires.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        9 2023-07-09 21:01:55.000000 gxabm-2.7.3/gxabm.egg-info/top_level.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       38 2023-07-09 21:01:55.936801 gxabm-2.7.3/setup.cfg
+-rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.7.3/setup.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-07-09 21:01:55.936002 gxabm-2.7.3/test/
+-rw-r--r--   0 suderman   (502) staff       (20)      543 2023-06-30 04:22:19.000000 gxabm-2.7.3/test/ThreadPoolTests.py
+-rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.7.3/test/__init__.py
+-rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.7.3/test/check_tools.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.7.3/test/metrics.py
+-rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.7.3/test/test_environments.py
+-rw-r--r--   0 suderman   (502) staff       (20)      718 2023-06-04 14:10:38.000000 gxabm-2.7.3/test/workflow.py
```

### Comparing `gxabm-2.7.2/PKG-INFO` & `gxabm-2.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.7.2
+Version: 2.7.3
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.7.2/README.md` & `gxabm-2.7.3/README.md`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/__main__.py` & `gxabm-2.7.3/abm/__main__.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/lib/benchmark.py` & `gxabm-2.7.3/abm/lib/benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
                                 for key in item.keys():
                                     #print(f"Getting dataset for {key} = {item[key]}")
                                     value = _get_dataset_data(gi, item[key])
                                     size += value['size']
                                     elements.append(_make_dataset_element(key, value['id']))
                                 description = dataset_collections.CollectionDescription(
                                     name=name,
-                                    type='paired',
+                                    # type='paired',
                                     elements=elements
                                 )
                                 pairs += 1
                                 # print(json.dumps(description.__dict__, indent=4))
                                 # pprint(description)
                                 collection = gi.histories.create_dataset_collection(
                                     history_id=hid,
```

### Comparing `gxabm-2.7.2/abm/lib/cloudlaunch.py` & `gxabm-2.7.3/abm/lib/cloudlaunch.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/lib/common.py` & `gxabm-2.7.3/abm/lib/common.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/lib/config.py` & `gxabm-2.7.3/abm/lib/config.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/lib/dataset.py` & `gxabm-2.7.3/abm/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/lib/experiment.py` & `gxabm-2.7.3/abm/lib/experiment.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/lib/folder.py` & `gxabm-2.7.3/abm/lib/folder.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/lib/helm.py` & `gxabm-2.7.3/abm/lib/helm.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/lib/history.py` & `gxabm-2.7.3/abm/lib/history.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/lib/invocation.py` & `gxabm-2.7.3/abm/lib/invocation.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/lib/job.py` & `gxabm-2.7.3/abm/lib/job.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/lib/kubectl.py` & `gxabm-2.7.3/abm/lib/kubectl.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/lib/library.py` & `gxabm-2.7.3/abm/lib/library.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/lib/menu.yml` & `gxabm-2.7.3/abm/lib/menu.yml`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/lib/users.py` & `gxabm-2.7.3/abm/lib/users.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/abm/lib/workflow.py` & `gxabm-2.7.3/abm/lib/workflow.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/gxabm.egg-info/PKG-INFO` & `gxabm-2.7.3/gxabm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.7.2
+Version: 2.7.3
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.7.2/gxabm.egg-info/SOURCES.txt` & `gxabm-2.7.3/gxabm.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -24,12 +24,13 @@
 abm/lib/workflow.py
 gxabm.egg-info/PKG-INFO
 gxabm.egg-info/SOURCES.txt
 gxabm.egg-info/dependency_links.txt
 gxabm.egg-info/entry_points.txt
 gxabm.egg-info/requires.txt
 gxabm.egg-info/top_level.txt
+test/ThreadPoolTests.py
 test/__init__.py
 test/check_tools.py
 test/metrics.py
 test/test_environments.py
 test/workflow.py
```

### Comparing `gxabm-2.7.2/setup.py` & `gxabm-2.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/test/check_tools.py` & `gxabm-2.7.3/test/check_tools.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/test/metrics.py` & `gxabm-2.7.3/test/metrics.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.2/test/workflow.py` & `gxabm-2.7.3/test/workflow.py`

 * *Files identical despite different names*

