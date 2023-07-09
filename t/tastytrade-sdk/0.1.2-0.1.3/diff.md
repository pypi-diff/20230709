# Comparing `tmp/tastytrade_sdk-0.1.2.tar.gz` & `tmp/tastytrade_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade_sdk-0.1.2.tar", max compression
+gzip compressed data, was "tastytrade_sdk-0.1.3.tar", max compression
```

## Comparing `tastytrade_sdk-0.1.2.tar` & `tastytrade_sdk-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1053 2023-07-08 07:22:28.139077 tastytrade_sdk-0.1.2/LICENSE
--rw-r--r--   0        0        0     1652 2023-07-08 07:22:28.139077 tastytrade_sdk-0.1.2/docs/users/README.md
--rw-r--r--   0        0        0      816 2023-07-08 07:22:28.139077 tastytrade_sdk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      516 2023-07-08 07:22:28.139077 tastytrade_sdk-0.1.2/src/tastytrade_sdk/__init__.py
--rw-r--r--   0        0        0     4185 2023-07-08 07:22:28.139077 tastytrade_sdk-0.1.2/src/tastytrade_sdk/api.py
--rw-r--r--   0        0        0      136 2023-07-08 07:22:28.139077 tastytrade_sdk-0.1.2/src/tastytrade_sdk/config.py
--rw-r--r--   0        0        0      421 2023-07-08 07:22:28.139077 tastytrade_sdk-0.1.2/src/tastytrade_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-08 07:22:28.139077 tastytrade_sdk-0.1.2/src/tastytrade_sdk/market_data/__init__.py
--rw-r--r--   0        0        0     1548 2023-07-08 07:22:28.139077 tastytrade_sdk-0.1.2/src/tastytrade_sdk/market_data/market_data.py
--rw-r--r--   0        0        0     2646 2023-07-08 07:22:28.139077 tastytrade_sdk-0.1.2/src/tastytrade_sdk/market_data/models.py
--rw-r--r--   0        0        0     1889 2023-07-08 07:22:28.143077 tastytrade_sdk-0.1.2/src/tastytrade_sdk/market_data/streamer_symbol_translation.py
--rw-r--r--   0        0        0     6137 2023-07-08 07:22:28.143077 tastytrade_sdk-0.1.2/src/tastytrade_sdk/market_data/subscription.py
--rw-r--r--   0        0        0     1266 2023-07-08 07:22:28.143077 tastytrade_sdk-0.1.2/src/tastytrade_sdk/tastytrade.py
--rw-r--r--   0        0        0     2453 1970-01-01 00:00:00.000000 tastytrade_sdk-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-07-09 05:07:09.064606 tastytrade_sdk-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1652 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/docs/users/README.md
+-rw-r--r--   0        0        0      816 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      516 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/__init__.py
+-rw-r--r--   0        0        0     4185 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/api.py
+-rw-r--r--   0        0        0      136 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/config.py
+-rw-r--r--   0        0        0      421 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/__init__.py
+-rw-r--r--   0        0        0     1548 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/market_data.py
+-rw-r--r--   0        0        0     2646 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/models.py
+-rw-r--r--   0        0        0     1889 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/streamer_symbol_translation.py
+-rw-r--r--   0        0        0     6137 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/subscription.py
+-rw-r--r--   0        0        0     1266 2023-07-09 05:07:09.068606 tastytrade_sdk-0.1.3/src/tastytrade_sdk/tastytrade.py
+-rw-r--r--   0        0        0     2453 1970-01-01 00:00:00.000000 tastytrade_sdk-0.1.3/PKG-INFO
```

### Comparing `tastytrade_sdk-0.1.2/LICENSE` & `tastytrade_sdk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.2/docs/users/README.md` & `tastytrade_sdk-0.1.3/docs/users/README.md`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.2/pyproject.toml` & `tastytrade_sdk-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tastytrade-sdk"
-version = "0.1.2"
+version = "0.1.3"
 description = "A python wrapper around the tastytrade open API"
 authors = [
     "Aaron Mamparo <aaronmamparo@gmail.com>"
 ]
 license = "MIT"
 readme = "docs/users/README.md"
 packages = [
```

### Comparing `tastytrade_sdk-0.1.2/src/tastytrade_sdk/__init__.py` & `tastytrade_sdk-0.1.3/src/tastytrade_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.2/src/tastytrade_sdk/api.py` & `tastytrade_sdk-0.1.3/src/tastytrade_sdk/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             data={'login': login, 'password': password}
         )['data']['session-token']
 
     def request(self, method: str, path: str, params: Optional[QueryParams] = tuple(),
                 data: Optional[dict] = None) -> Optional[dict]:
         url = self.__url(path, params)
         logging.debug('%s %s', path, params)
-        response = self.__session.request(method, url, data=data, headers={'User-Agent': self.__user_agent})
+        response = self.__session.request(method, url, json=data, headers={'User-Agent': self.__user_agent})
         is_ok = 200 <= response.status_code <= 399
         if is_ok:
             try:
                 return response.json()
             except JSONDecodeError:
                 return None
         if response.status_code == 400:
```

### Comparing `tastytrade_sdk-0.1.2/src/tastytrade_sdk/market_data/market_data.py` & `tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/market_data.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.2/src/tastytrade_sdk/market_data/models.py` & `tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/models.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.2/src/tastytrade_sdk/market_data/streamer_symbol_translation.py` & `tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/streamer_symbol_translation.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.2/src/tastytrade_sdk/market_data/subscription.py` & `tastytrade_sdk-0.1.3/src/tastytrade_sdk/market_data/subscription.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.2/src/tastytrade_sdk/tastytrade.py` & `tastytrade_sdk-0.1.3/src/tastytrade_sdk/tastytrade.py`

 * *Files identical despite different names*

### Comparing `tastytrade_sdk-0.1.2/PKG-INFO` & `tastytrade_sdk-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python wrapper around the tastytrade open API
 License: MIT
 Author: Aaron Mamparo
 Author-email: aaronmamparo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

