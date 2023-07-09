# Comparing `tmp/service_markets-0.3.7.tar.gz` & `tmp/service_markets-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "service_markets-0.3.7.tar", max compression
+gzip compressed data, was "service_markets-0.3.8.tar", max compression
```

## Comparing `service_markets-0.3.7.tar` & `service_markets-0.3.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2023-07-07 14:40:33.550520 service_markets-0.3.7/LICENSE
--rw-r--r--   0        0        0     1898 2023-07-08 09:02:23.832368 service_markets-0.3.7/README.md
--rw-r--r--   0        0        0      918 2023-07-09 03:34:48.985946 service_markets-0.3.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.7/src/service_markets/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.7/src/service_markets/api/__init__.py
--rw-r--r--   0        0        0     1254 2023-07-09 02:03:07.892011 service_markets-0.3.7/src/service_markets/api/api_model.py
--rw-r--r--   0        0        0     2553 2023-07-08 15:14:04.217846 service_markets-0.3.7/src/service_markets/api/main.py
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.7/src/service_markets/api/routers/__init__.py
--rw-r--r--   0        0        0     8502 2023-07-09 02:05:32.939412 service_markets-0.3.7/src/service_markets/api/routers/services.py
--rw-r--r--   0        0        0     2265 2023-07-08 19:15:04.173133 service_markets-0.3.7/src/service_markets/api/routers/users.py
--rw-r--r--   0        0        0      178 2023-07-07 14:40:33.558522 service_markets-0.3.7/src/service_markets/api/utils.py
--rw-r--r--   0        0        0        1 2023-07-07 14:40:33.558522 service_markets-0.3.7/src/service_markets/core/__init__.py
--rw-r--r--   0        0        0      780 2023-07-08 20:07:33.642896 service_markets-0.3.7/src/service_markets/core/constants.py
--rw-r--r--   0        0        0     3245 2023-07-09 03:34:48.969946 service_markets-0.3.7/src/service_markets/core/heimdall.py
--rw-r--r--   0        0        0     1114 2023-07-09 02:03:07.900011 service_markets-0.3.7/src/service_markets/core/model.py
--rw-r--r--   0        0        0     1520 2023-07-09 02:03:07.876011 service_markets-0.3.7/src/service_markets/core/request_network.py
--rw-r--r--   0        0        0     2769 2023-07-08 20:04:11.540378 service_markets-0.3.7/src/service_markets/core/session.py
--rw-r--r--   0        0        0     1342 2023-07-07 18:59:02.549799 service_markets-0.3.7/src/service_markets/local_listener.py
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.562523 service_markets-0.3.7/src/service_markets/py.typed
--rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 service_markets-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-07 14:40:33.550520 service_markets-0.3.8/LICENSE
+-rw-r--r--   0        0        0     1898 2023-07-08 09:02:23.832368 service_markets-0.3.8/README.md
+-rw-r--r--   0        0        0      918 2023-07-09 03:43:22.706422 service_markets-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.8/src/service_markets/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.8/src/service_markets/api/__init__.py
+-rw-r--r--   0        0        0     1254 2023-07-09 02:03:07.892011 service_markets-0.3.8/src/service_markets/api/api_model.py
+-rw-r--r--   0        0        0     2553 2023-07-08 15:14:04.217846 service_markets-0.3.8/src/service_markets/api/main.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.8/src/service_markets/api/routers/__init__.py
+-rw-r--r--   0        0        0     8502 2023-07-09 02:05:32.939412 service_markets-0.3.8/src/service_markets/api/routers/services.py
+-rw-r--r--   0        0        0     2265 2023-07-08 19:15:04.173133 service_markets-0.3.8/src/service_markets/api/routers/users.py
+-rw-r--r--   0        0        0      178 2023-07-07 14:40:33.558522 service_markets-0.3.8/src/service_markets/api/utils.py
+-rw-r--r--   0        0        0        1 2023-07-07 14:40:33.558522 service_markets-0.3.8/src/service_markets/core/__init__.py
+-rw-r--r--   0        0        0      780 2023-07-08 20:07:33.642896 service_markets-0.3.8/src/service_markets/core/constants.py
+-rw-r--r--   0        0        0     3245 2023-07-09 03:34:48.969946 service_markets-0.3.8/src/service_markets/core/heimdall.py
+-rw-r--r--   0        0        0     1114 2023-07-09 02:03:07.900011 service_markets-0.3.8/src/service_markets/core/model.py
+-rw-r--r--   0        0        0     1520 2023-07-09 02:03:07.876011 service_markets-0.3.8/src/service_markets/core/request_network.py
+-rw-r--r--   0        0        0     2840 2023-07-09 03:43:22.686422 service_markets-0.3.8/src/service_markets/core/session.py
+-rw-r--r--   0        0        0     1342 2023-07-07 18:59:02.549799 service_markets-0.3.8/src/service_markets/local_listener.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.562523 service_markets-0.3.8/src/service_markets/py.typed
+-rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 service_markets-0.3.8/PKG-INFO
```

### Comparing `service_markets-0.3.7/LICENSE` & `service_markets-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.7/README.md` & `service_markets-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.7/pyproject.toml` & `service_markets-0.3.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 tags = ["aleph.im", "saas", "marketplace", "cryptocurrency", "fastapi"]
 
 [tool.poetry]
 name = "service-markets"
