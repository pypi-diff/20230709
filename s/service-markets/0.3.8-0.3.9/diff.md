# Comparing `tmp/service_markets-0.3.8.tar.gz` & `tmp/service_markets-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "service_markets-0.3.8.tar", max compression
+gzip compressed data, was "service_markets-0.3.9.tar", max compression
```

## Comparing `service_markets-0.3.8.tar` & `service_markets-0.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2023-07-07 14:40:33.550520 service_markets-0.3.8/LICENSE
--rw-r--r--   0        0        0     1898 2023-07-08 09:02:23.832368 service_markets-0.3.8/README.md
--rw-r--r--   0        0        0      918 2023-07-09 03:43:22.706422 service_markets-0.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.8/src/service_markets/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.8/src/service_markets/api/__init__.py
--rw-r--r--   0        0        0     1254 2023-07-09 02:03:07.892011 service_markets-0.3.8/src/service_markets/api/api_model.py
--rw-r--r--   0        0        0     2553 2023-07-08 15:14:04.217846 service_markets-0.3.8/src/service_markets/api/main.py
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.8/src/service_markets/api/routers/__init__.py
--rw-r--r--   0        0        0     8502 2023-07-09 02:05:32.939412 service_markets-0.3.8/src/service_markets/api/routers/services.py
--rw-r--r--   0        0        0     2265 2023-07-08 19:15:04.173133 service_markets-0.3.8/src/service_markets/api/routers/users.py
--rw-r--r--   0        0        0      178 2023-07-07 14:40:33.558522 service_markets-0.3.8/src/service_markets/api/utils.py
--rw-r--r--   0        0        0        1 2023-07-07 14:40:33.558522 service_markets-0.3.8/src/service_markets/core/__init__.py
--rw-r--r--   0        0        0      780 2023-07-08 20:07:33.642896 service_markets-0.3.8/src/service_markets/core/constants.py
--rw-r--r--   0        0        0     3245 2023-07-09 03:34:48.969946 service_markets-0.3.8/src/service_markets/core/heimdall.py
--rw-r--r--   0        0        0     1114 2023-07-09 02:03:07.900011 service_markets-0.3.8/src/service_markets/core/model.py
--rw-r--r--   0        0        0     1520 2023-07-09 02:03:07.876011 service_markets-0.3.8/src/service_markets/core/request_network.py
--rw-r--r--   0        0        0     2840 2023-07-09 03:43:22.686422 service_markets-0.3.8/src/service_markets/core/session.py
--rw-r--r--   0        0        0     1342 2023-07-07 18:59:02.549799 service_markets-0.3.8/src/service_markets/local_listener.py
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.562523 service_markets-0.3.8/src/service_markets/py.typed
--rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 service_markets-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-07 14:40:33.550520 service_markets-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1898 2023-07-08 09:02:23.832368 service_markets-0.3.9/README.md
+-rw-r--r--   0        0        0      918 2023-07-09 04:21:14.221778 service_markets-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.9/src/service_markets/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.9/src/service_markets/api/__init__.py
+-rw-r--r--   0        0        0     1254 2023-07-09 02:03:07.892011 service_markets-0.3.9/src/service_markets/api/api_model.py
+-rw-r--r--   0        0        0     2553 2023-07-08 15:14:04.217846 service_markets-0.3.9/src/service_markets/api/main.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.9/src/service_markets/api/routers/__init__.py
+-rw-r--r--   0        0        0     8502 2023-07-09 02:05:32.939412 service_markets-0.3.9/src/service_markets/api/routers/services.py
+-rw-r--r--   0        0        0     2265 2023-07-08 19:15:04.173133 service_markets-0.3.9/src/service_markets/api/routers/users.py
+-rw-r--r--   0        0        0      178 2023-07-07 14:40:33.558522 service_markets-0.3.9/src/service_markets/api/utils.py
+-rw-r--r--   0        0        0        1 2023-07-07 14:40:33.558522 service_markets-0.3.9/src/service_markets/core/__init__.py
+-rw-r--r--   0        0        0      780 2023-07-08 20:07:33.642896 service_markets-0.3.9/src/service_markets/core/constants.py
+-rw-r--r--   0        0        0     3381 2023-07-09 04:21:08.825793 service_markets-0.3.9/src/service_markets/core/heimdall.py
+-rw-r--r--   0        0        0     1114 2023-07-09 02:03:07.900011 service_markets-0.3.9/src/service_markets/core/model.py
+-rw-r--r--   0        0        0     1520 2023-07-09 02:03:07.876011 service_markets-0.3.9/src/service_markets/core/request_network.py
+-rw-r--r--   0        0        0     2840 2023-07-09 03:43:22.686422 service_markets-0.3.9/src/service_markets/core/session.py
+-rw-r--r--   0        0        0     1342 2023-07-07 18:59:02.549799 service_markets-0.3.9/src/service_markets/local_listener.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.562523 service_markets-0.3.9/src/service_markets/py.typed
+-rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 service_markets-0.3.9/PKG-INFO
```

### Comparing `service_markets-0.3.8/LICENSE` & `service_markets-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.8/README.md` & `service_markets-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.8/pyproject.toml` & `service_markets-0.3.9/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 tags = ["aleph.im", "saas", "marketplace", "cryptocurrency", "fastapi"]
 
 [tool.poetry]
 name = "service-markets"
