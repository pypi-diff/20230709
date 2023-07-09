# Comparing `tmp/hftbacktest-1.6.1.tar.gz` & `tmp/hftbacktest-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hftbacktest-1.6.1.tar", last modified: Mon May 22 14:36:49 2023, max compression
+gzip compressed data, was "hftbacktest-1.6.2.tar", last modified: Sun Jul  9 14:23:09 2023, max compression
```

## Comparing `hftbacktest-1.6.1.tar` & `hftbacktest-1.6.2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.875651 hftbacktest-1.6.1/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/LICENSE
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6805 2023-05-22 14:36:49.875651 hftbacktest-1.6.1/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5696 2023-05-10 14:57:57.000000 hftbacktest-1.6.1/README.rst
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.872651 hftbacktest-1.6.1/hftbacktest/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11523 2023-05-22 14:19:54.000000 hftbacktest-1.6.1/hftbacktest/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/assettype.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    15671 2023-05-17 15:15:26.000000 hftbacktest-1.6.1/hftbacktest/backtest.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.873651 hftbacktest-1.6.1/hftbacktest/data/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1592 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/data/__init__.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.873651 hftbacktest-1.6.1/hftbacktest/data/utils/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/data/utils/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11565 2023-05-22 14:23:10.000000 hftbacktest-1.6.1/hftbacktest/data/utils/binancefutures.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2160 2023-04-30 14:00:09.000000 hftbacktest-1.6.1/hftbacktest/data/utils/snapshot.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6901 2023-04-28 13:18:47.000000 hftbacktest-1.6.1/hftbacktest/data/utils/tardis.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11553 2023-04-28 12:19:24.000000 hftbacktest-1.6.1/hftbacktest/data/validation.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.873651 hftbacktest-1.6.1/hftbacktest/experimental/
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.6.1/hftbacktest/experimental/__init__.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    14543 2023-05-11 12:00:41.000000 hftbacktest-1.6.1/hftbacktest/experimental/backtest.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.874652 hftbacktest-1.6.1/hftbacktest/experimental/live/
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.6.1/hftbacktest/experimental/live/__init__.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    19630 2023-04-29 10:30:43.000000 hftbacktest-1.6.1/hftbacktest/experimental/live/binancefutures.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)      333 2023-04-29 10:30:43.000000 hftbacktest-1.6.1/hftbacktest/experimental/live/custom_strategy.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     7792 2023-04-29 10:30:43.000000 hftbacktest-1.6.1/hftbacktest/experimental/live/ordermanager.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     3578 2023-04-29 10:30:43.000000 hftbacktest-1.6.1/hftbacktest/experimental/live/settings.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     6817 2023-05-11 11:48:17.000000 hftbacktest-1.6.1/hftbacktest/experimental/multiasset.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/marketdepth.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.874652 hftbacktest-1.6.1/hftbacktest/models/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/models/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10010 2023-04-29 14:47:02.000000 hftbacktest-1.6.1/hftbacktest/models/latencies.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3305 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/models/queue.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4150 2023-05-17 14:22:00.000000 hftbacktest-1.6.1/hftbacktest/order.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.874652 hftbacktest-1.6.1/hftbacktest/proc/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/proc/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6538 2023-05-18 14:26:22.000000 hftbacktest-1.6.1/hftbacktest/proc/local.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    19211 2023-05-18 13:30:05.000000 hftbacktest-1.6.1/hftbacktest/proc/nopartialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    29420 2023-05-18 13:41:42.000000 hftbacktest-1.6.1/hftbacktest/proc/partialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5899 2023-05-10 12:56:12.000000 hftbacktest-1.6.1/hftbacktest/proc/proc.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3252 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/hftbacktest/reader.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13687 2023-05-10 13:22:50.000000 hftbacktest-1.6.1/hftbacktest/stat.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-05-11 12:00:32.000000 hftbacktest-1.6.1/hftbacktest/state.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-05-11 11:04:39.000000 hftbacktest-1.6.1/hftbacktest/typing.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-22 14:36:49.873651 hftbacktest-1.6.1/hftbacktest.egg-info/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6805 2023-05-22 14:36:49.000000 hftbacktest-1.6.1/hftbacktest.egg-info/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1248 2023-05-22 14:36:49.000000 hftbacktest-1.6.1/hftbacktest.egg-info/SOURCES.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-05-22 14:36:49.000000 hftbacktest-1.6.1/hftbacktest.egg-info/dependency_links.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.6.1/hftbacktest.egg-info/not-zip-safe
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2023-05-22 14:36:49.000000 hftbacktest-1.6.1/hftbacktest.egg-info/requires.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2023-05-22 14:36:49.000000 hftbacktest-1.6.1/hftbacktest.egg-info/top_level.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1249 2023-05-22 14:36:49.875651 hftbacktest-1.6.1/setup.cfg
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.6.1/setup.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-07-09 14:23:09.933780 hftbacktest-1.6.2/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.6.2/LICENSE
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6805 2023-07-09 14:23:09.933780 hftbacktest-1.6.2/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5696 2023-05-10 14:57:57.000000 hftbacktest-1.6.2/README.rst
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-07-09 14:23:09.931780 hftbacktest-1.6.2/hftbacktest/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11523 2023-07-09 14:20:27.000000 hftbacktest-1.6.2/hftbacktest/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.6.2/hftbacktest/assettype.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    15792 2023-07-09 09:08:34.000000 hftbacktest-1.6.2/hftbacktest/backtest.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-07-09 14:23:09.931780 hftbacktest-1.6.2/hftbacktest/data/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1592 2023-04-27 05:42:48.000000 hftbacktest-1.6.2/hftbacktest/data/__init__.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-07-09 14:23:09.931780 hftbacktest-1.6.2/hftbacktest/data/utils/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.6.2/hftbacktest/data/utils/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11565 2023-05-22 14:23:10.000000 hftbacktest-1.6.2/hftbacktest/data/utils/binancefutures.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2160 2023-04-30 14:00:09.000000 hftbacktest-1.6.2/hftbacktest/data/utils/snapshot.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6959 2023-06-09 13:48:48.000000 hftbacktest-1.6.2/hftbacktest/data/utils/tardis.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11553 2023-04-28 12:19:24.000000 hftbacktest-1.6.2/hftbacktest/data/validation.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-07-09 14:23:09.932780 hftbacktest-1.6.2/hftbacktest/experimental/
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.6.2/hftbacktest/experimental/__init__.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    14543 2023-05-11 12:00:41.000000 hftbacktest-1.6.2/hftbacktest/experimental/backtest.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-07-09 14:23:09.932780 hftbacktest-1.6.2/hftbacktest/experimental/live/
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.6.2/hftbacktest/experimental/live/__init__.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    19630 2023-04-29 10:30:43.000000 hftbacktest-1.6.2/hftbacktest/experimental/live/binancefutures.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)      333 2023-04-29 10:30:43.000000 hftbacktest-1.6.2/hftbacktest/experimental/live/custom_strategy.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     7792 2023-04-29 10:30:43.000000 hftbacktest-1.6.2/hftbacktest/experimental/live/ordermanager.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     3578 2023-04-29 10:30:43.000000 hftbacktest-1.6.2/hftbacktest/experimental/live/settings.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     6817 2023-05-11 11:48:17.000000 hftbacktest-1.6.2/hftbacktest/experimental/multiasset.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-04-27 05:42:48.000000 hftbacktest-1.6.2/hftbacktest/marketdepth.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-07-09 14:23:09.932780 hftbacktest-1.6.2/hftbacktest/models/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.6.2/hftbacktest/models/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10010 2023-07-05 03:52:35.000000 hftbacktest-1.6.2/hftbacktest/models/latencies.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3305 2023-04-27 05:42:48.000000 hftbacktest-1.6.2/hftbacktest/models/queue.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4150 2023-05-17 14:22:00.000000 hftbacktest-1.6.2/hftbacktest/order.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-07-09 14:23:09.933780 hftbacktest-1.6.2/hftbacktest/proc/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.6.2/hftbacktest/proc/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6538 2023-05-18 14:26:22.000000 hftbacktest-1.6.2/hftbacktest/proc/local.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    19211 2023-05-18 13:30:05.000000 hftbacktest-1.6.2/hftbacktest/proc/nopartialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    29420 2023-05-18 13:41:42.000000 hftbacktest-1.6.2/hftbacktest/proc/partialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5899 2023-05-10 12:56:12.000000 hftbacktest-1.6.2/hftbacktest/proc/proc.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3252 2023-04-27 05:42:48.000000 hftbacktest-1.6.2/hftbacktest/reader.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13687 2023-05-10 13:22:50.000000 hftbacktest-1.6.2/hftbacktest/stat.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-05-11 12:00:32.000000 hftbacktest-1.6.2/hftbacktest/state.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     7460 2023-05-26 12:41:56.000000 hftbacktest-1.6.2/hftbacktest/stats.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-05-11 11:04:39.000000 hftbacktest-1.6.2/hftbacktest/typing.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-07-09 14:23:09.931780 hftbacktest-1.6.2/hftbacktest.egg-info/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6805 2023-07-09 14:23:09.000000 hftbacktest-1.6.2/hftbacktest.egg-info/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1269 2023-07-09 14:23:09.000000 hftbacktest-1.6.2/hftbacktest.egg-info/SOURCES.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-07-09 14:23:09.000000 hftbacktest-1.6.2/hftbacktest.egg-info/dependency_links.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.6.2/hftbacktest.egg-info/not-zip-safe
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2023-07-09 14:23:09.000000 hftbacktest-1.6.2/hftbacktest.egg-info/requires.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2023-07-09 14:23:09.000000 hftbacktest-1.6.2/hftbacktest.egg-info/top_level.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1249 2023-07-09 14:23:09.933780 hftbacktest-1.6.2/setup.cfg
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.6.2/setup.py
```

### Comparing `hftbacktest-1.6.1/LICENSE` & `hftbacktest-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/PKG-INFO` & `hftbacktest-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.6.1
+Version: 1.6.2
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
```

### Comparing `hftbacktest-1.6.1/README.rst` & `hftbacktest-1.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/__init__.py` & `hftbacktest-1.6.2/hftbacktest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     'validate_data',
     'correct_local_timestamp',
     'correct_exch_timestamp',
     'correct_exch_timestamp_adjust',
     'correct'
 )
 
