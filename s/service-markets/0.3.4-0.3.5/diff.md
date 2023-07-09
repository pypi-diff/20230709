# Comparing `tmp/service_markets-0.3.4.tar.gz` & `tmp/service_markets-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "service_markets-0.3.4.tar", max compression
+gzip compressed data, was "service_markets-0.3.5.tar", max compression
```

## Comparing `service_markets-0.3.4.tar` & `service_markets-0.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2023-07-07 14:40:33.550520 service_markets-0.3.4/LICENSE
--rw-r--r--   0        0        0     1898 2023-07-08 09:02:23.832368 service_markets-0.3.4/README.md
--rw-r--r--   0        0        0      918 2023-07-09 03:26:38.297831 service_markets-0.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.4/src/service_markets/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.4/src/service_markets/api/__init__.py
--rw-r--r--   0        0        0     1254 2023-07-09 02:03:07.892011 service_markets-0.3.4/src/service_markets/api/api_model.py
--rw-r--r--   0        0        0     2553 2023-07-08 15:14:04.217846 service_markets-0.3.4/src/service_markets/api/main.py
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.4/src/service_markets/api/routers/__init__.py
--rw-r--r--   0        0        0     8502 2023-07-09 02:05:32.939412 service_markets-0.3.4/src/service_markets/api/routers/services.py
--rw-r--r--   0        0        0     2265 2023-07-08 19:15:04.173133 service_markets-0.3.4/src/service_markets/api/routers/users.py
--rw-r--r--   0        0        0      178 2023-07-07 14:40:33.558522 service_markets-0.3.4/src/service_markets/api/utils.py
--rw-r--r--   0        0        0        1 2023-07-07 14:40:33.558522 service_markets-0.3.4/src/service_markets/core/__init__.py
--rw-r--r--   0        0        0      780 2023-07-08 20:07:33.642896 service_markets-0.3.4/src/service_markets/core/constants.py
--rw-r--r--   0        0        0     3449 2023-07-09 03:26:26.473927 service_markets-0.3.4/src/service_markets/core/heimdall.py
--rw-r--r--   0        0        0     1114 2023-07-09 02:03:07.900011 service_markets-0.3.4/src/service_markets/core/model.py
--rw-r--r--   0        0        0     1520 2023-07-09 02:03:07.876011 service_markets-0.3.4/src/service_markets/core/request_network.py
--rw-r--r--   0        0        0     2769 2023-07-08 20:04:11.540378 service_markets-0.3.4/src/service_markets/core/session.py
--rw-r--r--   0        0        0     1342 2023-07-07 18:59:02.549799 service_markets-0.3.4/src/service_markets/local_listener.py
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.562523 service_markets-0.3.4/src/service_markets/py.typed
--rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 service_markets-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-07 14:40:33.550520 service_markets-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1898 2023-07-08 09:02:23.832368 service_markets-0.3.5/README.md
+-rw-r--r--   0        0        0      918 2023-07-09 03:30:47.307838 service_markets-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.5/src/service_markets/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.5/src/service_markets/api/__init__.py
+-rw-r--r--   0        0        0     1254 2023-07-09 02:03:07.892011 service_markets-0.3.5/src/service_markets/api/api_model.py
+-rw-r--r--   0        0        0     2553 2023-07-08 15:14:04.217846 service_markets-0.3.5/src/service_markets/api/main.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.5/src/service_markets/api/routers/__init__.py
+-rw-r--r--   0        0        0     8502 2023-07-09 02:05:32.939412 service_markets-0.3.5/src/service_markets/api/routers/services.py
+-rw-r--r--   0        0        0     2265 2023-07-08 19:15:04.173133 service_markets-0.3.5/src/service_markets/api/routers/users.py
+-rw-r--r--   0        0        0      178 2023-07-07 14:40:33.558522 service_markets-0.3.5/src/service_markets/api/utils.py
+-rw-r--r--   0        0        0        1 2023-07-07 14:40:33.558522 service_markets-0.3.5/src/service_markets/core/__init__.py
+-rw-r--r--   0        0        0      780 2023-07-08 20:07:33.642896 service_markets-0.3.5/src/service_markets/core/constants.py
+-rw-r--r--   0        0        0     3314 2023-07-09 03:30:42.439876 service_markets-0.3.5/src/service_markets/core/heimdall.py
+-rw-r--r--   0        0        0     1114 2023-07-09 02:03:07.900011 service_markets-0.3.5/src/service_markets/core/model.py
+-rw-r--r--   0        0        0     1520 2023-07-09 02:03:07.876011 service_markets-0.3.5/src/service_markets/core/request_network.py
+-rw-r--r--   0        0        0     2769 2023-07-08 20:04:11.540378 service_markets-0.3.5/src/service_markets/core/session.py
+-rw-r--r--   0        0        0     1342 2023-07-07 18:59:02.549799 service_markets-0.3.5/src/service_markets/local_listener.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.562523 service_markets-0.3.5/src/service_markets/py.typed
+-rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 service_markets-0.3.5/PKG-INFO
```

### Comparing `service_markets-0.3.4/LICENSE` & `service_markets-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.4/README.md` & `service_markets-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.4/pyproject.toml` & `service_markets-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 tags = ["aleph.im", "saas", "marketplace", "cryptocurrency", "fastapi"]
 
 [tool.poetry]
 name = "service-markets"
