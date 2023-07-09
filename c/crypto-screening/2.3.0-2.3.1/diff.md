# Comparing `tmp/crypto-screening-2.3.0.tar.gz` & `tmp/crypto-screening-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-2.3.0.tar", last modified: Sun Jul  9 07:55:36 2023, max compression
+gzip compressed data, was "crypto-screening-2.3.1.tar", last modified: Sun Jul  9 08:02:36 2023, max compression
```

## Comparing `crypto-screening-2.3.0.tar` & `crypto-screening-2.3.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 07:55:36.886613 crypto-screening-2.3.0/
--rw-rw-rw-   0        0        0       98 2023-07-09 07:55:36.000000 crypto-screening-2.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-09 07:55:36.886613 crypto-screening-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.3.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.3.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-09 07:55:36.858643 crypto-screening-2.3.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-09 07:55:36.874638 crypto-screening-2.3.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.3.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-2.3.0/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    49469 2023-07-09 07:51:36.000000 crypto-screening-2.3.0/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    11824 2023-07-06 12:48:49.000000 crypto-screening-2.3.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.3.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-2.3.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.3.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.3.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-09 07:55:36.876627 crypto-screening-2.3.0/crypto_screening/market/
--rw-rw-rw-   0        0        0     9635 2023-07-09 06:41:57.000000 crypto-screening-2.3.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-09 07:55:36.880637 crypto-screening-2.3.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.3.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.3.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.3.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.3.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-09 07:55:36.885636 crypto-screening-2.3.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.3.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.3.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.3.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.3.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.3.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.3.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.3.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.3.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.3.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-2.3.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-09 07:55:36.870670 crypto-screening-2.3.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-09 07:55:36.000000 crypto-screening-2.3.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2023-07-09 07:55:36.000000 crypto-screening-2.3.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 07:55:36.000000 crypto-screening-2.3.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-07-09 07:55:36.000000 crypto-screening-2.3.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-09 07:55:36.000000 crypto-screening-2.3.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-09 07:55:36.000000 crypto-screening-2.3.0/pyproject.toml
--rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.3.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 07:55:36.887611 crypto-screening-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-09 07:55:31.000000 crypto-screening-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 08:02:36.492624 crypto-screening-2.3.1/
+-rw-rw-rw-   0        0        0       98 2023-07-09 08:02:36.000000 crypto-screening-2.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-09 08:02:36.491623 crypto-screening-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.3.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.3.1/build.py
+drwxrwxrwx   0        0        0        0 2023-07-09 08:02:36.475646 crypto-screening-2.3.1/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-09 08:02:36.483624 crypto-screening-2.3.1/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.3.1/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-2.3.1/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    49517 2023-07-09 08:02:20.000000 crypto-screening-2.3.1/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    11824 2023-07-06 12:48:49.000000 crypto-screening-2.3.1/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.3.1/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-2.3.1/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.3.1/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.3.1/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-09 08:02:36.484623 crypto-screening-2.3.1/crypto_screening/market/
+-rw-rw-rw-   0        0        0     9635 2023-07-09 06:41:57.000000 crypto-screening-2.3.1/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-09 08:02:36.486623 crypto-screening-2.3.1/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.3.1/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.3.1/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.3.1/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.3.1/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-09 08:02:36.490624 crypto-screening-2.3.1/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.3.1/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.3.1/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.3.1/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.3.1/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.3.1/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.3.1/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.3.1/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.3.1/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.3.1/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-2.3.1/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-09 08:02:36.479624 crypto-screening-2.3.1/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-09 08:02:36.000000 crypto-screening-2.3.1/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-07-09 08:02:36.000000 crypto-screening-2.3.1/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 08:02:36.000000 crypto-screening-2.3.1/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-07-09 08:02:36.000000 crypto-screening-2.3.1/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-09 08:02:36.000000 crypto-screening-2.3.1/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-09 08:02:32.000000 crypto-screening-2.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.3.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.3.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 08:02:36.492624 crypto-screening-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-09 08:02:29.000000 crypto-screening-2.3.1/setup.py
```

### Comparing `crypto-screening-2.3.0/PKG-INFO` & `crypto-screening-2.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.3.0
+Version: 2.3.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.3.0/README.md` & `crypto-screening-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/build.py` & `crypto-screening-2.3.1/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/collect/assets.py` & `crypto-screening-2.3.1/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/collect/exchanges.py` & `crypto-screening-2.3.1/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/collect/market.py` & `crypto-screening-2.3.1/crypto_screening/collect/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -500,15 +500,15 @@
         The bids volume prices of the assets.
 
     - asks_volume:
         The asks volume prices of the assets.
 
     >>> from crypto_screening.collect.market import AssetsMarketState
     >>>
