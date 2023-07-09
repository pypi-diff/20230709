# Comparing `tmp/tastytrade_sdk-0.1.3.tar.gz` & `tmp/tastytrade_sdk-0.1.4a0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade_sdk-0.1.3.tar", max compression
+gzip compressed data, was "tastytrade_sdk-0.1.4a0.dev1.tar", max compression
```

## Comparing `tastytrade_sdk-0.1.3.tar` & `tastytrade_sdk-0.1.4a0.dev1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1053 2023-07-09 05:07:09.064606 tastytrade_sdk-0.1.3/LICENSE
--rw-r--r--   0        0        0     1652 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/docs/users/README.md
--rw-r--r--   0        0        0      816 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      516 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/__init__.py
--rw-r--r--   0        0        0     4185 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/api.py
--rw-r--r--   0        0        0      136 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/config.py
--rw-r--r--   0        0        0      421 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/__init__.py
--rw-r--r--   0        0        0     1548 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/market_data.py
--rw-r--r--   0        0        0     2646 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/models.py
--rw-r--r--   0        0        0     1889 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/streamer_symbol_translation.py
--rw-r--r--   0        0        0     6137 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/subscription.py
--rw-r--r--   0        0        0     1266 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/tastytrade.py
--rw-r--r--   0        0        0     2453 1970-01-01 00:00:00.000000 tastytrade_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/LICENSE
+-rw-r--r--   0        0        0     1652 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/docs/users/README.md
+-rw-r--r--   0        0        0      822 2023-07-09 18:50:24.100857 tastytrade_sdk-0.1.4a0.dev1/pyproject.toml
+-rw-r--r--   0        0        0      516 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/__init__.py
+-rw-r--r--   0        0        0     2018 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/account.py
+-rw-r--r--   0        0        0     4185 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/api.py
+-rw-r--r--   0        0        0      136 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/config.py
+-rw-r--r--   0        0        0      421 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/__init__.py
+-rw-r--r--   0        0        0     1548 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/market_data.py
+-rw-r--r--   0        0        0     2646 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/models.py
+-rw-r--r--   0        0        0     1889 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/streamer_symbol_translation.py
+-rw-r--r--   0        0        0     6137 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/subscription.py
+-rw-r--r--   0        0        0     1414 2023-07-09 18:49:50.011980 tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/tastytrade.py
+-rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 tastytrade_sdk-0.1.4a0.dev1/PKG-INFO
```

### Comparing `tastytrade_sdk-0.1.3/LICENSE` & `tastytrade_sdk-0.1.4a0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.3/docs/users/README.md` & `tastytrade_sdk-0.1.4a0.dev1/docs/users/README.md`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.3/pyproject.toml` & `tastytrade_sdk-0.1.4a0.dev1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tastytrade-sdk"
-version = "0.1.3"
+version = "0.1.4a0dev1"
 description = "A python wrapper around the tastytrade open API"
 authors = [
     "Aaron Mamparo <aaronmamparo@gmail.com>"
 ]
 license = "MIT"
 readme = "docs/users/README.md"
 packages = [
```

### Comparing `tastytrade_sdk-0.1.3/src/tastytrade_sdk/__init__.py` & `tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.3/src/tastytrade_sdk/api.py` & `tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/api.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/market_data.py` & `tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/market_data.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/models.py` & `tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/models.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/streamer_symbol_translation.py` & `tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/streamer_symbol_translation.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/subscription.py` & `tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/market_data/subscription.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.3/src/tastytrade_sdk/tastytrade.py` & `tastytrade_sdk-0.1.4a0.dev1/src/tastytrade_sdk/tastytrade.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from injector import Injector
 
+from tastytrade_sdk.account import Account
 from tastytrade_sdk.config import Config
 from tastytrade_sdk.api import Api, RequestsSession
 from tastytrade_sdk.market_data.market_data import MarketData
 
 
 class Tastytrade:
     """
@@ -30,14 +31,17 @@
 
     def logout(self) -> None:
         """
         End the session
         """
         self.api.delete('/sessions')
 
+    def account(self, account_number: str) -> Account:
+        return Account(account_number, self.api)
+
     @property
     def market_data(self) -> MarketData:
         """
         Access the MarketData submodule
         """
         return self.__container.get(MarketData)
```

### Comparing `tastytrade_sdk-0.1.3/PKG-INFO` & `tastytrade_sdk-0.1.4a0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-sdk
-Version: 0.1.3
+Version: 0.1.4a0.dev1
 Summary: A python wrapper around the tastytrade open API
 License: MIT
 Author: Aaron Mamparo
 Author-email: aaronmamparo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

