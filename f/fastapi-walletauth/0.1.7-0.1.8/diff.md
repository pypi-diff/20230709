# Comparing `tmp/fastapi_walletauth-0.1.7.tar.gz` & `tmp/fastapi_walletauth-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_walletauth-0.1.7.tar", max compression
+gzip compressed data, was "fastapi_walletauth-0.1.8.tar", max compression
```

## Comparing `fastapi_walletauth-0.1.7.tar` & `fastapi_walletauth-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2542 2023-07-08 17:11:36.202319 fastapi_walletauth-0.1.7/README.md
--rw-r--r--   0        0        0      102 2023-07-08 13:39:37.701784 fastapi_walletauth-0.1.7/fastapi_walletauth/__init__.py
--rw-r--r--   0        0        0     7550 2023-07-08 17:10:36.198803 fastapi_walletauth-0.1.7/fastapi_walletauth/core.py
--rw-r--r--   0        0        0     1993 2023-07-08 12:27:15.855722 fastapi_walletauth-0.1.7/fastapi_walletauth/router.py
--rw-r--r--   0        0        0     2616 2023-07-08 12:19:55.853248 fastapi_walletauth-0.1.7/fastapi_walletauth/verification.py
--rw-r--r--   0        0        0     1025 2023-07-08 17:10:36.178803 fastapi_walletauth-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3684 1970-01-01 00:00:00.000000 fastapi_walletauth-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     2542 2023-07-08 17:11:36.202319 fastapi_walletauth-0.1.8/README.md
+-rw-r--r--   0        0        0      102 2023-07-08 13:39:37.701784 fastapi_walletauth-0.1.8/fastapi_walletauth/__init__.py
+-rw-r--r--   0        0        0     7555 2023-07-09 04:05:47.598404 fastapi_walletauth-0.1.8/fastapi_walletauth/core.py
+-rw-r--r--   0        0        0     1993 2023-07-08 12:27:15.855722 fastapi_walletauth-0.1.8/fastapi_walletauth/router.py
+-rw-r--r--   0        0        0     2616 2023-07-08 12:19:55.853248 fastapi_walletauth-0.1.8/fastapi_walletauth/verification.py
+-rw-r--r--   0        0        0     1025 2023-07-09 04:05:47.586404 fastapi_walletauth-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3684 1970-01-01 00:00:00.000000 fastapi_walletauth-0.1.8/PKG-INFO
```

### Comparing `fastapi_walletauth-0.1.7/README.md` & `fastapi_walletauth-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_walletauth-0.1.7/fastapi_walletauth/core.py` & `fastapi_walletauth-0.1.8/fastapi_walletauth/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     def clear_expired(cls):
         now = int(time.time())
         for challenge in cls.__challenges.values():
             if now > challenge.valid_til:
                 cls.remove_auth(challenge)
 
     @classmethod
-    def refresh_token(cls, token: str, ttl: int = 60 * 60):
+    def refresh_token(cls, token: str, ttl: int = 24 * 60 * 60):
         auth = cls.__auths.get(token)
         if not auth:
             raise NotAuthorizedError("Not authorized")
         if auth.expired:
             raise TimeoutError("Token expired")
         auth.refresh_token(ttl)
         return auth
```

### Comparing `fastapi_walletauth-0.1.7/fastapi_walletauth/router.py` & `fastapi_walletauth-0.1.8/fastapi_walletauth/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_walletauth-0.1.7/fastapi_walletauth/verification.py` & `fastapi_walletauth-0.1.8/fastapi_walletauth/verification.py`

 * *Files identical despite different names*

### Comparing `fastapi_walletauth-0.1.7/pyproject.toml` & `fastapi_walletauth-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-walletauth"
-version = "0.1.7"
+version = "0.1.8"
 description = "FastAPI extension for user authentication through signature challenges"
 authors = ["mhh <mike.hukiewitz@robotter.ai>"]
 readme = "README.md"
 packages = [{include = "fastapi_walletauth"}]
 keywords = ["FastAPI", "authentication", "signature", "wallet", "ethereum", "solana", "web3"]
 classifiers = [
     "Environment :: Web Environment",
```

### Comparing `fastapi_walletauth-0.1.7/PKG-INFO` & `fastapi_walletauth-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-walletauth
-Version: 0.1.7
+Version: 0.1.8
 Summary: FastAPI extension for user authentication through signature challenges
 Keywords: FastAPI,authentication,signature,wallet,ethereum,solana,web3
 Author: mhh
 Author-email: mike.hukiewitz@robotter.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

