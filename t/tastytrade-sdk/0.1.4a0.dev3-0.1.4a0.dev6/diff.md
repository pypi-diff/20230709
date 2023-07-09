# Comparing `tmp/tastytrade_sdk-0.1.4a0.dev3.tar.gz` & `tmp/tastytrade_sdk-0.1.4a0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade_sdk-0.1.4a0.dev3.tar", max compression
+gzip compressed data, was "tastytrade_sdk-0.1.4a0.dev6.tar", max compression
```

## Comparing `tastytrade_sdk-0.1.4a0.dev3.tar` & `tastytrade_sdk-0.1.4a0.dev6.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1053 2023-07-09 19:26:05.122836 tastytrade_sdk-0.1.4a0.dev3/LICENSE
--rw-r--r--   0        0        0     1652 2023-07-09 19:26:05.122836 tastytrade_sdk-0.1.4a0.dev3/docs/users/README.md
--rw-r--r--   0        0        0      822 2023-07-09 19:26:43.874481 tastytrade_sdk-0.1.4a0.dev3/pyproject.toml
--rw-r--r--   0        0        0      516 2023-07-09 19:26:05.122836 tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/__init__.py
--rw-r--r--   0        0        0     2624 2023-07-09 19:26:05.122836 tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/account.py
--rw-r--r--   0        0        0     4185 2023-07-09 19:26:05.122836 tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/api.py
--rw-r--r--   0        0        0      136 2023-07-09 19:26:05.122836 tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/config.py
--rw-r--r--   0        0        0      421 2023-07-09 19:26:05.122836 tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-09 19:26:05.122836 tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/market_data/__init__.py
--rw-r--r--   0        0        0     1548 2023-07-09 19:26:05.122836 tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/market_data/market_data.py
--rw-r--r--   0        0        0     2646 2023-07-09 19:26:05.122836 tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/market_data/models.py
--rw-r--r--   0        0        0     1889 2023-07-09 19:26:05.122836 tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/market_data/streamer_symbol_translation.py
--rw-r--r--   0        0        0     6137 2023-07-09 19:26:05.122836 tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/market_data/subscription.py
--rw-r--r--   0        0        0     1125 2023-07-09 19:26:05.122836 tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/orders.py
--rw-r--r--   0        0        0     1496 2023-07-09 19:26:05.122836 tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/tastytrade.py
--rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 tastytrade_sdk-0.1.4a0.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/LICENSE
+-rw-r--r--   0        0        0     1652 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/docs/users/README.md
+-rw-r--r--   0        0        0      822 2023-07-09 19:38:28.310251 tastytrade_sdk-0.1.4a0.dev6/pyproject.toml
+-rw-r--r--   0        0        0      614 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/__init__.py
+-rw-r--r--   0        0        0     2675 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/account.py
+-rw-r--r--   0        0        0     4185 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/api.py
+-rw-r--r--   0        0        0      136 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/config.py
+-rw-r--r--   0        0        0      421 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/__init__.py
+-rw-r--r--   0        0        0     1548 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/market_data.py
+-rw-r--r--   0        0        0     2646 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/models.py
+-rw-r--r--   0        0        0     1889 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/streamer_symbol_translation.py
+-rw-r--r--   0        0        0     6137 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/subscription.py
+-rw-r--r--   0        0        0        0 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/orders/__init__.py
+-rw-r--r--   0        0        0      731 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/orders/models.py
+-rw-r--r--   0        0        0      482 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/orders/orders.py
+-rw-r--r--   0        0        0     1503 2023-07-09 19:37:49.826034 tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/tastytrade.py
+-rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 tastytrade_sdk-0.1.4a0.dev6/PKG-INFO
```

### Comparing `tastytrade_sdk-0.1.4a0.dev3/LICENSE` & `tastytrade_sdk-0.1.4a0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev3/docs/users/README.md` & `tastytrade_sdk-0.1.4a0.dev6/docs/users/README.md`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev3/pyproject.toml` & `tastytrade_sdk-0.1.4a0.dev6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tastytrade-sdk"
-version = "0.1.4a0dev3"
+version = "0.1.4a0dev6"
 description = "A python wrapper around the tastytrade open API"
 authors = [
     "Aaron Mamparo <aaronmamparo@gmail.com>"
 ]
 license = "MIT"
 readme = "docs/users/README.md"
 packages = [
```

### Comparing `tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/__init__.py` & `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 .. include:: ../../docs/users/README.md
 ---
 """
 
-# Make these classes visible in the auto-generated documentation
+# Make these classes available to the user and visible in the auto-generated documentation
 __all__ = [
     'Tastytrade',
     'MarketData', 'Subscription', 'Quote', 'Candle', 'Greeks',
-    'Api'
+    'Api',
+    'Order', 'Leg'
 ]
 
 from tastytrade_sdk.api import Api, QueryParams
 from tastytrade_sdk.market_data.market_data import MarketData
 from tastytrade_sdk.market_data.models import Quote, Candle, Greeks
 from tastytrade_sdk.market_data.subscription import Subscription
+from tastytrade_sdk.orders.models import Order, Leg
 from tastytrade_sdk.tastytrade import Tastytrade
```

### Comparing `tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/account.py` & `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass
 from typing import List, Optional, Tuple, Any
 
-from tastytrade_sdk import Api
-from tastytrade_sdk.orders import Orders, Order
+from tastytrade_sdk.api import Api
+from tastytrade_sdk.orders.orders import Orders
+from tastytrade_sdk.orders.models import Order
 
 
 @dataclass
 class PositionsParams:
     underlying_symbols: Optional[List[str]] = None
     symbol: Optional[str] = None
     instrument_type: Optional[str] = None
```

### Comparing `tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/api.py` & `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/api.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/market_data/market_data.py` & `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/market_data.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/market_data/models.py` & `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/models.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/market_data/streamer_symbol_translation.py` & `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/streamer_symbol_translation.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/market_data/subscription.py` & `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/market_data/subscription.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.4a0.dev3/src/tastytrade_sdk/tastytrade.py` & `tastytrade_sdk-0.1.4a0.dev6/src/tastytrade_sdk/tastytrade.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from injector import Injector
 
 from tastytrade_sdk.account import Account
 from tastytrade_sdk.config import Config
 from tastytrade_sdk.api import Api, RequestsSession
 from tastytrade_sdk.market_data.market_data import MarketData
-from tastytrade_sdk.orders import Orders
+from tastytrade_sdk.orders.orders import Orders
 
 
 class Tastytrade:
     """
     The SDK's top-level class
     """
```

### Comparing `tastytrade_sdk-0.1.4a0.dev3/PKG-INFO` & `tastytrade_sdk-0.1.4a0.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-sdk
-Version: 0.1.4a0.dev3
+Version: 0.1.4a0.dev6
 Summary: A python wrapper around the tastytrade open API
 License: MIT
 Author: Aaron Mamparo
 Author-email: aaronmamparo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