-__version__ = '1.6.1'
+__version__ = '1.6.2'
 
 
 # JIT'ed latency models
 ConstantLatency = jitclass()(ConstantLatency_)
 FeedLatency = jitclass()(FeedLatency_)
 ForwardFeedLatency = jitclass()(ForwardFeedLatency_)
 BackwardFeedLatency = jitclass()(BackwardFeedLatency_)
```

### Comparing `hftbacktest-1.6.1/hftbacktest/assettype.py` & `hftbacktest-1.6.2/hftbacktest/assettype.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/backtest.py` & `hftbacktest-1.6.2/hftbacktest/backtest.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,21 @@
     def tick_size(self):
         """
         Tick size
         """
         return self.local.depth.tick_size
 
     @property
+    def lot_size(self):
+        """
+        Lot size
+        """
+        return self.local.depth.lot_size
+
+    @property
     def high_ask_tick(self):
         """
         The highest ask price in the market depth in tick.
         """
         return self.local.depth.high_ask_tick
 
     @property
```

### Comparing `hftbacktest-1.6.1/hftbacktest/data/__init__.py` & `hftbacktest-1.6.2/hftbacktest/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/data/utils/binancefutures.py` & `hftbacktest-1.6.2/hftbacktest/data/utils/binancefutures.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/data/utils/snapshot.py` & `hftbacktest-1.6.2/hftbacktest/data/utils/snapshot.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/data/utils/tardis.py` & `hftbacktest-1.6.2/hftbacktest/data/utils/tardis.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .. import merge_on_local_timestamp, correct, validate_data
 
 
 def convert(
         input_files: List[str],
         output_filename: Optional[str] = None,
         buffer_size: int = 100_000_000,
+        ss_buffer_size: int = 1_000,
         base_latency: float = 0,
         method: Literal['separate', 'adjust'] = 'separate'
 ) -> NDArray:
     r"""
     Converts Tardis.dev data files into a format compatible with HftBacktest.
 
     Args:
@@ -87,16 +88,16 @@
                     ]
                     row_num += 1
                 elif file_type == DEPTH:
                     if cols[4] == 'true':
                         # Prepare to insert DEPTH_SNAPSHOT_EVENT
                         if not is_snapshot:
                             is_snapshot = True
-                            ss_bid = np.empty((1000, 6), np.float64)
-                            ss_ask = np.empty((1000, 6), np.float64)
+                            ss_bid = np.empty((ss_buffer_size, 6), np.float64)
+                            ss_ask = np.empty((ss_buffer_size, 6), np.float64)
                             ss_bid_rn = 0
                             ss_ask_rn = 0
                         if cols[5] == 'bid':
                             ss_bid[ss_bid_rn] = [
                                 4,
                                 int(cols[2]),
                                 int(cols[3]),
```

### Comparing `hftbacktest-1.6.1/hftbacktest/data/validation.py` & `hftbacktest-1.6.2/hftbacktest/data/validation.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/experimental/backtest.py` & `hftbacktest-1.6.2/hftbacktest/experimental/backtest.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/experimental/live/binancefutures.py` & `hftbacktest-1.6.2/hftbacktest/experimental/live/binancefutures.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/experimental/live/ordermanager.py` & `hftbacktest-1.6.2/hftbacktest/experimental/live/ordermanager.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/experimental/live/settings.py` & `hftbacktest-1.6.2/hftbacktest/experimental/live/settings.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/experimental/multiasset.py` & `hftbacktest-1.6.2/hftbacktest/experimental/multiasset.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/marketdepth.py` & `hftbacktest-1.6.2/hftbacktest/marketdepth.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/models/latencies.py` & `hftbacktest-1.6.2/hftbacktest/models/latencies.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/models/queue.py` & `hftbacktest-1.6.2/hftbacktest/models/queue.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/order.py` & `hftbacktest-1.6.2/hftbacktest/order.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/proc/local.py` & `hftbacktest-1.6.2/hftbacktest/proc/local.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/proc/nopartialfillexchange.py` & `hftbacktest-1.6.2/hftbacktest/proc/nopartialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/proc/partialfillexchange.py` & `hftbacktest-1.6.2/hftbacktest/proc/partialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/proc/proc.py` & `hftbacktest-1.6.2/hftbacktest/proc/proc.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/reader.py` & `hftbacktest-1.6.2/hftbacktest/reader.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/stat.py` & `hftbacktest-1.6.2/hftbacktest/stat.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/state.py` & `hftbacktest-1.6.2/hftbacktest/state.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest/typing.py` & `hftbacktest-1.6.2/hftbacktest/typing.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.6.1/hftbacktest.egg-info/PKG-INFO` & `hftbacktest-1.6.2/hftbacktest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.6.1
+Version: 1.6.2
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
```

### Comparing `hftbacktest-1.6.1/hftbacktest.egg-info/SOURCES.txt` & `hftbacktest-1.6.2/hftbacktest.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 hftbacktest/assettype.py
 hftbacktest/backtest.py
 hftbacktest/marketdepth.py
 hftbacktest/order.py
 hftbacktest/reader.py
 hftbacktest/stat.py
 hftbacktest/state.py
+hftbacktest/stats.py
 hftbacktest/typing.py
 hftbacktest.egg-info/PKG-INFO
 hftbacktest.egg-info/SOURCES.txt
 hftbacktest.egg-info/dependency_links.txt
 hftbacktest.egg-info/not-zip-safe
 hftbacktest.egg-info/requires.txt
 hftbacktest.egg-info/top_level.txt
```

### Comparing `hftbacktest-1.6.1/setup.cfg` & `hftbacktest-1.6.2/setup.cfg`

 * *Files identical despite different names*

