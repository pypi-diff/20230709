# Comparing `tmp/crypto-screening-2.5.0.tar.gz` & `tmp/crypto-screening-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-2.5.0.tar", last modified: Sun Jul  9 10:53:36 2023, max compression
+gzip compressed data, was "crypto-screening-2.6.0.tar", last modified: Sun Jul  9 13:27:54 2023, max compression
```

## Comparing `crypto-screening-2.5.0.tar` & `crypto-screening-2.6.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 10:53:36.031875 crypto-screening-2.5.0/
--rw-rw-rw-   0        0        0       98 2023-07-09 10:53:35.000000 crypto-screening-2.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-09 10:53:36.031875 crypto-screening-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.5.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.5.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-09 10:53:36.010875 crypto-screening-2.5.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-09 10:53:36.022875 crypto-screening-2.5.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.5.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-2.5.0/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    54523 2023-07-09 10:53:20.000000 crypto-screening-2.5.0/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    11824 2023-07-06 12:48:49.000000 crypto-screening-2.5.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.5.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-2.5.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.5.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.5.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-09 10:53:36.024875 crypto-screening-2.5.0/crypto_screening/market/
--rw-rw-rw-   0        0        0     6010 2023-07-09 08:11:33.000000 crypto-screening-2.5.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-09 10:53:36.026875 crypto-screening-2.5.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.5.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.5.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.5.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.5.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-09 10:53:36.030874 crypto-screening-2.5.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.5.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.5.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.5.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.5.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.5.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.5.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.5.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.5.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.5.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-2.5.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-09 10:53:36.019876 crypto-screening-2.5.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-09 10:53:35.000000 crypto-screening-2.5.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2023-07-09 10:53:35.000000 crypto-screening-2.5.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 10:53:35.000000 crypto-screening-2.5.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-07-09 10:53:35.000000 crypto-screening-2.5.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-09 10:53:35.000000 crypto-screening-2.5.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-09 10:53:35.000000 crypto-screening-2.5.0/pyproject.toml
--rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.5.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.5.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 10:53:36.031875 crypto-screening-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-09 10:53:30.000000 crypto-screening-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:27:54.388899 crypto-screening-2.6.0/
+-rw-rw-rw-   0        0        0       98 2023-07-09 13:27:53.000000 crypto-screening-2.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-09 13:27:54.388389 crypto-screening-2.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.6.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.6.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:27:54.135507 crypto-screening-2.6.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-09 13:27:54.272233 crypto-screening-2.6.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.6.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4056 2023-06-27 13:26:48.000000 crypto-screening-2.6.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    49758 2023-07-09 13:27:34.000000 crypto-screening-2.6.0/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    11824 2023-07-06 12:48:49.000000 crypto-screening-2.6.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.6.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-2.6.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.6.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.6.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:27:54.282925 crypto-screening-2.6.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0     6010 2023-07-09 08:11:33.000000 crypto-screening-2.6.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:27:54.346905 crypto-screening-2.6.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.6.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.6.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.6.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.6.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:27:54.386819 crypto-screening-2.6.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.6.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.6.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.6.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.6.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.6.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.6.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.6.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.6.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.6.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3845 2023-06-27 09:22:00.000000 crypto-screening-2.6.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:27:54.245091 crypto-screening-2.6.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-09 13:27:54.000000 crypto-screening-2.6.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-07-09 13:27:54.000000 crypto-screening-2.6.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 13:27:54.000000 crypto-screening-2.6.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-07-09 13:27:54.000000 crypto-screening-2.6.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-09 13:27:54.000000 crypto-screening-2.6.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-09 13:27:53.000000 crypto-screening-2.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.6.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.6.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 13:27:54.388899 crypto-screening-2.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-09 13:27:48.000000 crypto-screening-2.6.0/setup.py
```

### Comparing `crypto-screening-2.5.0/PKG-INFO` & `crypto-screening-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.5.0
+Version: 2.6.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.5.0/README.md` & `crypto-screening-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/build.py` & `crypto-screening-2.6.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/collect/assets.py` & `crypto-screening-2.6.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/collect/exchanges.py` & `crypto-screening-2.6.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/collect/market.py` & `crypto-screening-2.6.0/crypto_screening/collect/market.py`

 * *Files 10% similar despite different names*

```diff
@@ -601,77 +601,64 @@
     def data(self) -> AssetsMarketData:
         """
         Returns the structured data of the state.
 
         :return: The data of the state.
         """
 
