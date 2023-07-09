# Comparing `tmp/crypto-screening-2.3.2.tar.gz` & `tmp/crypto-screening-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-2.3.2.tar", last modified: Sun Jul  9 08:11:43 2023, max compression
+gzip compressed data, was "crypto-screening-2.4.0.tar", last modified: Sun Jul  9 10:43:02 2023, max compression
```

## Comparing `crypto-screening-2.3.2.tar` & `crypto-screening-2.4.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 08:11:43.474995 crypto-screening-2.3.2/
--rw-rw-rw-   0        0        0       98 2023-07-09 08:11:43.000000 crypto-screening-2.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-09 08:11:43.474995 crypto-screening-2.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.3.2/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.3.2/build.py
-drwxrwxrwx   0        0        0        0 2023-07-09 08:11:43.453465 crypto-screening-2.3.2/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-09 08:11:43.465996 crypto-screening-2.3.2/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.3.2/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-2.3.2/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    49517 2023-07-09 08:02:20.000000 crypto-screening-2.3.2/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    11824 2023-07-06 12:48:49.000000 crypto-screening-2.3.2/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.3.2/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-2.3.2/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.3.2/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.3.2/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-09 08:11:43.466997 crypto-screening-2.3.2/crypto_screening/market/
--rw-rw-rw-   0        0        0     6010 2023-07-09 08:11:33.000000 crypto-screening-2.3.2/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-09 08:11:43.469997 crypto-screening-2.3.2/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.3.2/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.3.2/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.3.2/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.3.2/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-09 08:11:43.473997 crypto-screening-2.3.2/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.3.2/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.3.2/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.3.2/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.3.2/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.3.2/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.3.2/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.3.2/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.3.2/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.3.2/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-2.3.2/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-09 08:11:43.461995 crypto-screening-2.3.2/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-09 08:11:43.000000 crypto-screening-2.3.2/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2023-07-09 08:11:43.000000 crypto-screening-2.3.2/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 08:11:43.000000 crypto-screening-2.3.2/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-07-09 08:11:43.000000 crypto-screening-2.3.2/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-09 08:11:43.000000 crypto-screening-2.3.2/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-09 08:11:43.000000 crypto-screening-2.3.2/pyproject.toml
--rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.3.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.3.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 08:11:43.474995 crypto-screening-2.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-09 08:10:51.000000 crypto-screening-2.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 10:43:02.241171 crypto-screening-2.4.0/
+-rw-rw-rw-   0        0        0       98 2023-07-09 10:43:01.000000 crypto-screening-2.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-09 10:43:02.240170 crypto-screening-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.4.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.4.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-09 10:43:02.208883 crypto-screening-2.4.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-09 10:43:02.231170 crypto-screening-2.4.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.4.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-2.4.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    53434 2023-07-09 10:42:48.000000 crypto-screening-2.4.0/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    11824 2023-07-06 12:48:49.000000 crypto-screening-2.4.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.4.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-2.4.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.4.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.4.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-09 10:43:02.232185 crypto-screening-2.4.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0     6010 2023-07-09 08:11:33.000000 crypto-screening-2.4.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-09 10:43:02.235170 crypto-screening-2.4.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.4.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.4.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.4.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.4.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-09 10:43:02.240170 crypto-screening-2.4.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.4.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.4.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.4.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.4.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.4.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.4.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.4.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.4.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.4.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-2.4.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-09 10:43:02.226199 crypto-screening-2.4.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-09 10:43:02.000000 crypto-screening-2.4.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-07-09 10:43:02.000000 crypto-screening-2.4.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 10:43:02.000000 crypto-screening-2.4.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-07-09 10:43:02.000000 crypto-screening-2.4.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-09 10:43:02.000000 crypto-screening-2.4.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-09 10:43:01.000000 crypto-screening-2.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.4.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 10:43:02.241171 crypto-screening-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-09 10:42:57.000000 crypto-screening-2.4.0/setup.py
```

### Comparing `crypto-screening-2.3.2/PKG-INFO` & `crypto-screening-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.3.2
+Version: 2.4.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.3.2/README.md` & `crypto-screening-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/build.py` & `crypto-screening-2.4.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/collect/assets.py` & `crypto-screening-2.4.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/collect/exchanges.py` & `crypto-screening-2.4.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/collect/market.py` & `crypto-screening-2.4.0/crypto_screening/collect/market.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import numpy as np
 import pandas as pd
 
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.orderbook import OrderbookScreener
 from crypto_screening.dataset import BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME
 from crypto_screening.symbols import symbol_to_parts, parts_to_symbol
+from crypto_screening.collect.screeners import find_screeners
 from crypto_screening.market.screeners.orderbook import create_orderbook_dataframe
 
 __all__ = [
     "validate_assets_market_state_prices_symbol",
     "assets_market_price",
     "is_symbol_in_assets_market_prices",
     "symbols_market_prices",
@@ -41,15 +42,19 @@
     "assets_market_state_to_symbols_market_state",
     "assets_market_prices_to_symbol_market_prices",
     "assets_market_dataset_to_symbols_market_datasets",
     "symbols_market_dataset_to_assets_market_datasets",
     "symbols_screeners",
     "symbols_market_datasets_to_symbols_screeners",
     "assets_screeners",
-    "assets_market_datasets_to_assets_screeners"
+    "assets_market_datasets_to_assets_screeners",
+    "assets_market_data_to_symbols_market_data",
+    "add_symbols_data_to_screeners",
+    "add_assets_data_to_screeners",
+    "symbols_market_data_to_assets_market_data"
 ]
 
 AssetsPrices = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]]
 SymbolsPrices = Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]
 
 def is_exchange_in_market_prices(
         exchange: str,
@@ -1447,14 +1452,77 @@
         ),
         asks_volume=symbol_market_prices_to_assets_market_prices(
             state.asks_volume, separator=separator
         )
     )
 # end symbols_market_state_to_assets_market_state
 