-version = "0.3.7"
+version = "0.3.8"
 description = "Software-as-a-Service (SaaS) Marketplace with cryptocurrency payments"
 authors = ["Mike Hukiewitz <mike.hukiewitz@robotter.ai>"]
 license = "AGPL-3.0"
 readme = "README.md"
 packages = [{include = "service_markets", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `service_markets-0.3.7/src/service_markets/api/api_model.py` & `service_markets-0.3.8/src/service_markets/api/api_model.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.7/src/service_markets/api/main.py` & `service_markets-0.3.8/src/service_markets/api/main.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.7/src/service_markets/api/routers/services.py` & `service_markets-0.3.8/src/service_markets/api/routers/services.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.7/src/service_markets/api/routers/users.py` & `service_markets-0.3.8/src/service_markets/api/routers/users.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.7/src/service_markets/core/constants.py` & `service_markets-0.3.8/src/service_markets/core/constants.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.7/src/service_markets/core/heimdall.py` & `service_markets-0.3.8/src/service_markets/core/heimdall.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.7/src/service_markets/core/model.py` & `service_markets-0.3.8/src/service_markets/core/model.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.7/src/service_markets/core/request_network.py` & `service_markets-0.3.8/src/service_markets/core/request_network.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.7/src/service_markets/core/session.py` & `service_markets-0.3.8/src/service_markets/core/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,17 @@
     if custom_channel:
         channel = custom_channel
     elif test_channel_flag is not None and test_channel_flag.lower() == "true":
         channel = "SERVICE_MARKETS_TEST_" + str(datetime.now())
     else:
         channel = SERVICE_MARKETS_MESSAGE_CHANNEL
 
+    if not channel:
+        channel = SERVICE_MARKETS_MESSAGE_CHANNEL
+
     print("Using channel: " + channel)
 
     aars = AARS(
         account=aleph_account, channel=channel, cache=cache, session=aleph_session
     )
     print(f"Using account: {aleph_account.get_address()}")
     if aleph_account.get_address() in SERVICE_MARKETS_MANAGER_PUBKEYS:
```

### Comparing `service_markets-0.3.7/src/service_markets/local_listener.py` & `service_markets-0.3.8/src/service_markets/local_listener.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.7/PKG-INFO` & `service_markets-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: service-markets
-Version: 0.3.7
+Version: 0.3.8
 Summary: Software-as-a-Service (SaaS) Marketplace with cryptocurrency payments
 License: AGPL-3.0
 Author: Mike Hukiewitz
 Author-email: mike.hukiewitz@robotter.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