-        datasets: AssetsMarketData = {}
+        datasets: Dict[str, Dict[str, Dict[str, Dict[dt.datetime, Dict[str, float]]]]] = {}
 
-        for exchange, bases in self.bids.items():
-            for base, quotes in bases.items():
-                for quote, prices in quotes.items():
-                    for i, (time, price) in enumerate(prices):
-                        (
-                            datasets.
-                            setdefault(exchange, {}).
-                            setdefault(base, {}).
-                            setdefault(quote, [(time, {})])[i][-1]
-                        )[BIDS] = price
-                    # end for
+        for key, data in zip(
+            (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME),
+            (self.bids, self.asks, self.bids_volume, self.asks_volume)
+        ):
+            for exchange, bases in data.items():
+                for base, quotes in bases.items():
+                    for quote, prices in quotes.items():
+                        for i, (time, price) in enumerate(prices):
+                            try:
+                                if isinstance(time, str):
+                                    time = dt.datetime.fromisoformat(time)
+
+                                elif isinstance(time, int):
+                                    time = dt.datetime.fromtimestamp(time)
+
+                            except (Type, ValueError):
+                                pass
+                            # end try
+
+                            (
+                                datasets.
+                                setdefault(exchange, {}).
+                                setdefault(base, {}).
+                                setdefault(quote, {}).
+                                setdefault(time, {})
+                            )[key] = price
+                        # end for
                 # end for
             # end for
         # end for
 
-        for exchange, bases in self.asks.items():
-            for base, quotes in bases.items():
-                for quote, prices in quotes.items():
-                    for i, (time, price) in enumerate(prices):
-                        (
-                            datasets.
-                            setdefault(exchange, {}).
-                            setdefault(base, {}).
-                            setdefault(quote, [(time, {})])[i][-1]
-                        )[ASKS] = price
-                    # end for
-                # end for
-            # end for
-        # end for
-
-        for exchange, bases in self.bids_volume.items():
-            for base, quotes in bases.items():
-                for quote, prices in quotes.items():
-                    for i, (time, price) in enumerate(prices):
-                        (
-                            datasets.
-                            setdefault(exchange, {}).
-                            setdefault(base, {}).
-                            setdefault(quote, [(time, {})])[i][-1]
-                        )[BIDS_VOLUME] = price
-                    # end for
-                # end for
-            # end for
-        # end for
+        new_datasets: AssetsMarketData = {}
 
-        for exchange, bases in self.asks_volume.items():
+        for exchange, bases in datasets.items():
             for base, quotes in bases.items():
                 for quote, prices in quotes.items():
-                    for i, (time, price) in enumerate(prices):
-                        (
-                            datasets.
-                            setdefault(exchange, {}).
-                            setdefault(base, {}).
-                            setdefault(quote, [(time, {})])[i][-1]
-                        )[ASKS_VOLUME] = price
-                    # end for
+                    (
+                        new_datasets.
+                        setdefault(exchange, {}).
+                        setdefault(base, {})
+                    )[quote] = sorted(
+                        list(prices.items()), key=lambda pair: pair[0]
+                    )
                 # end for
             # end for
         # end for
 
