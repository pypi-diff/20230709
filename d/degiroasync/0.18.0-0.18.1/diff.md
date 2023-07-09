# Comparing `tmp/degiroasync-0.18.0.tar.gz` & `tmp/degiroasync-0.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degiroasync-0.18.0.tar", last modified: Sat Jul  8 08:42:07 2023, max compression
+gzip compressed data, was "degiroasync-0.18.1.tar", last modified: Sun Jul  9 09:11:35 2023, max compression
```

## Comparing `degiroasync-0.18.0.tar` & `degiroasync-0.18.1.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-08 08:42:07.048696 degiroasync-0.18.0/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1075 2022-01-20 21:38:48.000000 degiroasync-0.18.0/LICENSE
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5044 2023-07-08 08:42:07.048696 degiroasync-0.18.0/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4352 2023-07-08 08:35:06.000000 degiroasync-0.18.0/README.md
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-08 08:42:07.044696 degiroasync-0.18.0/degiroasync/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      692 2022-04-13 19:10:04.000000 degiroasync-0.18.0/degiroasync/__init__.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-08 08:42:07.048696 degiroasync-0.18.0/degiroasync/api/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4266 2023-07-08 08:13:36.000000 degiroasync-0.18.0/degiroasync/api/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     8334 2022-05-12 19:40:07.000000 degiroasync-0.18.0/degiroasync/api/orders.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    31824 2023-07-08 08:24:47.000000 degiroasync-0.18.0/degiroasync/api/product.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     8975 2023-07-02 19:55:02.000000 degiroasync-0.18.0/degiroasync/api/session.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-08 08:42:07.048696 degiroasync-0.18.0/degiroasync/core/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1551 2023-03-13 17:53:33.000000 degiroasync-0.18.0/degiroasync/core/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     6556 2023-07-08 08:00:18.000000 degiroasync-0.18.0/degiroasync/core/constants.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    14273 2023-07-05 15:56:57.000000 degiroasync-0.18.0/degiroasync/core/core.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      547 2023-03-13 16:44:13.000000 degiroasync-0.18.0/degiroasync/core/exceptions.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    16476 2023-07-08 08:24:23.000000 degiroasync-0.18.0/degiroasync/core/helpers.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-08 08:42:07.048696 degiroasync-0.18.0/degiroasync/webapi/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1857 2023-07-08 08:08:05.000000 degiroasync-0.18.0/degiroasync/webapi/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5780 2023-07-02 17:18:01.000000 degiroasync-0.18.0/degiroasync/webapi/login.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    12060 2023-07-02 17:18:26.000000 degiroasync-0.18.0/degiroasync/webapi/orders.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    28777 2023-07-08 08:17:42.000000 degiroasync-0.18.0/degiroasync/webapi/product.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-08 08:42:07.044696 degiroasync-0.18.0/degiroasync.egg-info/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5044 2023-07-08 08:42:07.000000 degiroasync-0.18.0/degiroasync.egg-info/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      743 2023-07-08 08:42:07.000000 degiroasync-0.18.0/degiroasync.egg-info/SOURCES.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-07-08 08:42:07.000000 degiroasync-0.18.0/degiroasync.egg-info/dependency_links.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      293 2023-07-08 08:42:07.000000 degiroasync-0.18.0/degiroasync.egg-info/requires.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       18 2023-07-08 08:42:07.000000 degiroasync-0.18.0/degiroasync.egg-info/top_level.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      108 2022-02-26 15:27:30.000000 degiroasync-0.18.0/pyproject.toml
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2023-07-08 08:42:07.048696 degiroasync-0.18.0/setup.cfg
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     2209 2023-07-07 09:15:51.000000 degiroasync-0.18.0/setup.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-08 08:42:07.048696 degiroasync-0.18.0/tests/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2023-07-02 12:58:48.000000 degiroasync-0.18.0/tests/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1504 2023-07-02 16:37:29.000000 degiroasync-0.18.0/tests/integration_login.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4826 2023-07-08 08:25:07.000000 degiroasync-0.18.0/tests/test_core.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    36370 2023-07-08 08:14:24.000000 degiroasync-0.18.0/tests/test_degiroapi.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    19359 2023-07-08 08:14:36.000000 degiroasync-0.18.0/tests/test_degirowebapi.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      153 2022-01-27 15:50:02.000000 degiroasync-0.18.0/tests/test_setup.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-09 09:11:35.489396 degiroasync-0.18.1/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1075 2023-07-08 16:07:32.000000 degiroasync-0.18.1/LICENSE
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5044 2023-07-09 09:11:35.489396 degiroasync-0.18.1/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4352 2023-07-08 16:07:32.000000 degiroasync-0.18.1/README.md
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-09 09:11:35.485396 degiroasync-0.18.1/degiroasync/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      692 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/__init__.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-09 09:11:35.489396 degiroasync-0.18.1/degiroasync/api/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4330 2023-07-09 09:11:20.000000 degiroasync-0.18.1/degiroasync/api/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     8334 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/api/orders.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    31824 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/api/product.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     8975 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/api/session.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-09 09:11:35.489396 degiroasync-0.18.1/degiroasync/core/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1551 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/core/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     6556 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/core/constants.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    14273 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/core/core.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      547 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/core/exceptions.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    16476 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/core/helpers.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-09 09:11:35.489396 degiroasync-0.18.1/degiroasync/webapi/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1925 2023-07-09 09:11:20.000000 degiroasync-0.18.1/degiroasync/webapi/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5780 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/webapi/login.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    12060 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/webapi/orders.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    28777 2023-07-08 16:07:32.000000 degiroasync-0.18.1/degiroasync/webapi/product.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-09 09:11:35.485396 degiroasync-0.18.1/degiroasync.egg-info/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5044 2023-07-09 09:11:35.000000 degiroasync-0.18.1/degiroasync.egg-info/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      723 2023-07-09 09:11:35.000000 degiroasync-0.18.1/degiroasync.egg-info/SOURCES.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-07-09 09:11:35.000000 degiroasync-0.18.1/degiroasync.egg-info/dependency_links.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      293 2023-07-09 09:11:35.000000 degiroasync-0.18.1/degiroasync.egg-info/requires.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       18 2023-07-09 09:11:35.000000 degiroasync-0.18.1/degiroasync.egg-info/top_level.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      108 2023-07-08 16:07:32.000000 degiroasync-0.18.1/pyproject.toml
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2023-07-09 09:11:35.489396 degiroasync-0.18.1/setup.cfg
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     2209 2023-07-09 09:11:20.000000 degiroasync-0.18.1/setup.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-09 09:11:35.489396 degiroasync-0.18.1/tests/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2023-07-08 16:07:32.000000 degiroasync-0.18.1/tests/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1504 2023-07-08 16:07:32.000000 degiroasync-0.18.1/tests/integration_login.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4826 2023-07-08 16:07:32.000000 degiroasync-0.18.1/tests/test_core.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    36370 2023-07-08 16:07:32.000000 degiroasync-0.18.1/tests/test_degiroapi.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    19359 2023-07-08 16:07:32.000000 degiroasync-0.18.1/tests/test_degirowebapi.py
```

### Comparing `degiroasync-0.18.0/LICENSE` & `degiroasync-0.18.1/LICENSE`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/PKG-INFO` & `degiroasync-0.18.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degiroasync
-Version: 0.18.0
+Version: 0.18.1
 Summary: A Python asynchronous library for Degiro trading service.
 Home-page: https://github.com/OhMajesticLama/degiroasync
 Author-email: ohmajesticlama@gmail.com
 Project-URL: Documentation, https://ohmajesticlama.github.io/degiroasync/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `degiroasync-0.18.0/README.md` & `degiroasync-0.18.1/README.md`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/degiroasync/__init__.py` & `degiroasync-0.18.1/degiroasync/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/degiroasync/api/__init__.py` & `degiroasync-0.18.1/degiroasync/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 from .session import login
 from .session import get_exchange_dictionary
 from .session import ExchangeDictionary
 from .session import Exchange, Region, Country
 from .product import get_portfolio
 from .product import get_portfolio_total
 from .product import get_price_series
+from .product import get_price_data
 from .product import search_product
 from .product import Stock
 from .product import Currency
 from .product import ProductBase
 from .product import ProductFactory  # Don't expose in __all__
 from .product import ProductGeneric
 from .product import PriceSeries
@@ -98,14 +99,15 @@
             get_exchange_dictionary,
             ExchangeDictionary,
             Exchange, Region, Country,
 
             # Product
             search_product,
             get_portfolio,
+            get_price_data,
             get_price_series,
 
             # PriceData,
             PriceSeries,
             Stock,
             Currency,
             ProductBase,
```

