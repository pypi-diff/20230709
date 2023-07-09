# Comparing `tmp/service_markets-0.3.2.tar.gz` & `tmp/service_markets-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "service_markets-0.3.2.tar", max compression
+gzip compressed data, was "service_markets-0.3.3.tar", max compression
```

## Comparing `service_markets-0.3.2.tar` & `service_markets-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0    34523 2023-07-07 14:40:33.550520 service_markets-0.3.2/LICENSE
--rw-r--r--   0        0        0     1898 2023-07-08 09:02:23.832368 service_markets-0.3.2/README.md
--rw-r--r--   0        0        0      918 2023-07-09 00:01:05.930639 service_markets-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.2/src/service_markets/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.2/src/service_markets/api/__init__.py
--rw-r--r--   0        0        0     1104 2023-07-08 18:56:29.117429 service_markets-0.3.2/src/service_markets/api/api_model.py
--rw-r--r--   0        0        0     2553 2023-07-08 15:14:04.217846 service_markets-0.3.2/src/service_markets/api/main.py
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.2/src/service_markets/api/routers/__init__.py
--rw-r--r--   0        0        0     7183 2023-07-08 19:15:04.169133 service_markets-0.3.2/src/service_markets/api/routers/services.py
--rw-r--r--   0        0        0     2265 2023-07-08 19:15:04.173133 service_markets-0.3.2/src/service_markets/api/routers/users.py
--rw-r--r--   0        0        0      178 2023-07-07 14:40:33.558522 service_markets-0.3.2/src/service_markets/api/utils.py
--rw-r--r--   0        0        0        1 2023-07-07 14:40:33.558522 service_markets-0.3.2/src/service_markets/core/__init__.py
--rw-r--r--   0        0        0      780 2023-07-08 20:07:33.642896 service_markets-0.3.2/src/service_markets/core/constants.py
--rw-r--r--   0        0        0     3113 2023-07-08 23:59:59.091090 service_markets-0.3.2/src/service_markets/core/heimdall.py
--rw-r--r--   0        0        0      878 2023-07-08 15:13:58.497873 service_markets-0.3.2/src/service_markets/core/model.py
--rw-r--r--   0        0        0     2769 2023-07-08 20:04:11.540378 service_markets-0.3.2/src/service_markets/core/session.py
--rw-r--r--   0        0        0     1342 2023-07-07 18:59:02.549799 service_markets-0.3.2/src/service_markets/local_listener.py
--rw-r--r--   0        0        0        0 2023-07-07 14:40:33.562523 service_markets-0.3.2/src/service_markets/py.typed
--rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 service_markets-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-07 14:40:33.550520 service_markets-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1898 2023-07-08 09:02:23.832368 service_markets-0.3.3/README.md
+-rw-r--r--   0        0        0      918 2023-07-09 03:10:59.678497 service_markets-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.3/src/service_markets/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.3/src/service_markets/api/__init__.py
+-rw-r--r--   0        0        0     1254 2023-07-09 02:03:07.892011 service_markets-0.3.3/src/service_markets/api/api_model.py
+-rw-r--r--   0        0        0     2553 2023-07-08 15:14:04.217846 service_markets-0.3.3/src/service_markets/api/main.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.554521 service_markets-0.3.3/src/service_markets/api/routers/__init__.py
+-rw-r--r--   0        0        0     8502 2023-07-09 02:05:32.939412 service_markets-0.3.3/src/service_markets/api/routers/services.py
+-rw-r--r--   0        0        0     2265 2023-07-08 19:15:04.173133 service_markets-0.3.3/src/service_markets/api/routers/users.py
+-rw-r--r--   0        0        0      178 2023-07-07 14:40:33.558522 service_markets-0.3.3/src/service_markets/api/utils.py
+-rw-r--r--   0        0        0        1 2023-07-07 14:40:33.558522 service_markets-0.3.3/src/service_markets/core/__init__.py
+-rw-r--r--   0        0        0      780 2023-07-08 20:07:33.642896 service_markets-0.3.3/src/service_markets/core/constants.py
+-rw-r--r--   0        0        0     3144 2023-07-09 03:15:10.439873 service_markets-0.3.3/src/service_markets/core/heimdall.py
+-rw-r--r--   0        0        0     1114 2023-07-09 02:03:07.900011 service_markets-0.3.3/src/service_markets/core/model.py
+-rw-r--r--   0        0        0     1520 2023-07-09 02:03:07.876011 service_markets-0.3.3/src/service_markets/core/request_network.py
+-rw-r--r--   0        0        0     2769 2023-07-08 20:04:11.540378 service_markets-0.3.3/src/service_markets/core/session.py
+-rw-r--r--   0        0        0     1342 2023-07-07 18:59:02.549799 service_markets-0.3.3/src/service_markets/local_listener.py
+-rw-r--r--   0        0        0        0 2023-07-07 14:40:33.562523 service_markets-0.3.3/src/service_markets/py.typed
+-rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 service_markets-0.3.3/PKG-INFO
```

### Comparing `service_markets-0.3.2/LICENSE` & `service_markets-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.2/README.md` & `service_markets-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.2/pyproject.toml` & `service_markets-0.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 tags = ["aleph.im", "saas", "marketplace", "cryptocurrency", "fastapi"]
 
 [tool.poetry]
 name = "service-markets"