-version = "0.3.8"
+version = "0.3.9"
 description = "Software-as-a-Service (SaaS) Marketplace with cryptocurrency payments"
 authors = ["Mike Hukiewitz <mike.hukiewitz@robotter.ai>"]
 license = "AGPL-3.0"
 readme = "README.md"
 packages = [{include = "service_markets", from = "src"}]
 
 [tool.poetry.dependencies]
@@ -18,15 +18,15 @@
 semver = "^3.0.0"
 pydantic = "^1.10.8"
 fastapi = "^0.95.1"
 aleph-sdk-python = "^0.6.0"
 aiohttp = "^3.8.4"
 aars = "^0.7.2"
 python-multipart = "^0.0.6"
-fastapi-walletauth = "^0.1.7"
+fastapi-walletauth = "^0.1.8"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 uvicorn = {extras = ["standard"], version = "^0.22.0"}
 black = "^23.3.0"
 httpx = "^0.24.1"
 pytest-cov = "^4.1.0"
```

### Comparing `service_markets-0.3.8/src/service_markets/api/api_model.py` & `service_markets-0.3.9/src/service_markets/api/api_model.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.8/src/service_markets/api/main.py` & `service_markets-0.3.9/src/service_markets/api/main.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.8/src/service_markets/api/routers/services.py` & `service_markets-0.3.9/src/service_markets/api/routers/services.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.8/src/service_markets/api/routers/users.py` & `service_markets-0.3.9/src/service_markets/api/routers/users.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.8/src/service_markets/core/constants.py` & `service_markets-0.3.9/src/service_markets/core/constants.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.8/src/service_markets/core/heimdall.py` & `service_markets-0.3.9/src/service_markets/core/heimdall.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Desc: FastAPI Depends plugin for controlling access to API endpoints
 # It will raise a 403 if the user is not allowed to access the endpoint.
 # For the first request, the Aleph network will be queried to see if the user is allowed to access the endpoint.
 import asyncio
 from typing import Optional
 
-from aars import AARS, Index
+from aars import AARS, Index, Record
 from fastapi import HTTPException, FastAPI
 from fastapi_walletauth import WalletAuth
 from fastapi_walletauth.core import SignatureChallengeTokenAuth
 from starlette.requests import Request
 from starlette.middleware.base import BaseHTTPMiddleware
 
 from .model import Permission, Service
@@ -50,14 +50,16 @@
                 detail="User does not have permission to access this service",
             )
         self.cached_permissions[wallet_auth.address] = permission_record
         return wallet_auth
 
     async def setup(self, **kwargs):
         self.aars = await initialize_aars(**kwargs)
+        print(f"Heimdall re-indexing channel {AARS.channel}")
+        await asyncio.wait_for(AARS.sync_indices(), timeout=None)
         service = await Service.filter(url=self.service_url).first()
         if not service:
             raise ValueError(
                 f"Service with url {self.service_url} is not registered on service.markets"
             )
         print(f"Service {self.service_url} successfully loaded. Heimdall is ready.")
         self.service_record = service
```

### Comparing `service_markets-0.3.8/src/service_markets/core/model.py` & `service_markets-0.3.9/src/service_markets/core/model.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.8/src/service_markets/core/request_network.py` & `service_markets-0.3.9/src/service_markets/core/request_network.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.8/src/service_markets/core/session.py` & `service_markets-0.3.9/src/service_markets/core/session.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.8/src/service_markets/local_listener.py` & `service_markets-0.3.9/src/service_markets/local_listener.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.8/PKG-INFO` & `service_markets-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: service-markets
-Version: 0.3.8
+Version: 0.3.9
 Summary: Software-as-a-Service (SaaS) Marketplace with cryptocurrency payments
 License: AGPL-3.0
 Author: Mike Hukiewitz
 Author-email: mike.hukiewitz@robotter.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyNaCl (>=1.5.0,<2.0.0)
 Requires-Dist: aars (>=0.7.2,<0.8.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: aleph-sdk-python (>=0.6.0,<0.7.0)
 Requires-Dist: base58 (>=2.1.1,<3.0.0)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
-Requires-Dist: fastapi-walletauth (>=0.1.7,<0.2.0)
+Requires-Dist: fastapi-walletauth (>=0.1.8,<0.2.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: semver (>=3.0.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # service.markets
```