-        return datasets
+        return new_datasets
     # end data
 
     def datasets(self) -> AssetsMarketDatasets:
         """
         Rebuilds the dataset from the market state.
 
         :return: The dataset of the state data.
@@ -754,85 +741,46 @@
         if adjust and (length is None):
             length = len(screener.market)
 
         elif adjust:
             length = min([len(screener.market), length])
         # end if
 
+        if length > len(screener.market):
+            raise ValueError(
+                f"Data of '{screener.exchange}' "
+                f"symbol in '{screener.symbol}' exchange "
+                f"is not long enough for the requested length: {length}. "
+                f"Consider using the 'adjust' parameter as {True}, "
+                f"to adjust to the actual length of the data."
+            )
+        # end if
+
         base, quote = symbol_to_parts(
             symbol=screener.symbol, separator=separator
         )
 
-        try:
-            (
-                bids.
-                setdefault(screener.exchange, {}).
-                setdefault(base, {}).
-                setdefault(
-                    quote,
-                    list(
-                        zip(
-                            list(screener.market.index),
-                            list(screener.market[BIDS][-length:])
-                        )
-                    )
-                )
-            )
-            (
-                asks.
-                setdefault(screener.exchange, {}).
-                setdefault(base, {}).
-                setdefault(
-                    quote,
-                    list(
-                        zip(
-                            list(screener.market.index),
-                            list(screener.market[ASKS][-length:])
-                        )
-                    )
-                )
-            )
-            (
-                bids_volume.
-                setdefault(screener.exchange, {}).
-                setdefault(base, {}).
-                setdefault(
-                    quote,
-                    list(
-                        zip(
-                            list(screener.market.index),
-                            list(screener.market[BIDS_VOLUME][-length:])
-                        )
-                    )
-                )
-            )
+        for key, data in zip(
+            (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME),
+            (bids, asks, bids_volume, asks_volume)
+        ):
             (
-                asks_volume.
+                data.
                 setdefault(screener.exchange, {}).
                 setdefault(base, {}).
                 setdefault(
                     quote,
                     list(
                         zip(
                             list(screener.market.index),
-                            list(screener.market[ASKS_VOLUME][-length:])
+                            list(screener.market[key][-length:])
                         )
                     )
                 )
             )
-
-        except IndexError:
-            raise ValueError(
-                f"Data of '{screener.exchange}' "
-                f"symbol in '{screener.symbol}' exchange "
-                f"is not long enough for the requested length: {length}. "
-                f"Consider using the 'adjust' parameter as {True}, "
-                f"to adjust to the actual length of the data."
-            )
-        # end try
     # end for
 
     return AssetsMarketState(
         screeners=screeners, bids=bids, asks=asks,
         bids_volume=bids_volume, asks_volume=asks_volume
     )
 # end assets_market_state
@@ -951,65 +899,56 @@
     def data(self) -> SymbolsMarketData:
         """
         Returns the structured data of the state.
 
         :return: The data of the state.
         """
 
-        datasets: SymbolsMarketData = {}
+        datasets: Dict[str, Dict[str, Dict[dt.datetime, Dict[str, float]]]] = {}
 
-        for exchange, symbols in self.bids.items():
-            for symbol, prices in symbols.items():
-                for i, (time, price) in enumerate(prices):
-                    (
-                        datasets.
-                        setdefault(exchange, {}).
-                        setdefault(symbol, [(time, {})])[i][-1]
-                    )[BIDS] = price
-                # end for
-            # end for
-        # end for
+        for key, data in zip(
+            (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME),
+            (self.bids, self.asks, self.bids_volume, self.asks_volume)
+        ):
+            for exchange, symbols in data.items():
+                for symbol, prices in symbols.items():
+                    for i, (time, price) in enumerate(prices):
+                        try:
+                            if isinstance(time, str):
+                                time = dt.datetime.fromisoformat(time)
+
+                            elif isinstance(time, int):
+                                time = dt.datetime.fromtimestamp(time)
+
+                        except (Type, ValueError):
+                            pass
+                        # end try
 
-        for exchange, symbols in self.asks.items():
-            for symbol, prices in symbols.items():
-                for i, (time, price) in enumerate(prices):
-                    (
-                        datasets.
-                        setdefault(exchange, {}).
-                        setdefault(symbol, [(time, {})])[i][-1]
-                    )[ASKS] = price
+                        (
+                            datasets.
+                            setdefault(exchange, {}).
+                            setdefault(symbol, {}).
+                            setdefault(time, {})
+                        )[key] = price
+                    # end for
                 # end for
             # end for
         # end for
 
-        for exchange, symbols in self.bids_volume.items():
-            for symbol, prices in symbols.items():
-                for i, (time, price) in enumerate(prices):
-                    (
-                        datasets.
-                        setdefault(exchange, {}).
-                        setdefault(symbol, [(time, {})])[i][-1]
-                    )[BIDS_VOLUME] = price
-                # end for
-            # end for
-        # end for
+        new_datasets: SymbolsMarketData = {}
 
-        for exchange, symbols in self.asks_volume.items():
-            for symbol, prices in symbols.items():
-                for i, (time, price) in enumerate(prices):
-                    (
-                        datasets.
-                        setdefault(exchange, {}).
-                        setdefault(symbol, [(time, {})])[i][-1]
-                    )[ASKS_VOLUME] = price
-                # end for
+        for exchange, symbols in datasets.items():
+            for symbol, prices in symbols.copy().items():
+                new_datasets.setdefault(exchange, {})[symbol] = sorted(
+                    list(prices.items()), key=lambda pair: pair[0]
+                )
             # end for
         # end for
 
-        return datasets
+        return new_datasets
     # end data
 
     def datasets(self) -> SymbolsMarketDatasets:
         """
         Rebuilds the dataset from the market state.
 
         :return: The dataset of the state data.