-version = "0.3.2"
+version = "0.3.3"
 description = "Software-as-a-Service (SaaS) Marketplace with cryptocurrency payments"
 authors = ["Mike Hukiewitz <mike.hukiewitz@robotter.ai>"]
 license = "AGPL-3.0"
 readme = "README.md"
 packages = [{include = "service_markets", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `service_markets-0.3.2/src/service_markets/api/main.py` & `service_markets-0.3.3/src/service_markets/api/main.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.2/src/service_markets/api/routers/services.py` & `service_markets-0.3.3/src/service_markets/api/routers/services.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 
 from ...core.model import (
     Service,
     Permission,
     Comment,
     VoteType,
     Vote,
-    VotableType,
+    VotableType, Payment,
 )
 from ..api_model import (
     ServiceWithPermissionStatus,
     UploadServiceRequest,
     VoteServiceResponse,
-    VoteCommentResponse,
+    VoteCommentResponse, PutInvoiceServiceResponse,
 )
+from ...core.request_network import fetch_payment
 
 router = APIRouter(
     prefix="/services",
     tags=["services"],
     responses={404: {"description": "Not found"}},
 )
 
@@ -146,14 +147,50 @@
         )
     else:
         vote_record.vote = vote
     service, vote_record = await update_vote(service, vote_record)
     return VoteServiceResponse(service=service, vote=vote_record)
 
 
+@router.put("/{service_id}/payment/{tx_hash}")
+async def put_invoice_service(
+    service_id: str,
+    tx_hash: str,
+    wallet: WalletAuthDep,
+) -> PutInvoiceServiceResponse:
+    """
+    Update your payment for a given service.
+    """
+    service = await Service.fetch(service_id).first()
+    if not service:
+        raise HTTPException(status_code=404, detail="No Service found")
+    payment = await Payment.filter(txHash=tx_hash).first()
+    if payment:
+        raise HTTPException(status_code=409, detail="Payment already registered")
+    payment = await fetch_payment(tx_hash)
+    if not payment:
+        raise HTTPException(status_code=404, detail="No Payment found")
+    if payment.from_ != wallet.address:
+        raise HTTPException(
+            status_code=403,
+            detail="payment does not match currently authorized user wallet",
+        )
+    await payment.save()
+    service.payment_id = payment.item_hash
+    permission = Permission(
+        service_id=service_id,
+        user_address=wallet.address,
+    )
+    service, permission = await asyncio.gather(
+        service.save(),
+        permission.save(),
+    )
+    return PutInvoiceServiceResponse(service=service, permission=permission, payment=payment)
+
+
 @router.get("/{service_id}/comments")
 async def get_service_comments(
     service_id: str, page: int = 1, page_size: int = 20
 ) -> List[Comment]:
     """
     Get all comments for a given service.
     """
```

### Comparing `service_markets-0.3.2/src/service_markets/api/routers/users.py` & `service_markets-0.3.3/src/service_markets/api/routers/users.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.2/src/service_markets/core/constants.py` & `service_markets-0.3.3/src/service_markets/core/constants.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.2/src/service_markets/core/heimdall.py` & `service_markets-0.3.3/src/service_markets/core/heimdall.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     def __call__(self, request: Request) -> WalletAuth:
         """
         Check if the user has the given permission for the given service.
         """
         wallet_auth: WalletAuth = super().__call__(request)
         if self.cached_permissions.get(wallet_auth.address):
             return wallet_auth
-        permission_record = asyncio.get_event_loop().run_until_complete(Permission.filter(
+        loop = self.aars.session.http_session.loop
+        permission_record = loop.run_until_complete(Permission.filter(
             user_address=wallet_auth.address,
             service_id=self.service_record.item_hash,
         ).all())
         if not permission_record:
             raise HTTPException(
                 status_code=403,
                 detail="User does not have permission to access this service",
```

### Comparing `service_markets-0.3.2/src/service_markets/core/model.py` & `service_markets-0.3.3/src/service_markets/core/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from enum import Enum
 from typing import List, Optional
 
 from aars import Record
+from pydantic import Field
 
 
 class UserInfo(Record):
     username: str
     address: str
     bio: Optional[str]
     email: Optional[str]
@@ -22,14 +23,15 @@
     description: str
     url: str
     image_url: Optional[str]
     price: float
     tags: List[str]
     owner_address: str
     comment_counter: int = 0
+    payment_id: Optional[str] = None
 
 
 class VoteType(str, Enum):
     UP = "up"
     DOWN = "down"
 
 
@@ -50,7 +52,17 @@
     user_address: str
     comment: str
 
 
 class Permission(Record):
     user_address: str
     service_id: str
+
+
+class Payment(Record):
+    contractAddress: str
+    tokenAddress: str
+    txHash: str
+    to: str
+    from_: str = Field(alias='from')
+    amount: str
+    reference: str
```

### Comparing `service_markets-0.3.2/src/service_markets/core/session.py` & `service_markets-0.3.3/src/service_markets/core/session.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.2/src/service_markets/local_listener.py` & `service_markets-0.3.3/src/service_markets/local_listener.py`

 * *Files identical despite different names*

### Comparing `service_markets-0.3.2/PKG-INFO` & `service_markets-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: service-markets
-Version: 0.3.2
+Version: 0.3.3
 Summary: Software-as-a-Service (SaaS) Marketplace with cryptocurrency payments
 License: AGPL-3.0
 Author: Mike Hukiewitz
 Author-email: mike.hukiewitz@robotter.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

