# Comparing `tmp/saic_ismart_client-1.4.0.tar.gz` & `tmp/saic_ismart_client-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client-1.4.0.tar", last modified: Sun Jul  9 13:16:31 2023, max compression
+gzip compressed data, was "saic_ismart_client-1.4.1.tar", last modified: Sun Jul  9 13:43:24 2023, max compression
```

## Comparing `saic_ismart_client-1.4.0.tar` & `saic_ismart_client-1.4.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.756845 saic_ismart_client-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-09 13:16:31.756845 saic_ismart_client-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:16:31.756845 saic_ismart_client-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.748845 saic_ismart_client-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.748845 saic_ismart_client-1.4.0/src/saic_ismart_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.748845 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/common_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v1_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v1_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v2_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v2_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v2_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v3_0/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v3_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23240 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v3_0/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    43976 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/saic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-09 13:16:31.000000 saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-09 13:16:31.000000 saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:16:31.000000 saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-09 13:16:31.000000 saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-09 13:16:31.000000 saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/tests/test_Message_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/tests/test_Message_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/tests/test_Message_v3_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/tests/test_abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/tests/test_saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.787799 saic_ismart_client-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.787799 saic_ismart_client-1.4.1/src/saic_ismart_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.787799 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.787799 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/common_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v1_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v1_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v2_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v2_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v2_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v3_0/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v3_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23240 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v3_0/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43976 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/src/saic_ismart_client/saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.787799 saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-09 13:43:24.000000 saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-09 13:43:24.000000 saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:43:24.000000 saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-09 13:43:24.000000 saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-09 13:43:24.000000 saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:43:24.791799 saic_ismart_client-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/tests/test_Message_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/tests/test_Message_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/tests/test_Message_v3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/tests/test_abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-09 13:43:15.000000 saic_ismart_client-1.4.1/tests/test_saic_api.py
```

### Comparing `saic_ismart_client-1.4.0/LICENSE` & `saic_ismart_client-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/PKG-INFO` & `saic_ismart_client-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client
-Version: 1.4.0
+Version: 1.4.1
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.4.0/README.md` & `saic_ismart_client-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/pyproject.toml` & `saic_ismart_client-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
     { name = "Thomas Salm", email="saic-python-client@devtom.de"},
 ]
 dependencies = [
     "asn1tools >= 0.165.0",
     "requests >= 2.28.2",
     "urllib3 >= 1.26.14",
```

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1` & `saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1` & `saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1` & `saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,12 @@
 ApplicationDataModule
 
 DEFINITIONS
 AUTOMATIC TAGS ::= 
 BEGIN
-OTAChrgCtrlReq ::= SEQUENCE
-{
-  chrgCtrlReq INTEGER(0..255),
-  tboxV2XReq INTEGER(0..255),
-  tboxEleccLckCtrlReq INTEGER(0..255)
-}
-OTAChrgCtrlStsResp ::= SEQUENCE
-{
-  chrgCtrlDspCmd INTEGER(0..255),
-  chrgCtrlResp INTEGER(0..255),
-  bmsDsChrgCtrlDspCmd INTEGER(0..255) OPTIONAL,
-  bmsDsChrgCtrlResp INTEGER(0..255) OPTIONAL,
-  ccuEleccLckCtrlDspCmd INTEGER(0..255) OPTIONAL,
-  ccuEleccLckCtrlResp INTEGER(0..255) OPTIONAL,
-  rvcReqSts OCTET STRING(SIZE(1))
-}
 OTAChrgMangDataResp ::= SEQUENCE
 {
   bmsReserCtrlDspCmd INTEGER(0..255),
   bmsReserStHourDspCmd INTEGER(0..255),
   bmsReserStMintueDspCmd INTEGER(0..255),
   bmsReserSpHourDspCmd INTEGER(0..255),
   bmsReserSpMintueDspCmd INTEGER(0..255),
```

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.1/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client/abrp_api.py` & `saic_ismart_client-1.4.1/src/saic_ismart_client/abrp_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,16 @@
                 raise AbrpApiException(f'Connection error: {ece}')
             except requests.exceptions.Timeout as et:
                 raise AbrpApiException(f'Timeout error {et}')
             except requests.exceptions.HTTPError as ehttp:
                 raise AbrpApiException(f'HTTP error {ehttp}')
             except requests.exceptions.RequestException as e:
                 raise AbrpApiException(f'{e}')
+        else:
+            return 'ABRP request skipped because of missing configuration'
 
     @staticmethod
     def __extract_basic_vehicle_status(basic_vehicle_status: RvsBasicStatus25857) -> dict:
         data = {}
 
         exterior_temperature = basic_vehicle_status.exterior_temperature
         if exterior_temperature is not None and exterior_temperature != -128:
```

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client/common_model.py` & `saic_ismart_client-1.4.1/src/saic_ismart_client/common_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v1_1/Message.py` & `saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v1_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v1_1/data_model.py` & `saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v1_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v2_1/Message.py` & `saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v2_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v2_1/data_model.py` & `saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v2_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v3_0/Message.py` & `saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v3_0/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v3_0/data_model.py` & `saic_ismart_client-1.4.1/src/saic_ismart_client/ota_v3_0/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client/saic_api.py` & `saic_ismart_client-1.4.1/src/saic_ismart_client/saic_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/PKG-INFO` & `saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic-ismart-client
-Version: 1.4.0
+Version: 1.4.1
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/SOURCES.txt` & `saic_ismart_client-1.4.1/src/saic_ismart_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/tests/test_Message_v1_1.py` & `saic_ismart_client-1.4.1/tests/test_Message_v1_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/tests/test_Message_v2_1.py` & `saic_ismart_client-1.4.1/tests/test_Message_v2_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/tests/test_Message_v3_0.py` & `saic_ismart_client-1.4.1/tests/test_Message_v3_0.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/tests/test_abrp_api.py` & `saic_ismart_client-1.4.1/tests/test_abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.4.0/tests/test_saic_api.py` & `saic_ismart_client-1.4.1/tests/test_saic_api.py`

 * *Files identical despite different names*

