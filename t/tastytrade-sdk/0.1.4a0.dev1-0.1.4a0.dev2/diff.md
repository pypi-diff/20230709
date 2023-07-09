# Comparing `tmp/tastytrade_sdk-0.1.4a0.dev1.tar.gz` & `tmp/tastytrade_sdk-0.1.4a0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade_sdk-0.1.4a0.dev1.tar", max compression
+gzip compressed data, was "tastytrade_sdk-0.1.4a0.dev2.tar", max compression
```

## Comparing `tastytrade_sdk-0.1.4a0.dev1.tar` & `tastytrade_sdk-0.1.4a0.dev2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1053 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/LICENSE
--rw-r--r--   0        0        0     1652 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/docs/users/README.md
--rw-r--r--   0        0        0      822 2023-07-09 18:50:24.100857 tastytrade_sdk-0.1.4a0.dev1/pyproject.toml
--rw-r--r--   0        0        0      516 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/__init__.py
--rw-r--r--   0        0        0     2018 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/account.py
--rw-r--r--   0        0        0     4185 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/api.py
--rw-r--r--   0        0        0      136 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/config.py
--rw-r--r--   0        0        0      421 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/__init__.py
--rw-r--r--   0        0        0     1548 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/market_data.py
--rw-r--r--   0        0        0     2646 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/models.py
--rw-r--r--   0        0        0     1889 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/streamer_symbol_translation.py
--rw-r--r--   0        0        0     6137 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/subscription.py
--rw-r--r--   0        0        0     1414 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/tastytrade.py
--rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 tastytrade_sdk-0.1.4a0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-07-09 19:21:03.853323 tastytrade_sdk-0.1.4a0.dev2/LICENSE
+-rw-r--r--   0        0        0     1652 2023-07-09 19:21:03.853323 tastytrade_sdk-0.1.4a0.dev2/docs/users/README.md
+-rw-r--r--   0        0        0      822 2023-07-09 19:21:38.612943 tastytrade_sdk-0.1.4a0.dev2/pyproject.toml
+-rw-r--r--   0        0        0      516 2023-07-09 19:21:03.857323 tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/__init__.py
+-rw-r--r--   0        0        0     2624 2023-07-09 19:21:03.857323 tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/account.py
+-rw-r--r--   0        0        0     4185 2023-07-09 19:21:03.857323 tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/api.py
+-rw-r--r--   0        0        0      136 2023-07-09 19:21:03.857323 tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/config.py
+-rw-r--r--   0        0        0      421 2023-07-09 19:21:03.857323 tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-09 19:21:03.857323 tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/market_data/__init__.py
+-rw-r--r--   0        0        0     1548 2023-07-09 19:21:03.857323 tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/market_data/market_data.py
+-rw-r--r--   0        0        0     2646 2023-07-09 19:21:03.857323 tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/market_data/models.py
+-rw-r--r--   0        0        0     1889 2023-07-09 19:21:03.857323 tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/market_data/streamer_symbol_translation.py
+-rw-r--r--   0        0        0     6137 2023-07-09 19:21:03.857323 tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/market_data/subscription.py
+-rw-r--r--   0        0        0     1125 2023-07-09 19:21:03.857323 tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/orders.py
+-rw-r--r--   0        0        0     1496 2023-07-09 19:21:03.857323 tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/tastytrade.py
+-rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 tastytrade_sdk-0.1.4a0.dev2/PKG-INFO
```

### Comparing `tastytrade_sdk-0.1.4a0.dev1/LICENSE` & `tastytrade_sdk-0.1.4a0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev1/docs/users/README.md` & `tastytrade_sdk-0.1.4a0.dev2/docs/users/README.md`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev1/pyproject.toml` & `tastytrade_sdk-0.1.4a0.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tastytrade-sdk"
-version = "0.1.4a0dev1"
+version = "0.1.4a0dev2"
 description = "A python wrapper around the tastytrade open API"
 authors = [
     "Aaron Mamparo <aaronmamparo@gmail.com>"
 ]
 license = "MIT"
 readme = "docs/users/README.md"
 packages = [
```

### Comparing `tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/__init__.py` & `tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/account.py` & `tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/account.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,66 @@
-from typing import List, Optional
+from dataclasses import dataclass
+from typing import List, Optional, Tuple, Any
 
 from tastytrade_sdk import Api