### Comparing `degiroasync-0.18.0/degiroasync/api/orders.py` & `degiroasync-0.18.1/degiroasync/api/orders.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/degiroasync/api/product.py` & `degiroasync-0.18.1/degiroasync/api/product.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/degiroasync/api/session.py` & `degiroasync-0.18.1/degiroasync/api/session.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/degiroasync/core/__init__.py` & `degiroasync-0.18.1/degiroasync/core/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/degiroasync/core/constants.py` & `degiroasync-0.18.1/degiroasync/core/constants.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/degiroasync/core/core.py` & `degiroasync-0.18.1/degiroasync/core/core.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/degiroasync/core/exceptions.py` & `degiroasync-0.18.1/degiroasync/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/degiroasync/core/helpers.py` & `degiroasync-0.18.1/degiroasync/core/helpers.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/degiroasync/webapi/__init__.py` & `degiroasync-0.18.1/degiroasync/webapi/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from .login import get_account_info
 from .product import get_products_info
 from .product import search_product
 from .product import get_portfolio
 from .product import get_portfolio_total
 from .product import get_company_profile
 from .product import get_news_by_company
+from .product import get_price_data
 from .product import get_price_series
 from .orders import get_orders
 from .orders import get_orders_history
 from .orders import get_transactions
 from .orders import confirm_order
 from .orders import check_order
 from .orders import ORDER_DATE_FORMAT