-version = "0.3.4"
+version = "0.3.5"
 description = "Software-as-a-Service (SaaS) Marketplace with cryptocurrency payments"
 authors = ["Mike Hukiewitz <mike.hukiewitz@robotter.ai>"]
 license = "AGPL-3.0"
 readme = "README.md"
 packages = [{include = "service_markets", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `service_markets-0.3.4/src/service_markets/api/api_model.py` & `service_markets-0.3.5/src/service_markets/api/api_model.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.4/src/service_markets/api/main.py` & `service_markets-0.3.5/src/service_markets/api/main.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.4/src/service_markets/api/routers/services.py` & `service_markets-0.3.5/src/service_markets/api/routers/services.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.4/src/service_markets/api/routers/users.py` & `service_markets-0.3.5/src/service_markets/api/routers/users.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.4/src/service_markets/core/constants.py` & `service_markets-0.3.5/src/service_markets/core/constants.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.4/src/service_markets/core/heimdall.py` & `service_markets-0.3.5/src/service_markets/core/heimdall.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .session import initialize_aars
 
 
 class ServicePermissionAuth(SignatureChallengeTokenAuth):
     aars: AARS
     service_record: Optional[Service] = None
     cached_permissions = {}
+    ready = False
 
     def __init__(
         self,
         service_url: str,
     ):
         super().__init__()
         self.service_url = service_url
@@ -55,29 +56,27 @@
         service = await Service.filter(url=self.service_url).first()
         if not service:
             raise ValueError(
                 f"Service with url {self.service_url} is not registered on service.markets"
             )
         print(f"Service {self.service_url} successfully loaded. Heimdall is ready.")
         self.service_record = service
+        self.ready = True
 
 
 class HeimdallMiddleware(BaseHTTPMiddleware):
     def __init__(self, app: FastAPI, backend: ServicePermissionAuth, **kwargs):
         super().__init__(app)
         self.backend = backend
         self.kwargs = kwargs
-        # setup backend
-        account = kwargs.get("account", get_fallback_account())
-        aleph_session = AuthenticatedAlephClient(account, settings.API_HOST)
-        loop = aleph_session.http_session.loop
-        loop.run_until_complete(self.backend.setup(**kwargs))
 
     async def dispatch(self, request, call_next):
         if not request.url.path.startswith("/authorization"):
+            if not self.backend.ready:
+                await self.backend.setup(**self.kwargs)
             request.state.wallet_auth = self.backend(request)
         return await call_next(request)
 
 
 def setup_heimdall(app: FastAPI, service_url: str, **kwargs):
     """
     Setup Heimdall middleware for the given app. This will check if the user has permission to access the given service.
```

### Comparing `service_markets-0.3.4/src/service_markets/core/model.py` & `service_markets-0.3.5/src/service_markets/core/model.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.4/src/service_markets/core/request_network.py` & `service_markets-0.3.5/src/service_markets/core/request_network.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.4/src/service_markets/core/session.py` & `service_markets-0.3.5/src/service_markets/core/session.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.4/src/service_markets/local_listener.py` & `service_markets-0.3.5/src/service_markets/local_listener.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.4/PKG-INFO` & `service_markets-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: service-markets
-Version: 0.3.4
+Version: 0.3.5
 Summary: Software-as-a-Service (SaaS) Marketplace with cryptocurrency payments
 License: AGPL-3.0
 Author: Mike Hukiewitz
 Author-email: mike.hukiewitz@robotter.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

