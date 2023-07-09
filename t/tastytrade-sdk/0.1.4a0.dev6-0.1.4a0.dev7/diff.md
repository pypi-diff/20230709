# Comparing `tmp/tastytrade_sdk-0.1.4a0.dev6.tar.gz` & `tmp/tastytrade_sdk-0.1.4a0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade_sdk-0.1.4a0.dev6.tar", max compression
+gzip compressed data, was "tastytrade_sdk-0.1.4a0.dev7.tar", max compression
```

## Comparing `tastytrade_sdk-0.1.4a0.dev6.tar` & `tastytrade_sdk-0.1.4a0.dev7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1053 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/LICENSE
--rw-r--r--   0        0        0     1652 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/docs/users/README.md
--rw-r--r--   0        0        0      822 2023-07-09 19:38:28.310251 tastytrade_sdk-0.1.4a0.dev6/pyproject.toml
--rw-r--r--   0        0        0      614 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/__init__.py
--rw-r--r--   0        0        0     2675 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/account.py
--rw-r--r--   0        0        0     4185 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/api.py
--rw-r--r--   0        0        0      136 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/config.py
--rw-r--r--   0        0        0      421 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/__init__.py
--rw-r--r--   0        0        0     1548 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/market_data.py
--rw-r--r--   0        0        0     2646 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/models.py
--rw-r--r--   0        0        0     1889 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/streamer_symbol_translation.py
--rw-r--r--   0        0        0     6137 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/subscription.py
--rw-r--r--   0        0        0        0 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/orders/__init__.py
--rw-r--r--   0        0        0      731 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/orders/models.py
--rw-r--r--   0        0        0      482 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/orders/orders.py
--rw-r--r--   0        0        0     1503 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/tastytrade.py
--rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 tastytrade_sdk-0.1.4a0.dev6/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-07-09 19:48:26.642971 tastytrade_sdk-0.1.4a0.dev7/LICENSE
+-rw-r--r--   0        0        0     1652 2023-07-09 19:48:26.642971 tastytrade_sdk-0.1.4a0.dev7/docs/users/README.md
+-rw-r--r--   0        0        0      822 2023-07-09 19:48:57.379416 tastytrade_sdk-0.1.4a0.dev7/pyproject.toml
+-rw-r--r--   0        0        0      688 2023-07-09 19:48:26.642971 tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/__init__.py
+-rw-r--r--   0        0        0     2694 2023-07-09 19:48:26.642971 tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/account.py
+-rw-r--r--   0        0        0     4185 2023-07-09 19:48:26.642971 tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/api.py
+-rw-r--r--   0        0        0      136 2023-07-09 19:48:26.642971 tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/config.py
+-rw-r--r--   0        0        0      421 2023-07-09 19:48:26.642971 tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-09 19:48:26.642971 tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/market_data/__init__.py
+-rw-r--r--   0        0        0     1548 2023-07-09 19:48:26.642971 tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/market_data/market_data.py
+-rw-r--r--   0        0        0     2646 2023-07-09 19:48:26.646972 tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/market_data/models.py
+-rw-r--r--   0        0        0     1889 2023-07-09 19:48:26.646972 tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/market_data/streamer_symbol_translation.py
+-rw-r--r--   0        0        0     6137 2023-07-09 19:48:26.646972 tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/market_data/subscription.py
+-rw-r--r--   0        0        0        0 2023-07-09 19:48:26.646972 tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/orders/__init__.py
+-rw-r--r--   0        0        0      731 2023-07-09 19:48:26.646972 tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/orders/models.py
+-rw-r--r--   0        0        0      482 2023-07-09 19:48:26.646972 tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/orders/orders.py
+-rw-r--r--   0        0        0     1526 2023-07-09 19:48:26.646972 tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/tastytrade.py
+-rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 tastytrade_sdk-0.1.4a0.dev7/PKG-INFO
```

### Comparing `tastytrade_sdk-0.1.4a0.dev6/LICENSE` & `tastytrade_sdk-0.1.4a0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev6/docs/users/README.md` & `tastytrade_sdk-0.1.4a0.dev7/docs/users/README.md`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev6/pyproject.toml` & `tastytrade_sdk-0.1.4a0.dev7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tastytrade-sdk"
-version = "0.1.4a0dev6"
+version = "0.1.4a0dev7"
 description = "A python wrapper around the tastytrade open API"
 authors = [
     "Aaron Mamparo <aaronmamparo@gmail.com>"
 ]
 license = "MIT"
 readme = "docs/users/README.md"
 packages = [
```

### Comparing `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/account.py` & `tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from tastytrade_sdk.api import Api
 from tastytrade_sdk.orders.orders import Orders
 from tastytrade_sdk.orders.models import Order
 
 
 @dataclass
 class PositionsParams:
+    """@private"""
     underlying_symbols: Optional[List[str]] = None
     symbol: Optional[str] = None
     instrument_type: Optional[str] = None
     include_closed_positions: Optional[bool] = None
     underlying_product_code: Optional[str] = None
     partition_keys: Optional[List[str]] = None
     net_positions: Optional[bool] = None
```

### Comparing `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/api.py` & `tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/api.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/market_data.py` & `tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/market_data/market_data.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/models.py` & `tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/market_data/models.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/streamer_symbol_translation.py` & `tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/market_data/streamer_symbol_translation.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/subscription.py` & `tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/market_data/subscription.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/orders/models.py` & `tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/orders/models.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/tastytrade.py` & `tastytrade_sdk-0.1.4a0.dev7/src/tastytrade_sdk/tastytrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     def logout(self) -> None:
         """
         End the session
         """
         self.api.delete('/sessions')
 
     def account(self, account_number: str) -> Account:
+        """@private"""
         return Account(account_number, api=self.api, orders=self.__container.get(Orders))
 
     @property
     def market_data(self) -> MarketData:
         """
         Access the MarketData submodule
         """
```

### Comparing `tastytrade_sdk-0.1.4a0.dev6/PKG-INFO` & `tastytrade_sdk-0.1.4a0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-sdk
-Version: 0.1.4a0.dev6
+Version: 0.1.4a0.dev7
 Summary: A python wrapper around the tastytrade open API
 License: MIT
 Author: Aaron Mamparo
 Author-email: aaronmamparo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