@@ -46,14 +47,15 @@
                 # product
                 get_portfolio,
                 get_portfolio_total,
                 get_products_info,
                 search_product,
                 get_company_profile,
                 get_news_by_company,
+                get_price_data,
                 get_price_series,
                 # orders
                 get_orders,
                 get_orders_history,
                 get_transactions,
                 confirm_order,
                 check_order,
```

### Comparing `degiroasync-0.18.0/degiroasync/webapi/login.py` & `degiroasync-0.18.1/degiroasync/webapi/login.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/degiroasync/webapi/orders.py` & `degiroasync-0.18.1/degiroasync/webapi/orders.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/degiroasync/webapi/product.py` & `degiroasync-0.18.1/degiroasync/webapi/product.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/degiroasync.egg-info/PKG-INFO` & `degiroasync-0.18.1/degiroasync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degiroasync
-Version: 0.18.0
+Version: 0.18.1
 Summary: A Python asynchronous library for Degiro trading service.
 Home-page: https://github.com/OhMajesticLama/degiroasync
 Author-email: ohmajesticlama@gmail.com
 Project-URL: Documentation, https://ohmajesticlama.github.io/degiroasync/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `degiroasync-0.18.0/degiroasync.egg-info/SOURCES.txt` & `degiroasync-0.18.1/degiroasync.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,9 +21,8 @@
 degiroasync/webapi/login.py
 degiroasync/webapi/orders.py
 degiroasync/webapi/product.py
 tests/__init__.py
 tests/integration_login.py
 tests/test_core.py
 tests/test_degiroapi.py
-tests/test_degirowebapi.py
-tests/test_setup.py
+tests/test_degirowebapi.py
```

### Comparing `degiroasync-0.18.0/setup.py` & `degiroasync-0.18.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     description = "A Python asynchronous library for Degiro trading service."
     readme_path = os.path.join(os.path.dirname(__file__), 'README.md')
     with open(readme_path, "r") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="degiroasync",
-        version="0.18.0",
+        version="0.18.1",
         author_email="ohmajesticlama@gmail.com",
         description=description,
         long_description=long_description,
         long_description_content_type='text/markdown',
         url="https://github.com/OhMajesticLama/degiroasync",
         project_urls={
             'Documentation':
```

### Comparing `degiroasync-0.18.0/tests/integration_login.py` & `degiroasync-0.18.1/tests/integration_login.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/tests/test_core.py` & `degiroasync-0.18.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/tests/test_degiroapi.py` & `degiroasync-0.18.1/tests/test_degiroapi.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.18.0/tests/test_degirowebapi.py` & `degiroasync-0.18.1/tests/test_degirowebapi.py`

 * *Files identical despite different names*