+def assets_market_data_to_symbols_market_data(
+        data: AssetsMarketData,
+        separator: Optional[str] = None
+) -> SymbolsMarketData:
+    """
+    Converts the structure of the market data from assets to symbols.
+
+    :param data: The data to convert.
+    :param separator: The separator for the symbols.
+
+    :return: The data in the new structure
+    """
+
+    symbols_data: SymbolsMarketData = {}
+
+    for exchange, bases in data.items():
+        for base, quotes in bases.items():
+            for quote, data in quotes.items():
+                symbol = parts_to_symbol(base, quote, separator=separator)
+
+                (
+                    symbols_data.
+                    setdefault(exchange, {}).
+                    setdefault(symbol, data)
+                )
+            # end for
+    # end for
+
+    return symbols_data
+# end assets_market_data_to_symbols_market_data
+
+def symbols_market_data_to_assets_market_data(
+        data: SymbolsMarketData,
+        separator: Optional[str] = None
+) -> AssetsMarketData:
+    """
+    Converts the structure of the market data from assets to symbols.
+
+    :param data: The data to convert.
+    :param separator: The separator for the symbols.
+
+    :return: The data in the new structure
+    """
+
+    assets_data: AssetsMarketData = {}
+
+    for exchange, symbols in data.items():
+        for symbol, data in symbols.items():
+            base, quote = symbol_to_parts(symbol, separator=separator)
+
+            (
+                assets_data.
+                setdefault(exchange, {}).
+                setdefault(base, {}).
+                setdefault(quote, data)
+            )
+            # end for
+        # end for
+    # end for
+
+    return assets_data
+# end assets_market_data_to_symbols_market_data
+
 _ST = TypeVar("_ST", Type[BaseScreener], Type[OrderbookScreener])
 
 AssetsScreeners = Dict[str, Dict[str, Dict[str, Union[BaseScreener, _ST]]]]
 
 def assets_market_datasets_to_assets_screeners(
         datasets: AssetsMarketDatasets,
         base: Optional[_ST] = None,
@@ -1597,8 +1665,64 @@
     for exchange, symbols in screeners.items():
         for symbol, screener in symbols.items():
             screeners_collection.append(screener)
         # end for
     # end for
 
     return screeners_collection
-# end symbols_screeners
+# end symbols_screeners
+
+def add_symbols_data_to_screeners(
+        screeners: Iterable[BaseScreener],
+        data: SymbolsMarketData,
+        adjust: Optional[bool] = True
+) -> None:
+    """
+    Updates the data of the screeners with the symbols data.
+
+    :param screeners: The screeners to update.
+    :param data: The new data to add to the screeners.
+    :param adjust: The value to adjust with screeners that are not found.
+    """
+
+    for exchange, symbols in data.items():
+        for symbol, rows in symbols.items():
+            found_screeners = find_screeners(
+                screeners, exchange=exchange, symbol=symbol
+            )
+
+            if not found_screeners and not adjust:
+                raise ValueError(
+                    f"Unable to find a screener with exchange "
+                    f"'{exchange}' and symbol '{symbol}' to update its data. "
+                    f"Consider setting the 'adjust' parameter to True, ignore."
+                )
+            # end if
+
+            screener = found_screeners[0]
+
+            for time, row in rows:
+                screener.market.loc[time] = row
+            # end for
+        # end for
+    # end for
+# end add_symbols_data_to_screeners
+
+def add_assets_data_to_screeners(
+        screeners: Iterable[BaseScreener],
+        data: AssetsMarketData,
+        adjust: Optional[bool] = True
+) -> None:
+    """
+    Updates the data of the screeners with the symbols data.
+
+    :param screeners: The screeners to update.
+    :param data: The new data to add to the screeners.
+    :param adjust: The value to adjust with screeners that are not found.
+    """
+
+    return add_symbols_data_to_screeners(
+        screeners=screeners,
+        data=assets_market_data_to_symbols_market_data(data=data),
+        adjust=adjust
+    )
+# end add_assets_data_to_screeners
```

### Comparing `crypto-screening-2.3.2/crypto_screening/collect/screeners.py` & `crypto-screening-2.4.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/collect/symbols.py` & `crypto-screening-2.4.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/dataset.py` & `crypto-screening-2.4.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/interval.py` & `crypto-screening-2.4.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/market/dynamic.py` & `crypto-screening-2.4.0/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/market/foundation/data.py` & `crypto-screening-2.4.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/market/foundation/protocols.py` & `crypto-screening-2.4.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/market/foundation/state.py` & `crypto-screening-2.4.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/market/foundation/waiting.py` & `crypto-screening-2.4.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/market/screeners/base.py` & `crypto-screening-2.4.0/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/market/screeners/container.py` & `crypto-screening-2.4.0/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-2.4.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-2.4.0/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/market/screeners/recorder.py` & `crypto-screening-2.4.0/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/market/waiting.py` & `crypto-screening-2.4.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/process.py` & `crypto-screening-2.4.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/symbols.py` & `crypto-screening-2.4.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening/validate.py` & `crypto-screening-2.4.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-2.4.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.3.2
+Version: 2.4.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.3.2/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-2.4.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.3.2/pyproject.toml` & `crypto-screening-2.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '2.3.2'
+version = '2.4.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-2.3.2/setup.py` & `crypto-screening-2.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='2.3.2',
+        version='2.4.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