+from tastytrade_sdk.orders import Orders, Order
+
+
+@dataclass
+class PositionsParams:
+    underlying_symbols: Optional[List[str]] = None
+    symbol: Optional[str] = None
+    instrument_type: Optional[str] = None
+    include_closed_positions: Optional[bool] = None
+    underlying_product_code: Optional[str] = None
+    partition_keys: Optional[List[str]] = None
+    net_positions: Optional[bool] = None
+    include_marks: Optional[bool] = None
+
+    def to_params(self) -> List[Tuple[str, Any]]:
+        params = []
+        if self.underlying_symbols:
+            params.extend([('underlying-symbols[]', x) for x in self.underlying_symbols])
+        if self.symbol:
+            params.append(('symbol', self.symbol))
+        if self.instrument_type:
+            params.append(('instrument-type', self.instrument_type))
+        if self.include_closed_positions is not None:
+            params.append(('include-closed-positions', self.include_closed_positions))
+        if self.underlying_product_code:
+            params.append(('underlying-product-code', self.underlying_product_code))
+        if self.partition_keys:
+            params.extend([('partition-keys[]', x) for x in self.partition_keys])
+        if self.net_positions is not None:
+            params.append(('net-positions', self.net_positions))
+        if self.include_marks:
+            params.append(('include-marks', self.include_marks))
+        return params
 
 
 class Account:
-    def __init__(self, account_number: str, api: Api):
+    def __init__(self, account_number: str, api: Api, orders: Orders):
         self.__account_number = account_number
         self.__api = api
+        self.__orders = orders
 
     @property
     def balances(self) -> dict:
         """
         https://developer.tastytrade.com/open-api-spec/balances-and-positions/#/accounts/getAccountsAccountNumberBalances
         """
         return self.__api.get(f'/accounts/{self.__account_number}/balances')['data']
 
-    def get_positions(self, underlying_symbols: Optional[List[str]] = None, symbol: Optional[str] = None,
-                      instrument_type: Optional[str] = None, include_closed_positions: Optional[bool] = None,
-                      underlying_product_code: Optional[str] = None, partition_keys: Optional[List[str]] = None,
-                      net_positions: Optional[bool] = None, include_marks: Optional[bool] = None) -> List[dict]:
+    def get_positions(self, params: PositionsParams) -> List[dict]:
         """
         https://developer.tastytrade.com/open-api-spec/balances-and-positions/#/positions/getAccountsAccountNumberPositions
         """
-        params = []
-        if underlying_symbols:
-            params.extend([('underlying-symbols[]', x) for x in underlying_symbols])
-        if symbol:
-            params.append(('symbol', symbol))
-        if instrument_type:
-            params.append(('instrument-type', instrument_type))
-        if include_closed_positions is not None:
-            params.append(('include-closed-positions', include_closed_positions))
-        if underlying_product_code:
-            params.append(('underlying-product-code', underlying_product_code))
-        if partition_keys:
-            params.extend([('partition-keys[]', x) for x in partition_keys])
-        if net_positions is not None:
-            params.append(('net-positions', net_positions))
-        if include_marks:
-            params.append(('include-marks', include_marks))
+        return self.__api.get(
+            f'/accounts/{self.__account_number}/positions',
+            params=params.to_params()
+        )['data']['items']
 
-        return self.__api.get(f'/accounts/{self.__account_number}/positions', params=params)['data']['items']
+    def place_order(self, order: Order) -> dict:
+        """
+        https://developer.tastytrade.com/open-api-spec/orders/#/orders/postAccountsAccountNumberOrders
+        """
+        return self.__orders.place_order(self.__account_number, order)
```

### Comparing `tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/api.py` & `tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/api.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/market_data.py` & `tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/market_data/market_data.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/models.py` & `tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/market_data/models.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/streamer_symbol_translation.py` & `tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/market_data/streamer_symbol_translation.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/subscription.py` & `tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/market_data/subscription.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/tastytrade.py` & `tastytrade_sdk-0.1.4a0.dev2/src/tastytrade_sdk/tastytrade.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from injector import Injector
 
 from tastytrade_sdk.account import Account
 from tastytrade_sdk.config import Config
 from tastytrade_sdk.api import Api, RequestsSession
 from tastytrade_sdk.market_data.market_data import MarketData
+from tastytrade_sdk.orders import Orders
 
 
 class Tastytrade:
     """
     The SDK's top-level class
     """
 
@@ -32,15 +33,15 @@
     def logout(self) -> None:
         """
         End the session
         """
         self.api.delete('/sessions')
 
     def account(self, account_number: str) -> Account:
-        return Account(account_number, self.api)
+        return Account(account_number, api=self.api, orders=self.__container.get(Orders))
 
     @property
     def market_data(self) -> MarketData:
         """
         Access the MarketData submodule
         """
         return self.__container.get(MarketData)
```

### Comparing `tastytrade_sdk-0.1.4a0.dev1/PKG-INFO` & `tastytrade_sdk-0.1.4a0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-sdk
-Version: 0.1.4a0.dev1
+Version: 0.1.4a0.dev2
 Summary: A python wrapper around the tastytrade open API
 License: MIT
 Author: Aaron Mamparo
 Author-email: aaronmamparo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