-    >>> state = assets_market_state(["BTC", "ETH", "LTC"], currency="USDT")
+    >>> state = assets_market_state(...)
     """
 
     bids: AssetsPrices
     asks: AssetsPrices
     bids_volume: AssetsPrices
     asks_volume: AssetsPrices
 
@@ -823,15 +823,16 @@
                 f"Consider using the 'adjust' parameter as {True}, "
                 f"to adjust to the actual length of the data."
             )
         # end try
     # end for
 
     return AssetsMarketState(
-        screeners=screeners, bids=bids, asks=asks
+        screeners=screeners, bids=bids, asks=asks,
+        bids_volume=bids_volume, asks_volume=asks_volume
     )
 # end assets_market_state
 
 SymbolsMarketData = Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]
 SymbolsMarketDatasets = Dict[str, Dict[str, pd.DataFrame]]
 
 @define(repr=False)
@@ -861,15 +862,15 @@
         The bids volume prices of the assets.
 
     - asks_volume:
         The asks volume prices of the assets.
 
     >>> from crypto_screening.collect.market import AssetsMarketState
     >>>
-    >>> state = assets_market_state(["BTC", "ETH", "LTC"], currency="USDT")
+    >>> state = assets_market_state(...)
     """
 
     bids: SymbolsPrices
     asks: SymbolsPrices
     bids_volume: SymbolsPrices
     asks_volume: SymbolsPrices
 
@@ -1118,15 +1119,16 @@
                 f"Consider using the 'adjust' parameter as {True}, "
                 f"to adjust to the actual length of the data."
             )
         # end try
     # end for
 
     return SymbolsMarketState(
-        screeners=screeners, bids=bids, asks=asks
+        screeners=screeners, bids=bids, asks=asks,
+        bids_volume=bids_volume, asks_volume=asks_volume
     )
 # end symbols_market_state
 
 def merge_symbols_market_states(*states: SymbolsMarketState) -> SymbolsMarketState:
     """
     Concatenates the states of the market.
```

### Comparing `crypto-screening-2.3.0/crypto_screening/collect/screeners.py` & `crypto-screening-2.3.1/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/collect/symbols.py` & `crypto-screening-2.3.1/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/dataset.py` & `crypto-screening-2.3.1/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/interval.py` & `crypto-screening-2.3.1/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/market/dynamic.py` & `crypto-screening-2.3.1/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/market/foundation/data.py` & `crypto-screening-2.3.1/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-2.3.1/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/market/foundation/state.py` & `crypto-screening-2.3.1/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-2.3.1/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/market/screeners/base.py` & `crypto-screening-2.3.1/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/market/screeners/container.py` & `crypto-screening-2.3.1/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-2.3.1/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-2.3.1/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-2.3.1/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/market/waiting.py` & `crypto-screening-2.3.1/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/process.py` & `crypto-screening-2.3.1/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/symbols.py` & `crypto-screening-2.3.1/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening/validate.py` & `crypto-screening-2.3.1/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-2.3.1/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.3.0
+Version: 2.3.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.3.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-2.3.1/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.0/pyproject.toml` & `crypto-screening-2.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '2.3.0'
+version = '2.3.1'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-2.3.0/setup.py` & `crypto-screening-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='2.3.0',
+        version='2.3.1',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

