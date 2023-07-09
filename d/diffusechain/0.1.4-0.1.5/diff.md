# Comparing `tmp/diffusechain-0.1.4.tar.gz` & `tmp/diffusechain-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffusechain-0.1.4.tar", max compression
+gzip compressed data, was "diffusechain-0.1.5.tar", max compression
```

## Comparing `diffusechain-0.1.4.tar` & `diffusechain-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      233 2023-07-09 12:50:06.797797 diffusechain-0.1.4/diffusechain/__init__.py
--rw-r--r--   0        0        0    15514 2023-07-09 12:55:02.030549 diffusechain-0.1.4/diffusechain/Automatic1111.py
--rw-r--r--   0        0        0        0 2023-07-09 12:48:39.750318 diffusechain-0.1.4/diffusechain/chains/__init__.py
--rw-r--r--   0        0        0       73 2023-07-09 12:53:17.902435 diffusechain-0.1.4/diffusechain/chains/consistentFaceChain.py
--rw-r--r--   0        0        0       63 2023-07-09 12:14:22.417256 diffusechain-0.1.4/diffusechain/Diffusers.py
--rw-r--r--   0        0        0      414 2023-07-09 12:57:40.299846 diffusechain-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       15 2023-07-06 19:14:58.750868 diffusechain-0.1.4/README.md
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 diffusechain-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      233 2023-07-09 12:50:06.797797 diffusechain-0.1.5/diffusechain/__init__.py
+-rw-r--r--   0        0        0    15749 2023-07-09 13:15:20.723018 diffusechain-0.1.5/diffusechain/Automatic1111.py
+-rw-r--r--   0        0        0        0 2023-07-09 12:48:39.750318 diffusechain-0.1.5/diffusechain/chains/__init__.py
+-rw-r--r--   0        0        0       73 2023-07-09 12:53:17.902435 diffusechain-0.1.5/diffusechain/chains/consistentFaceChain.py
+-rw-r--r--   0        0        0       63 2023-07-09 12:14:22.417256 diffusechain-0.1.5/diffusechain/Diffusers.py
+-rw-r--r--   0        0        0      414 2023-07-09 13:18:58.459920 diffusechain-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       15 2023-07-06 19:14:58.750868 diffusechain-0.1.5/README.md
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 diffusechain-0.1.5/PKG-INFO
```

### Comparing `diffusechain-0.1.4/diffusechain/Automatic1111.py` & `diffusechain-0.1.5/diffusechain/Automatic1111.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,20 @@
         password=None,
     ):
         if baseurl is None:
             if use_https:
                 baseurl = f"https://{host}:{port}/sdapi/v1"
             else:
                 baseurl = f"http://{host}:{port}/sdapi/v1"
+            print(baseurl)
+        else:
+            if baseurl[-1] == "/":
+                baseurl = baseurl[:-1]
+            baseurl = f"{baseurl}/sdapi/v1"
+            print(baseurl)
 
         self.baseurl = baseurl
         self.default_sampler = sampler
         self.default_steps = steps
 
         self.session = requests.Session()
 
@@ -170,14 +176,15 @@
 
     def set_auth(self, username, password):
         self.session.auth = (username, password)
         self.check_controlnet()
 
     def _to_api_result(self, response):
         if response.status_code != 200:
+            # print(response.status_code)
             raise RuntimeError(response.status_code, response.text)
 
         r = response.json()
         images = []
         if "images" in r.keys():
             images = [Image.open(io.BytesIO(base64.b64decode(i))) for i in r["images"]]
         elif "image" in r.keys():
```

### Comparing `diffusechain-0.1.4/PKG-INFO` & `diffusechain-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffusechain
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Adithya S K
 Author-email: adithyaskolavi@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

