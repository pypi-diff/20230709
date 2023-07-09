# Comparing `tmp/service_markets-0.3.1.tar.gz` & `tmp/service_markets-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "service_markets-0.3.1.tar", max compression
+gzip compressed data, was "service_markets-0.3.2.tar", max compression
```

## Comparing `service_markets-0.3.1.tar` & `service_markets-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34523 2023-07-07 14:40:33.550520 service_markets-0.3.1/LICENSE
--rw-r--r--   0        0        0     1898 2023-07-08 09:02:23.832368 service_markets-0.3.1/README.md
--rw-r--r--   0        0        0      918 2023-07-08 22:52:32.029214 service_markets-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.1/src/service_markets/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.1/src/service_markets/api/__init__.py
--rw-r--r--   0        0        0     1104 2023-07-08 18:56:29.117429 service_markets-0.3.1/src/service_markets/api/api_model.py
--rw-r--r--   0        0        0     2553 2023-07-08 15:14:04.217846 service_markets-0.3.1/src/service_markets/api/main.py
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.1/src/service_markets/api/routers/__init__.py
--rw-r--r--   0        0        0     7183 2023-07-08 19:15:04.169133 service_markets-0.3.1/src/service_markets/api/routers/services.py
--rw-r--r--   0        0        0     2265 2023-07-08 19:15:04.173133 service_markets-0.3.1/src/service_markets/api/routers/users.py
--rw-r--r--   0        0        0      178 2023-07-07 14:40:33.558522 service_markets-0.3.1/src/service_markets/api/utils.py
--rw-r--r--   0        0        0        1 2023-07-07 14:40:33.558522 service_markets-0.3.1/src/service_markets/core/__init__.py
--rw-r--r--   0        0        0      780 2023-07-08 20:07:33.642896 service_markets-0.3.1/src/service_markets/core/constants.py
--rw-r--r--   0        0        0     3074 2023-07-08 19:15:04.157133 service_markets-0.3.1/src/service_markets/core/heimdall.py
--rw-r--r--   0        0        0      878 2023-07-08 15:13:58.497873 service_markets-0.3.1/src/service_markets/core/model.py
--rw-r--r--   0        0        0     2769 2023-07-08 20:04:11.540378 service_markets-0.3.1/src/service_markets/core/session.py
--rw-r--r--   0        0        0     1342 2023-07-07 18:59:02.549799 service_markets-0.3.1/src/service_markets/local_listener.py
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.562523 service_markets-0.3.1/src/service_markets/py.typed
--rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 service_markets-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-07 14:40:33.550520 service_markets-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1898 2023-07-08 09:02:23.832368 service_markets-0.3.2/README.md
+-rw-r--r--   0        0        0      918 2023-07-09 00:01:05.930639 service_markets-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.2/src/service_markets/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.2/src/service_markets/api/__init__.py
+-rw-r--r--   0        0        0     1104 2023-07-08 18:56:29.117429 service_markets-0.3.2/src/service_markets/api/api_model.py
+-rw-r--r--   0        0        0     2553 2023-07-08 15:14:04.217846 service_markets-0.3.2/src/service_markets/api/main.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.2/src/service_markets/api/routers/__init__.py
+-rw-r--r--   0        0        0     7183 2023-07-08 19:15:04.169133 service_markets-0.3.2/src/service_markets/api/routers/services.py
+-rw-r--r--   0        0        0     2265 2023-07-08 19:15:04.173133 service_markets-0.3.2/src/service_markets/api/routers/users.py
+-rw-r--r--   0        0        0      178 2023-07-07 14:40:33.558522 service_markets-0.3.2/src/service_markets/api/utils.py
+-rw-r--r--   0        0        0        1 2023-07-07 14:40:33.558522 service_markets-0.3.2/src/service_markets/core/__init__.py
+-rw-r--r--   0        0        0      780 2023-07-08 20:07:33.642896 service_markets-0.3.2/src/service_markets/core/constants.py
+-rw-r--r--   0        0        0     3113 2023-07-08 23:59:59.091090 service_markets-0.3.2/src/service_markets/core/heimdall.py
+-rw-r--r--   0        0        0      878 2023-07-08 15:13:58.497873 service_markets-0.3.2/src/service_markets/core/model.py
+-rw-r--r--   0        0        0     2769 2023-07-08 20:04:11.540378 service_markets-0.3.2/src/service_markets/core/session.py
+-rw-r--r--   0        0        0     1342 2023-07-07 18:59:02.549799 service_markets-0.3.2/src/service_markets/local_listener.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.562523 service_markets-0.3.2/src/service_markets/py.typed
+-rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 service_markets-0.3.2/PKG-INFO
```

### Comparing `service_markets-0.3.1/LICENSE` & `service_markets-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.1/README.md` & `service_markets-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.1/pyproject.toml` & `service_markets-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 tags = ["aleph.im", "saas", "marketplace", "cryptocurrency", "fastapi"]
 
 [tool.poetry]
 name = "service-markets"
-version = "0.3.1"
+version = "0.3.2"
 description = "Software-as-a-Service (SaaS) Marketplace with cryptocurrency payments"
 authors = ["Mike Hukiewitz <mike.hukiewitz@robotter.ai>"]
 license = "AGPL-3.0"
 readme = "README.md"
 packages = [{include = "service_markets", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `service_markets-0.3.1/src/service_markets/api/api_model.py` & `service_markets-0.3.2/src/service_markets/api/api_model.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.1/src/service_markets/api/main.py` & `service_markets-0.3.2/src/service_markets/api/main.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.1/src/service_markets/api/routers/services.py` & `service_markets-0.3.2/src/service_markets/api/routers/services.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.1/src/service_markets/api/routers/users.py` & `service_markets-0.3.2/src/service_markets/api/routers/users.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.1/src/service_markets/core/constants.py` & `service_markets-0.3.2/src/service_markets/core/constants.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.1/src/service_markets/core/heimdall.py` & `service_markets-0.3.2/src/service_markets/core/heimdall.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,18 +30,18 @@
     def __call__(self, request: Request) -> WalletAuth:
         """
         Check if the user has the given permission for the given service.
         """
         wallet_auth: WalletAuth = super().__call__(request)
         if self.cached_permissions.get(wallet_auth.address):
             return wallet_auth
-        permission_record = await Permission.filter(
+        permission_record = asyncio.get_event_loop().run_until_complete(Permission.filter(
             user_address=wallet_auth.address,
             service_id=self.service_record.item_hash,
-        ).all()
+        ).all())
         if not permission_record:
             raise HTTPException(
                 status_code=403,
                 detail="User does not have permission to access this service",
             )
         self.cached_permissions[wallet_auth.address] = permission_record
         return wallet_auth
```

### Comparing `service_markets-0.3.1/src/service_markets/core/model.py` & `service_markets-0.3.2/src/service_markets/core/model.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.1/src/service_markets/core/session.py` & `service_markets-0.3.2/src/service_markets/core/session.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.1/src/service_markets/local_listener.py` & `service_markets-0.3.2/src/service_markets/local_listener.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.1/PKG-INFO` & `service_markets-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: service-markets
-Version: 0.3.1
+Version: 0.3.2
 Summary: Software-as-a-Service (SaaS) Marketplace with cryptocurrency payments
 License: AGPL-3.0
 Author: Mike Hukiewitz
 Author-email: mike.hukiewitz@robotter.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