@@ -1059,76 +998,41 @@
         if adjust and (length is None):
             length = len(screener.market)
 
         elif adjust:
             length = min([len(screener.market), length])
         # end if
 
-        try:
-            (
-                bids.
-                setdefault(screener.exchange, {}).
-                setdefault(
-                    screener.symbol,
-                    list(
-                        zip(
-                            list(screener.market.index),
-                            list(screener.market[BIDS][-length:])
-                        )
-                    )
-                )
-            )
-            (
-                asks.
-                setdefault(screener.exchange, {}).
-                setdefault(
-                    screener.symbol,
-                    list(
-                        zip(
-                            list(screener.market.index),
-                            list(screener.market[ASKS][-length:])
-                        )
-                    )
-                )
-            )
-            (
-                bids_volume.
-                setdefault(screener.exchange, {}).
-                setdefault(
-                    screener.symbol,
-                    list(
-                        zip(
-                            list(screener.market.index),
-                            list(screener.market[BIDS_VOLUME][-length:])
-                        )
-                    )
-                )
+        if length > len(screener.market):
+            raise ValueError(
+                f"Data of '{screener.exchange}' symbol in '{screener.symbol}' exchange "
+                f"is not long enough for the requested length: {length}. "
+                f"Consider using the 'adjust' parameter as {True}, "
+                f"to adjust to the actual length of the data."
             )
+        # end if
+
+        for key, data in zip(
+            (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME),
+            (bids, asks, bids_volume, asks_volume)
+        ):
             (
-                asks_volume.
+                data.
                 setdefault(screener.exchange, {}).
                 setdefault(
                     screener.symbol,
                     list(
                         zip(
                             list(screener.market.index),
-                            list(screener.market[ASKS_VOLUME][-length:])
+                            list(screener.market[key][-length:])
                         )
                     )
                 )
             )
-
-        except IndexError:
-            raise ValueError(
-                f"Data of '{screener.exchange}' symbol in '{screener.symbol}' exchange "
-                f"is not long enough for the requested length: {length}. "
-                f"Consider using the 'adjust' parameter as {True}, "
-                f"to adjust to the actual length of the data."
-            )
-        # end try
+        # end for
     # end for
 
     return SymbolsMarketState(
         screeners=screeners, bids=bids, asks=asks,
         bids_volume=bids_volume, asks_volume=asks_volume
     )
 # end symbols_market_state
@@ -1147,51 +1051,31 @@
 
     bids: SymbolsPrices = {}
     asks: SymbolsPrices = {}
     bids_volume: SymbolsPrices = {}
     asks_volume: SymbolsPrices = {}
 
     for state in states:
-        for exchange, symbols in state.asks.items():
-            for symbol, prices in symbols.items():
-                (
-                    asks.setdefault(exchange, {}).
-                    setdefault(symbol, []).
-                    extend(prices)
-                )
-            # end for
-        # end for
-
-        for exchange, symbols in state.bids.items():
-            for symbol, prices in symbols.items():
-                (
-                    bids.setdefault(exchange, {}).
-                    setdefault(symbol, []).
-                    extend(prices)
-                )
-            # end for
-        # end for
-
-        for exchange, symbols in state.asks_volume.items():
-            for symbol, prices in symbols.items():
-                (
-                    asks_volume.setdefault(exchange, {}).
-                    setdefault(symbol, []).
-                    extend(prices)
-                )
-            # end for
-        # end for
-
-        for exchange, symbols in state.bids_volume.items():
-            for symbol, prices in symbols.items():
-                (
-                    bids_volume.setdefault(exchange, {}).
-                    setdefault(symbol, []).
-                    extend(prices)
-                )
+        for key, (state_data, data) in zip(
+            (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME),
+            (
+                (state.bids, bids),
+                (state.asks, asks),
+                (state.bids_volume, bids_volume),
+                (state.asks_volume, asks_volume)
+            )
+        ):
+            for exchange, symbols in state_data.items():
+                for symbol, prices in symbols.items():
+                    (
+                        data.setdefault(exchange, {}).
+                        setdefault(symbol, []).
+                        extend(prices)
+                    )
+                # end for
             # end for
         # end for
     # end for
 
     screeners = []
 
     if sort:
@@ -1228,59 +1112,33 @@
 
     bids: AssetsPrices = {}
     asks: AssetsPrices = {}
     bids_volume: AssetsPrices = {}
     asks_volume: AssetsPrices = {}
 
     for state in states:
-        for exchange, symbols in state.bids.items():
-            for base, quotes in symbols.items():
-                for quote, prices in quotes.items():
-                    (
-                        bids.setdefault(exchange, {}).
-                        setdefault(base, {}).
-                        setdefault(quote, []).
-                        extend(prices)
-                    )
-            # end for
-        # end for
-
-        for exchange, symbols in state.asks.items():
-            for base, quotes in symbols.items():
-                for quote, prices in quotes.items():
-                    (
-                        asks.setdefault(exchange, {}).
-                        setdefault(base, {}).
-                        setdefault(quote, []).
-                        extend(prices)
-                    )
-            # end for
-        # end for
-
-        for exchange, symbols in state.bids_volume.items():
-            for base, quotes in symbols.items():
-                for quote, prices in quotes.items():
-                    (
-                        bids_volume.setdefault(exchange, {}).
-                        setdefault(base, {}).
-                        setdefault(quote, []).
-                        extend(prices)
-                    )
-            # end for
-        # end for
-
-        for exchange, symbols in state.asks_volume.items():
-            for base, quotes in symbols.items():
-                for quote, prices in quotes.items():
-                    (
-                        asks_volume.setdefault(exchange, {}).
-                        setdefault(base, {}).
-                        setdefault(quote, []).
-                        extend(prices)
-                    )
+        for key, (state_data, data) in zip(
+            (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME),
+            (
+                (state.bids, bids),
+                (state.asks, asks),
+                (state.bids_volume, bids_volume),
+                (state.asks_volume, asks_volume)
+            )
+        ):
+            for exchange, symbols in state_data.items():
+                for base, quotes in symbols.items():
+                    for quote, prices in quotes.items():
+                        (
+                            data.setdefault(exchange, {}).
+                            setdefault(base, {}).
+                            setdefault(quote, []).
+                            extend(prices)
+                        )
+                # end for
             # end for
         # end for
     # end for
 
     if sort:
         for prices_data in (bids, asks, bids_volume, asks_volume):
             for exchange, bases in prices_data.items():
```

### Comparing `crypto-screening-2.5.0/crypto_screening/collect/screeners.py` & `crypto-screening-2.6.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/collect/symbols.py` & `crypto-screening-2.6.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/dataset.py` & `crypto-screening-2.6.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/interval.py` & `crypto-screening-2.6.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/market/dynamic.py` & `crypto-screening-2.6.0/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/market/foundation/data.py` & `crypto-screening-2.6.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-2.6.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/market/foundation/state.py` & `crypto-screening-2.6.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-2.6.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/market/screeners/base.py` & `crypto-screening-2.6.0/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/market/screeners/container.py` & `crypto-screening-2.6.0/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-2.6.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-2.6.0/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-2.6.0/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/market/waiting.py` & `crypto-screening-2.6.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/process.py` & `crypto-screening-2.6.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/symbols.py` & `crypto-screening-2.6.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening/validate.py` & `crypto-screening-2.6.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-2.6.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.5.0
+Version: 2.6.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.5.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-2.6.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.5.0/pyproject.toml` & `crypto-screening-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '2.5.0'
+version = '2.6.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-2.5.0/setup.py` & `crypto-screening-2.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='2.5.0',
+        version='2.6.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

