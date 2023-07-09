# Comparing `tmp/saic_ismart_client-1.3.0.tar.gz` & `tmp/saic_ismart_client-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client-1.3.0.tar", last modified: Sat Jun 10 09:09:14 2023, max compression
+gzip compressed data, was "saic_ismart_client-1.4.0.tar", last modified: Sun Jul  9 13:16:31 2023, max compression
```

## Comparing `saic_ismart_client-1.3.0.tar` & `saic_ismart_client-1.4.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:09:14.138620 saic_ismart_client-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-10 09:09:14.138620 saic_ismart_client-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 09:09:14.138620 saic_ismart_client-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:09:14.134620 saic_ismart_client-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:09:14.138620 saic_ismart_client-1.3.0/src/saic_ismart_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:09:14.134620 saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:09:14.138620 saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:09:14.138620 saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:09:14.138620 saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/common_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:09:14.138620 saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v1_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v1_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:09:14.138620 saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v2_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v2_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v2_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:09:14.138620 saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v3_0/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v3_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v3_0/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    29769 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/src/saic_ismart_client/saic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:09:14.138620 saic_ismart_client-1.3.0/src/saic_ismart_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-10 09:09:14.000000 saic_ismart_client-1.3.0/src/saic_ismart_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-10 09:09:14.000000 saic_ismart_client-1.3.0/src/saic_ismart_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:09:14.000000 saic_ismart_client-1.3.0/src/saic_ismart_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-10 09:09:14.000000 saic_ismart_client-1.3.0/src/saic_ismart_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-10 09:09:14.000000 saic_ismart_client-1.3.0/src/saic_ismart_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:09:14.138620 saic_ismart_client-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/tests/test_Message_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/tests/test_Message_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/tests/test_Message_v3_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/tests/test_abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-06-10 09:08:59.000000 saic_ismart_client-1.3.0/tests/test_saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.756845 saic_ismart_client-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-09 13:16:31.756845 saic_ismart_client-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:16:31.756845 saic_ismart_client-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.748845 saic_ismart_client-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.748845 saic_ismart_client-1.4.0/src/saic_ismart_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.748845 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/common_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v1_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v1_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v2_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v2_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v2_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v3_0/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v3_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23240 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v3_0/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43976 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/src/saic_ismart_client/saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-09 13:16:31.000000 saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-09 13:16:31.000000 saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:16:31.000000 saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-09 13:16:31.000000 saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-09 13:16:31.000000 saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:16:31.752845 saic_ismart_client-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/tests/test_Message_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/tests/test_Message_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/tests/test_Message_v3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/tests/test_abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-09 13:16:22.000000 saic_ismart_client-1.4.0/tests/test_saic_api.py
```

### Comparing `saic_ismart_client-1.3.0/LICENSE` & `saic_ismart_client-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/PKG-INFO` & `saic_ismart_client-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client
-Version: 1.3.0
+Version: 1.4.0
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.3.0/README.md` & `saic_ismart_client-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/pyproject.toml` & `saic_ismart_client-1.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client"
-version = "1.3.0"
+version = "1.4.0"
 authors = [
     { name = "Thomas Salm", email="saic-python-client@devtom.de"},
 ]
 dependencies = [
     "asn1tools >= 0.165.0",
     "requests >= 2.28.2",
     "urllib3 >= 1.26.14",
```

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1` & `saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1` & `saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1` & `saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,28 @@
 ApplicationDataModule
 
 DEFINITIONS
 AUTOMATIC TAGS ::= 
 BEGIN
+OTAChrgCtrlReq ::= SEQUENCE
+{
+  chrgCtrlReq INTEGER(0..255),
+  tboxV2XReq INTEGER(0..255),
+  tboxEleccLckCtrlReq INTEGER(0..255)
+}
+OTAChrgCtrlStsResp ::= SEQUENCE
+{
+  chrgCtrlDspCmd INTEGER(0..255),
+  chrgCtrlResp INTEGER(0..255),
+  bmsDsChrgCtrlDspCmd INTEGER(0..255) OPTIONAL,
+  bmsDsChrgCtrlResp INTEGER(0..255) OPTIONAL,
+  ccuEleccLckCtrlDspCmd INTEGER(0..255) OPTIONAL,
+  ccuEleccLckCtrlResp INTEGER(0..255) OPTIONAL,
+  rvcReqSts OCTET STRING(SIZE(1))
+}
 OTAChrgMangDataResp ::= SEQUENCE
 {
   bmsReserCtrlDspCmd INTEGER(0..255),
   bmsReserStHourDspCmd INTEGER(0..255),
   bmsReserStMintueDspCmd INTEGER(0..255),
   bmsReserSpHourDspCmd INTEGER(0..255),
   bmsReserSpMintueDspCmd INTEGER(0..255),
@@ -75,9 +91,72 @@
   fotaLowestVoltage INTEGER(0..255) OPTIONAL,
   mileage INTEGER(0..2147483647),
   extendedData1 INTEGER(0..2147483647) OPTIONAL,
   extendedData2 INTEGER(0..2147483647) OPTIONAL,
   extendedData3 IA5String(SIZE(0..1024)) OPTIONAL,
   extendedData4 IA5String(SIZE(0..1024)) OPTIONAL
 }
-
+OTAChrgCtrlReq ::= SEQUENCE
+{
+    chrgCtrlReq INTEGER(0..255),
+    tboxV2XReq INTEGER(0..255),
+    tboxEleccLckCtrlReq INTEGER(0..255)
+}
+OTAChrgCtrlStsResp ::= SEQUENCE
+{
+    chrgCtrlDspCmd INTEGER(0..255),
+    chrgCtrlResp INTEGER(0..255),
+    bmsDsChrgCtrlDspCmd INTEGER(0..255) OPTIONAL,
+    bmsDsChrgCtrlResp INTEGER(0..255) OPTIONAL,
+    ccuEleccLckCtrlDspCmd INTEGER(0..255) OPTIONAL,
+    ccuEleccLckCtrlResp INTEGER(0..255) OPTIONAL,
+    rvcReqSts OCTET STRING(SIZE(1)) OPTIONAL
+}
+OTAChrgRsvanReq ::= SEQUENCE
+{
+    rsvanStHour INTEGER(0..255),
+    rsvanStMintu INTEGER(0..255),
+    rsvanSpHour INTEGER(0..255),
+    rsvanSpMintu INTEGER(0..255),
+    tboxReserCtrlReq INTEGER(0..255),
+    tboxAdpPubChrgSttnReq INTEGER(0..255)
+}
+OTAChrgRsvanResp ::= SEQUENCE
+{
+    rvcReqSts OCTET STRING(SIZE(1)),
+    bmsReserCtrlDspCmd INTEGER(0..255),
+    bmsReserStHourDspCmd INTEGER(0..255),
+    bmsReserStMintueDspCmd INTEGER(0..255),
+    bmsReserSpHourDspCmd INTEGER(0..255),
+    bmsReserSpMintueDspCmd INTEGER(0..255),
+    bmsAdpPubChrgSttnDspCmd INTEGER(0..255),
+    bmsReserChrgCtrlResp INTEGER(0..255) OPTIONAL
+}
+OTAChrgSetngReq ::= SEQUENCE
+{
+    onBdChrgTrgtSOCReq INTEGER(0..255),
+    altngChrgCrntReq INTEGER(0..255),
+    tboxV2XSpSOCReq INTEGER(0..255)
+}
+OTAChrgSetngResp ::= SEQUENCE
+{
+    rvcReqSts OCTET STRING(SIZE(1)),
+    bmsOnBdChrgTrgtSOCDspCmd INTEGER(0..255),
+    bmsChrgTrgtSOCResp INTEGER(0..255),
+    bmsEstdElecRng INTEGER(0..65535),
+    bmsAltngChrgCrntDspCmd INTEGER(0..255),
+    bmsPackCrnt INTEGER(0..65535),
+    bmsAltngChrgCrntResp INTEGER(0..255),
+    imcuDschrgTrgtSOCDspCmd INTEGER(0..255) OPTIONAL,
+    imcuDschrgTrgtSOCResp INTEGER(0..255) OPTIONAL
+}
+OTAChrgHeatReq ::= SEQUENCE
+{
+    ptcHeatReq INTEGER(0..255)
+}
+OTAChrgHeatResp ::= SEQUENCE
+{
+    ptcHeatReqDspCmd INTEGER(0..255),
+    ptcHeatResp INTEGER(0..255),
+    rvcReqSts OCTET STRING(SIZE(1))
+}
 END
```

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1` & `saic_ismart_client-1.4.0/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client/abrp_api.py` & `saic_ismart_client-1.4.0/src/saic_ismart_client/abrp_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class AbrpApi:
     def __init__(self, abrp_api_key: str, abrp_user_token: str) -> None:
         self.abrp_api_key = abrp_api_key
         self.abrp_user_token = abrp_user_token
 
-    def update_abrp(self, vehicle_status: OtaRvmVehicleStatusResp25857, charge_status: OtaChrgMangDataResp) -> None:
+    def update_abrp(self, vehicle_status: OtaRvmVehicleStatusResp25857, charge_status: OtaChrgMangDataResp) -> str:
         if (
                 self.abrp_api_key is not None
                 and self.abrp_user_token is not None
                 and vehicle_status is not None
                 and charge_status is not None
         ):
             # Request
@@ -51,15 +51,15 @@
             }
 
             try:
                 response = requests.post(url=tlm_send_url, headers=headers, params={
                     'token': self.abrp_user_token,
                     'tlm': json.dumps(data)
                 })
-                print(f'ABRP: {response.content}')
+                return response.content.decode()
             except requests.exceptions.ConnectionError as ece:
                 raise AbrpApiException(f'Connection error: {ece}')
             except requests.exceptions.Timeout as et:
                 raise AbrpApiException(f'Timeout error {et}')
             except requests.exceptions.HTTPError as ehttp:
                 raise AbrpApiException(f'HTTP error {ehttp}')
             except requests.exceptions.RequestException as e:
```

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client/common_model.py` & `saic_ismart_client-1.4.0/src/saic_ismart_client/common_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v1_1/Message.py` & `saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v1_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v1_1/data_model.py` & `saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v1_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v2_1/Message.py` & `saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v2_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v2_1/data_model.py` & `saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v2_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v3_0/Message.py` & `saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v3_0/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client/ota_v3_0/data_model.py` & `saic_ismart_client-1.4.0/src/saic_ismart_client/ota_v3_0/data_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -239,7 +239,214 @@
         self.total_battery_capacity = data.get('totalBatteryCapacity')
         self.fota_lowest_voltage = data.get('fotaLowestVoltage')
         self.mileage = data.get('mileage')
         self.extended_data1 = data.get('extendedData1')
         self.extended_data2 = data.get('extendedData2')
         self.extended_data3 = data.get('extendedData3')
         self.extended_data4 = data.get('extendedData4')
+
+
+class OtaChrgCtrlReq(ApplicationData):
+    def __init__(self):
+        super().__init__('OTAChrgCtrlReq')
+        self.chrgCtrlReq = None
+        self.tboxV2XReq = None
+        self.tboxEleccLckCtrlReq = None
+
+    def get_data(self) -> dict:
+        data = {
+            'chrgCtrlReq': self.chrgCtrlReq,
+            'tboxV2XReq': self.tboxV2XReq,
+            'tboxEleccLckCtrlReq': self.tboxEleccLckCtrlReq,
+        }
+        return data
+
+    def init_from_dict(self, data: dict):
+        self.chrgCtrlReq = data.get('chrgCtrlReq')
+        self.tboxV2XReq = data.get('tboxV2XReq')
+        self.tboxEleccLckCtrlReq = data.get('tboxEleccLckCtrlReq')
+
+
+class OtaChrgCtrlStsResp(ApplicationData):
+    def __init__(self):
+        super().__init__('OTAChrgCtrlStsResp')
+        self.chrgCtrlDspCmd = None
+        self.chrgCtrlResp = None
+        self.bmsDsChrgCtrlDspCmd = None
+        self.bmsDsChrgCtrlResp = None
+        self.ccuEleccLckCtrlDspCmd = None
+        self.ccuEleccLckCtrlResp = None
+        self.rvcReqSts = None
+
+    def get_data(self) -> dict:
+        data = {
+            'chrgCtrlDspCmd': self.chrgCtrlDspCmd,
+            'chrgCtrlResp': self.chrgCtrlResp,
+        }
+        self.add_optional_field_to_data(data, 'bmsDsChrgCtrlDspCmd', self.bmsDsChrgCtrlDspCmd)
+        self.add_optional_field_to_data(data, 'bmsDsChrgCtrlResp', self.bmsDsChrgCtrlResp)
+        self.add_optional_field_to_data(data, 'ccuEleccLckCtrlDspCmd', self.ccuEleccLckCtrlDspCmd)
+        self.add_optional_field_to_data(data, 'ccuEleccLckCtrlResp', self.ccuEleccLckCtrlResp)
+        self.add_optional_field_to_data(data, 'rvcReqSts', self.rvcReqSts)
+        return data
+
+
+class OtaChrgRsvanReq(ApplicationData):
+    def __init__(self):
+        super().__init__('OTAChrgRsvanReq')
+        self.rsvanStHour = None
+        self.rsvanStMintu = None
+        self.rsvanSpHour = None
+        self.rsvanSpMintu = None
+        self.tboxReserCtrlReq = None
+        self.tboxAdpPubChrgSttnReq = None
+
+    def get_data(self) -> dict:
+        data = {
+            'rsvanStHour': self.rsvanStHour,
+            'rsvanStMintu': self.rsvanStMintu,
+            'rsvanSpHour': self.rsvanSpHour,
+            'rsvanSpMintu': self.rsvanSpMintu,
+            'tboxReserCtrlReq': self.tboxReserCtrlReq,
+            'tboxAdpPubChrgSttnReq': self.tboxAdpPubChrgSttnReq
+        }
+        return data
+
+    def init_from_dict(self, data: dict):
+        self.rsvanStHour = data.get('rsvanStHour')
+        self.rsvanStMintu = data.get('rsvanStMintu')
+        self.rsvanSpHour = data.get('rsvanSpHour')
+        self.rsvanSpMintu = data.get('rsvanSpMintu')
+        self.tboxReserCtrlReq = data.get('tboxReserCtrlReq')
+        self.tboxAdpPubChrgSttnReq = data.get('tboxAdpPubChrgSttnReq')
+
+
+class OtaChrgRsvanResp(ApplicationData):
+    def __init__(self):
+        super().__init__('OTAChrgRsvanResp')
+        self.rvcReqSts = None
+        self.bmsReserCtrlDspCmd = None
+        self.bmsReserStHourDspCmd = None
+        self.bmsReserStMintueDspCmd = None
+        self.bmsReserSpHourDspCmd = None
+        self.bmsReserSpMintueDspCmd = None
+        self.bmsAdpPubChrgSttnDspCmd = None
+        self.bmsReserChrCtrlResp = None
+
+    def get_data(self) -> dict:
+        data = {
+            'rvcReqSts': self.rvcReqSts,
+            'bmsReserCtrlDspCmd': self.bmsReserCtrlDspCmd,
+            'bmsReserStHourDspCmd': self.bmsReserStHourDspCmd,
+            'bmsReserStMintueDspCmd': self.bmsReserStMintueDspCmd,
+            'bmsReserSpHourDspCmd': self.bmsReserSpHourDspCmd,
+            'bmsReserSpMintueDspCmd': self.bmsReserSpMintueDspCmd,
+            'bmsAdpPubChrgSttnDspCmd': self.bmsAdpPubChrgSttnDspCmd,
+        }
+        self.add_optional_field_to_data(data, 'bmsReserChrCtrlResp', self.bmsReserChrCtrlResp)
+        return data
+
+    def init_from_dict(self, data: dict):
+        self.rvcReqSts = data.get('rvcReqSts')
+        self.bmsReserCtrlDspCmd = data.get('bmsReserCtrlDspCmd')
+        self.bmsReserStHourDspCmd = data.get('bmsReserStHourDspCmd')
+        self.bmsReserStMintueDspCmd = data.get('bmsReserStMintueDspCmd')
+        self.bmsReserSpHourDspCmd = data.get('bmsReserSpHourDspCmd')
+        self.bmsReserSpMintueDspCmd = data.get('bmsReserSpMintueDspCmd')
+        self.bmsAdpPubChrgSttnDspCmd = data.get('bmsAdpPubChrgSttnDspCmd')
+        self.bmsReserChrCtrlResp = data.get('bmsReserChrCtrlResp')
+
+
+class OtaChrgSetngReq(ApplicationData):
+    def __init__(self):
+        super().__init__('OTAChrgSetngReq')
+        self.onBdChrgTrgtSOCReq = None
+        self.altngChrgCrntReq = None
+        self.tboxV2XSpSOCReq = None
+
+    def get_data(self) -> dict:
+        data = {
+            'onBdChrgTrgtSOCReq': self.onBdChrgTrgtSOCReq,
+            'altngChrgCrntReq': self.altngChrgCrntReq,
+            'tboxV2XSpSOCReq': self.tboxV2XSpSOCReq
+        }
+        return data
+
+    def init_from_dict(self, data: dict):
+        self.onBdChrgTrgtSOCReq = data.get('onBdChrgTrgtSOCReq')
+        self.altngChrgCrntReq = data.get('altngChrgCrntReq')
+        self.tboxV2XSpSOCReq = data.get('tboxV2XSpSOCReq')
+
+
+class OtaChrgSetngResp(ApplicationData):
+    def __init__(self):
+        super().__init__('OTAChrgSetngResp')
+        self.rvcReqSts = None
+        self.bmsOnBdChrgTrgtSOCDspCmd = None
+        self.bmsChrgTrgtSOCResp = None
+        self.bmsEstdElecRng = None
+        self.bmsAltngChrgCrntDspCmd = None
+        self.bmsPackCrnt = None
+        self.bmsAltngChrgCrntResp = None
+        self.imcuDschrgTrgtSOCDspCmd = None
+        self.imcuDschrgTrgtSOCResp = None
+
+    def get_data(self) -> dict:
+        data = {
+            'rvcReqSts': self.rvcReqSts,
+            'bmsOnBdChrgTrgtSOCDspCmd': self.bmsOnBdChrgTrgtSOCDspCmd,
+            'bmsChrgTrgtSOCResp': self.bmsChrgTrgtSOCResp,
+            'bmsEstdElecRng': self.bmsEstdElecRng,
+            'bmsAltngChrgCrntDspCmd': self.bmsAltngChrgCrntDspCmd,
+            'bmsPackCrnt': self.bmsPackCrnt,
+            'bmsAltngChrgCrntResp': self.bmsAltngChrgCrntResp
+        }
+        self.add_optional_field_to_data(data, 'imcuDschrgTrgtSOCDspCmd', self.imcuDschrgTrgtSOCDspCmd)
+        self.add_optional_field_to_data(data, 'imcuDschrgTrgtSOCResp', self.imcuDschrgTrgtSOCResp)
+        return data
+
+    def init_from_dict(self, data: dict):
+        self.rvcReqSts = data.get('rvcReqSts')
+        self.bmsOnBdChrgTrgtSOCDspCmd = data.get('bmsOnBdChrgTrgtSOCDspCmd')
+        self.bmsChrgTrgtSOCResp = data.get('bmsChrgTrgtSOCResp')
+        self.bmsEstdElecRng = data.get('bmsEstdElecRng')
+        self.bmsAltngChrgCrntDspCmd = data.get('bmsAltngChrgCrntDspCmd')
+        self.bmsPackCrnt = data.get('bmsPackCrnt')
+        self.bmsAltngChrgCrntResp = data.get('bmsAltngChrgCrntResp')
+        self.imcuDschrgTrgtSOCDspCmd = data.get('imcuDschrgTrgtSOCDspCmd')
+        self.imcuDschrgTrgtSOCResp = data.get('imcuDschrgTrgtSOCResp')
+
+
+class OtaChrgHeatReq(ApplicationData):
+    def __init__(self):
+        super().__init__('OTAChrgHeatReq')
+        self.ptcHeatReq = None
+
+    def get_data(self) -> dict:
+        data = {
+            'ptcHeatReq': self.ptcHeatReq
+        }
+        return data
+
+    def init_from_dict(self, data: dict):
+        self.ptcHeatReq = data.get('ptcHeatReq')
+
+
+class OtaChrgHeatResp(ApplicationData):
+    def __init__(self):
+        super().__init__('OTAChrgHeatResp')
+        self.ptcHeatReqDspCmd = None
+        self.ptcHeatResp = None
+        self.rvcReqSts = None
+
+    def get_data(self) -> dict:
+        data = {
+            'ptcHeatReqDspCmd': self.ptcHeatReqDspCmd,
+            'ptcHeatResp': self.ptcHeatResp,
+            'rvcReqSts': self.rvcReqSts
+        }
+        return data
+
+    def init_from_dict(self, data: dict):
+        self.ptcHeatReqDspCmd = data.get('ptcHeatReqDspCmd')
+        self.ptcHeatResp = data.get('ptcHeatResp')
+        self.rvcReqSts = data.get('rvcReqSts')
```

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client/saic_api.py` & `saic_ismart_client-1.4.0/src/saic_ismart_client/saic_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,50 @@
 import datetime
 import hashlib
 import logging
 import time
 import urllib.parse
+from enum import Enum
 from typing import cast
 
 import requests as requests
 
-from saic_ismart_client.common_model import MessageV2, MessageBodyV2, Header, AbstractMessageBody, AbstractMessage
+from saic_ismart_client.common_model import AbstractMessage, AbstractMessageBody, Header, MessageBodyV2, MessageV2
 from saic_ismart_client.ota_v1_1.Message import MessageCoderV11
-from saic_ismart_client.ota_v1_1.data_model import VinInfo, MpUserLoggingInReq, MpUserLoggingInRsp, AlarmSwitchReq, \
-    MpAlarmSettingType, AlarmSwitch, MessageBodyV11, MessageV11, MessageListReq, StartEndNumber, MessageListResp, \
-    Timestamp, Message, AbortSendMessageReq
+from saic_ismart_client.ota_v1_1.data_model import AbortSendMessageReq, AlarmSwitch, AlarmSwitchReq, Message, \
+    MessageBodyV11, MessageListReq, MessageListResp, MessageV11, MpAlarmSettingType, MpUserLoggingInReq, \
+    MpUserLoggingInRsp, StartEndNumber, Timestamp, VinInfo
 from saic_ismart_client.ota_v2_1.Message import MessageCoderV21
-from saic_ismart_client.ota_v2_1.data_model import OtaRvmVehicleStatusReq, OtaRvmVehicleStatusResp25857, OtaRvcReq,\
-    RvcReqParam, OtaRvcStatus25857
-from saic_ismart_client.ota_v3_0.Message import MessageCoderV30, MessageV30, MessageBodyV30
-from saic_ismart_client.ota_v3_0.data_model import OtaChrgMangDataResp
+from saic_ismart_client.ota_v2_1.data_model import OtaRvcReq, OtaRvcStatus25857, OtaRvmVehicleStatusReq, \
+    OtaRvmVehicleStatusResp25857, RvcReqParam
+from saic_ismart_client.ota_v3_0.Message import MessageBodyV30, MessageCoderV30, MessageV30
+from saic_ismart_client.ota_v3_0.data_model import OtaChrgCtrlReq, OtaChrgCtrlStsResp, OtaChrgHeatReq, \
+    OtaChrgHeatResp, OtaChrgMangDataResp, OtaChrgRsvanReq, OtaChrgSetngReq, OtaChrgSetngResp, OtaChrgRsvanResp
 
 UID_INIT = '0000000000000000000000000000000000000000000000000#'
 AVG_SMS_DELIVERY_TIME = 15
 logging.basicConfig(format='%(asctime)s %(message)s', level=logging.INFO)
 
 
+class ScheduledChargingMode(Enum):
+    DISABLED = 2
+    UNTIL_CONFIGURED_SOC = 3
+    UNTIL_CONFIGURED_TIME = 1
+
+
+class TargetBatteryCode(Enum):
+    P_40 = 1
+    P_50 = 2
+    P_60 = 3
+    P_70 = 4
+    P_80 = 5
+    P_90 = 6
+    P_100 = 7
+
+
 class SaicMessage:
     def __init__(self, message_id: int, message_type: str, title: str, message_time: datetime, sender: str,
                  content: str, read_status: int, vin: str):
         self.message_id = message_id
         self.message_type = message_type
         self.title = title
         self.message_time = message_time
@@ -40,15 +58,15 @@
             return 'unknown'
         elif self.read_status == 0:
             return 'unread'
         else:
             return 'read'
 
     def get_details(self) -> str:
-        return f'ID: {self.message_id}, Time: {self.message_time}, Type: {self.message_type}, Title: {self.title}, '\
+        return f'ID: {self.message_id}, Time: {self.message_time}, Type: {self.message_type}, Title: {self.title}, ' \
             + f'Content: {self.content}, Status: {self.get_read_status_str()}, Sender: {self.sender}, VIN: {self.vin}'
 
 
 def convert(message: Message) -> SaicMessage:
     if message.content is not None:
         content = message.content.decode()
     else:
@@ -119,18 +137,24 @@
         else:
             self.uid = login_response_message.body.uid
             self.token = logging_in_rsp.token
             if logging_in_rsp.token_expiration is not None:
                 self.token_expiration = logging_in_rsp.token_expiration
         return login_response_message
 
-    def set_alarm_switches(self, alarm_switches: list) -> None:
+    def set_geofence_alarm_switch(self) -> None:
+        return self.set_alarm_switches(
+            [create_alarm_switch(MpAlarmSettingType.REGION)],
+            pin='22222222222222222222222222222222'
+        )
+
+    def set_alarm_switches(self, alarm_switches: list, pin: str = None) -> None:
         alarm_switch_req = AlarmSwitchReq()
         alarm_switch_req.alarm_switch_list = alarm_switches
-        alarm_switch_req.pin = hash_md5('123456')
+        alarm_switch_req.pin = hash_md5('123456') if pin is None else pin
 
         header = Header()
         header.protocol_version = 17
         alarm_switch_req_message = MessageV11(header, MessageBodyV11(), alarm_switch_req)
         application_id = '521'
         application_data_protocol_version = 513
         self.message_v1_1_coder.initialize_message(
@@ -176,14 +200,23 @@
         self.message_V2_1_coder.decode_response(vehicle_status_rsp_hex, vehicle_status_rsp_msg)
         self.publish_json_response(application_id, application_data_protocol_version, vehicle_status_rsp_msg.get_data())
         return vehicle_status_rsp_msg
 
     def get_vehicle_status_with_retry(self, vin_info: VinInfo) -> MessageV2:
         return self.handle_retry(self.get_vehicle_status, vin_info)
 
+    def unknown_engine_control(self, vin_info: VinInfo) -> MessageV2:
+        rvc_params = []
+        param1 = RvcReqParam()
+        param1.param_id = 16
+        param1.param_value = b'\x01'
+        rvc_params.append(param1)
+
+        return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x11', rvc_params, True)
+
     def lock_vehicle(self, vin_info: VinInfo) -> MessageV2:
         rvc_params = []
         return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x01', rvc_params, False)
 
     def unlock_vehicle(self, vin_info: VinInfo) -> MessageV2:
         rvc_params = []
         param1 = RvcReqParam()
@@ -210,174 +243,249 @@
         param5.param_id = 255
         param5.param_value = b'\x00'
         rvc_params.append(param5)
 
         return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x02', rvc_params, False)
 
     def start_rear_window_heat(self, vin_info: VinInfo) -> MessageV2:
-        rvc_params = []
-        param1 = RvcReqParam()
-        param1.param_id = 23
-        param1.param_value = b'\x01'
-        rvc_params.append(param1)
-
-        param2 = RvcReqParam()
-        param2.param_id = 255
-        param2.param_value = b'\x00'
-        rvc_params.append(param2)
-
-        return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x20', rvc_params, False)
+        return self.__control_rear_window_heat(vin_info, True)
 
     def stop_rear_window_heat(self, vin_info: VinInfo) -> MessageV2:
+        return self.__control_rear_window_heat(vin_info, False)
+
+    def __control_rear_window_heat(self, vin_info: VinInfo, enable: bool) -> MessageV2:
         rvc_params = []
         param1 = RvcReqParam()
         param1.param_id = 23
-        param1.param_value = b'\x00'
+        param1.param_value = bool_to_bit(enable)
         rvc_params.append(param1)
 
         param2 = RvcReqParam()
         param2.param_id = 255
         param2.param_value = b'\x00'
         rvc_params.append(param2)
 
         return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x20', rvc_params, False)
 
-    def start_ac(self, vin_info: VinInfo) -> MessageV2:
+    def control_heated_seats(self, vin_info: VinInfo, driver_side=True, passenger_side=True):
         rcv_params = []
         param1 = RvcReqParam()
-        param1.param_id = 19
-        param1.param_value = b'\x02'
+        param1.param_id = 17
+        param1.param_value = bool_to_bit(driver_side)
         rcv_params.append(param1)
 
         param2 = RvcReqParam()
-        param2.param_id = 20
-        param2.param_value = b'\x08'
+        param2.param_id = 18
+        param2.param_value = bool_to_bit(passenger_side)
         rcv_params.append(param2)
 
         param3 = RvcReqParam()
         param3.param_id = 255
         param3.param_value = b'\x00'
         rcv_params.append(param3)
+        return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x05', rcv_params, True)
 
-        return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x06', rcv_params, True)
-
-    def stop_ac(self, vin_info: VinInfo) -> MessageV2:
+    def start_ac(self, vin_info: VinInfo) -> MessageV2:
         rcv_params = []
         param1 = RvcReqParam()
         param1.param_id = 19
-        param1.param_value = b'\x00'
+        param1.param_value = b'\x02'
         rcv_params.append(param1)
 
         param2 = RvcReqParam()
         param2.param_id = 20
-        param2.param_value = b'\x00'
+        param2.param_value = b'\x08'
         rcv_params.append(param2)
 
         param3 = RvcReqParam()
         param3.param_id = 255
         param3.param_value = b'\x00'
         rcv_params.append(param3)
 
         return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x06', rcv_params, True)
 
+    def stop_ac(self, vin_info: VinInfo) -> MessageV2:
+        return self.control_climate(vin_info, fan_speed=0, ac_on=False, temperature_idx=0)
+
     def start_ac_blowing(self, vin_info: VinInfo) -> MessageV2:
+        return self.control_climate(vin_info, fan_speed=1, ac_on=False, temperature_idx=0)
+
+    def stop_ac_blowing(self, vin_info: VinInfo) -> MessageV2:
         rcv_params = []
         param1 = RvcReqParam()
         param1.param_id = 19
-        param1.param_value = b'\x01'
+        param1.param_value = b'\x00'
         rcv_params.append(param1)
 
         param2 = RvcReqParam()
         param2.param_id = 20
         param2.param_value = b'\x00'
         rcv_params.append(param2)
 
         param3 = RvcReqParam()
         param3.param_id = 22
-        param3.param_value = b'\x01'
+        param3.param_value = b'\x00'
         rcv_params.append(param3)
 
         param4 = RvcReqParam()
         param4.param_id = 255
         param4.param_value = b'\x00'
         rcv_params.append(param4)
 
         return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x06', rcv_params, True)
 
-    def stop_ac_blowing(self, vin_info: VinInfo) -> MessageV2:
+    def start_front_defrost(self, vin_info: VinInfo) -> MessageV2:
+        return self.control_climate(vin_info, fan_speed=5, ac_on=True, temperature_idx=8)
+
+    def stop_front_defrost(self, vin_info: VinInfo) -> MessageV2:
         rcv_params = []
         param1 = RvcReqParam()
         param1.param_id = 19
         param1.param_value = b'\x00'
         rcv_params.append(param1)
 
         param2 = RvcReqParam()
         param2.param_id = 20
-        param2.param_value = b'\x00'
+        param2.param_value = b'\x08'
         rcv_params.append(param2)
 
         param3 = RvcReqParam()
         param3.param_id = 22
         param3.param_value = b'\x00'
         rcv_params.append(param3)
 
         param4 = RvcReqParam()
         param4.param_id = 255
         param4.param_value = b'\x00'
         rcv_params.append(param4)
 
         return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x06', rcv_params, True)
 
-    def start_front_defrost(self, vin_info: VinInfo) -> MessageV2:
+    def control_climate(
+            self,
+            vin_info: VinInfo,
+            fan_speed: int = 5,
+            ac_on: bool = True,
+            temperature_idx: int = 8
+    ) -> MessageV2:
+
+        if fan_speed < 0 or fan_speed > 5:
+            raise Exception('fan_speed must be between 0 and 5')
+
+        if temperature_idx < 0 or temperature_idx > 14:
+            raise Exception('temperature_idx must be between 0 and 14')
+
+        if fan_speed == 0:
+            ac_on = False
+            temperature_idx = 8
+
         rcv_params = []
         param1 = RvcReqParam()
         param1.param_id = 19
-        param1.param_value = b'\x05'
+        param1.param_value = fan_speed.to_bytes(1, 'big')
         rcv_params.append(param1)
 
-        param2 = RvcReqParam()
-        param2.param_id = 20
-        param2.param_value = b'\x08'
-        rcv_params.append(param2)
+        if fan_speed > 0:
+            param2 = RvcReqParam()
+            param2.param_id = 20
+            param2.param_value = temperature_idx.to_bytes(1, 'big')
+            rcv_params.append(param2)
 
         param3 = RvcReqParam()
         param3.param_id = 22
-        param3.param_value = b'\x01'
+        param3.param_value = bool_to_bit(ac_on)
         rcv_params.append(param3)
 
         param4 = RvcReqParam()
         param4.param_id = 255
         param4.param_value = b'\x00'
         rcv_params.append(param4)
-
         return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x06', rcv_params, True)
 
-    def stop_front_defrost(self, vin_info: VinInfo) -> MessageV2:
+    def close_driver_window(self, vin_info: VinInfo) -> MessageV2:
         rcv_params = []
         param1 = RvcReqParam()
-        param1.param_id = 19
-        param1.param_value = b'\x00'
+        param1.param_id = 9
+        param1.param_value = b'\x01'
         rcv_params.append(param1)
 
-        param2 = RvcReqParam()
-        param2.param_id = 20
-        param2.param_value = b'\x08'
-        rcv_params.append(param2)
+        for i in [10, 11, 12, 13, 255]:
+            param = RvcReqParam()
+            param.param_id = i
+            param.param_value = b'\x00'
+            rcv_params.append(param)
 
-        param3 = RvcReqParam()
-        param3.param_id = 22
-        param3.param_value = b'\x00'
-        rcv_params.append(param3)
+        return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x03', rcv_params, False)
 
-        param4 = RvcReqParam()
-        param4.param_id = 255
-        param4.param_value = b'\x00'
-        rcv_params.append(param4)
+    def control_sunroof(self, should_open: bool, vin_info: VinInfo) -> MessageV2:
+        rcv_params = []
+        param1 = RvcReqParam()
+        param1.param_id = 8
+        param1.param_value = b'\x01'
+        rcv_params.append(param1)
 
-        return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x06', rcv_params, True)
+        for i in [9, 10, 11, 12, 255]:
+            param = RvcReqParam()
+            param.param_id = i
+            param.param_value = b'\x00'
+            rcv_params.append(param)
+
+        param = RvcReqParam()
+        param.param_id = 13
+        param.param_value = b'\x03' if should_open else b'\x00'
+        rcv_params.append(param)
+
+        return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x03', rcv_params, True)
+
+    def open_door_locks(self, vin_info: VinInfo) -> MessageV2:
+        return self.__open_vehicle_lock(vin_info, 3)
+
+    def open_tailgate(self, vin_info: VinInfo) -> MessageV2:
+        return self.__open_vehicle_lock(vin_info, 2)
+
+    def __open_vehicle_lock(self, vin_info: VinInfo, lock_id: int) -> MessageV2:
+        rcv_params = []
+
+        for i in [4, 5, 6, 255]:
+            param = RvcReqParam()
+            param.param_id = i
+            param.param_value = b'\x00'
+            rcv_params.append(param)
+
+        param1 = RvcReqParam()
+        param1.param_id = 7
+        param1.param_value = lock_id.to_bytes(1, 'big')
+        rcv_params.append(param1)
+
+        return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x02', rcv_params, False)
+
+    def find_my_car(self, vin_info: VinInfo, with_horn: bool = True, with_lights: bool = True) -> MessageV2:
+        rcv_params = []
+
+        param = RvcReqParam()
+        param.param_id = 1
+        param.param_value = b'\x01'
+        rcv_params.append(param)
+
+        param = RvcReqParam()
+        param.param_id = 2
+        param.param_value = bool_to_bit(with_horn)
+        rcv_params.append(param)
+
+        param = RvcReqParam()
+        param.param_id = 3
+        param.param_value = bool_to_bit(with_lights)
+        rcv_params.append(param)
+
+        param = RvcReqParam()
+        param.param_id = 255
+        param.param_value = b'\x00'
+        rcv_params.append(param)
+
+        return self.send_vehicle_ctrl_cmd_with_retry(vin_info, b'\x00', rcv_params, True)
 
     def send_vehicle_ctrl_cmd_with_retry(self, vin_info: VinInfo, rvc_req_type: bytes, rvc_params: list,
                                          has_app_data: bool) -> MessageV2:
         vehicle_control_cmd_rsp_msg = self.send_vehicle_control_command(vin_info, rvc_req_type, rvc_params)
 
         if has_app_data:
             while vehicle_control_cmd_rsp_msg.application_data is None:
@@ -388,17 +496,17 @@
                     time.sleep(float(AVG_SMS_DELIVERY_TIME))
 
                 event_id = vehicle_control_cmd_rsp_msg.body.event_id
                 vehicle_control_cmd_rsp_msg = self.send_vehicle_control_command(vin_info, rvc_req_type, rvc_params,
                                                                                 event_id)
         else:
             retry = 1
-            while(
-                vehicle_control_cmd_rsp_msg.body.error_message is not None
-                and retry <= 3
+            while (
+                    vehicle_control_cmd_rsp_msg.body.error_message is not None
+                    and retry <= 3
             ):
                 self.handle_error(vehicle_control_cmd_rsp_msg.body)
                 event_id = vehicle_control_cmd_rsp_msg.body.event_id
                 vehicle_control_cmd_rsp_msg = self.send_vehicle_control_command(vin_info, rvc_req_type, rvc_params,
                                                                                 event_id)
                 retry += 1
             if vehicle_control_cmd_rsp_msg.body.error_message is not None:
@@ -460,14 +568,16 @@
         self.publish_raw_response(application_id, application_data_protocol_version, vehicle_control_cmd_rsp_msg_hex)
         vehicle_control_cmd_rsp_msg = MessageV2(MessageBodyV2(), OtaRvcStatus25857())
         self.message_V2_1_coder.decode_response(vehicle_control_cmd_rsp_msg_hex, vehicle_control_cmd_rsp_msg)
         self.publish_json_response(application_id, application_data_protocol_version,
                                    vehicle_control_cmd_rsp_msg.get_data())
         return vehicle_control_cmd_rsp_msg
 
+    # CHARGING MANAGEMENT
+
     def get_charging_status(self, vin_info: VinInfo, event_id: str = None) -> MessageV30:
         chrg_mgmt_data_req_msg = MessageV30(MessageBodyV30())
         application_id = '516'
         application_data_protocol_version = 768
         self.message_V3_0_coder.initialize_message(self.uid, self.get_token(), vin_info.vin, application_id,
                                                    application_data_protocol_version, 5, chrg_mgmt_data_req_msg)
         if event_id is not None:
@@ -482,20 +592,157 @@
         self.message_V3_0_coder.decode_response(chrg_mgmt_data_rsp_hex, chrg_mgmt_data_rsp_msg)
         self.publish_json_response(application_id, application_data_protocol_version, chrg_mgmt_data_rsp_msg.get_data())
         return chrg_mgmt_data_rsp_msg
 
     def get_charging_status_with_retry(self, vin_info: VinInfo) -> MessageV30:
         return self.handle_retry(self.get_charging_status, vin_info)
 
+    def control_battery_heating(self, enable: bool, vin_info: VinInfo, event_id: str = None) -> MessageV30:
+        chrg_heat_req = OtaChrgHeatReq()
+        chrg_heat_req.ptcHeatReq = bool_to_int(enable)
+        chrg_heat_req_msg = MessageV30(MessageBodyV30(), chrg_heat_req)
+        application_id = '516'
+        application_data_protocol_version = 768
+        self.message_V3_0_coder.initialize_message(self.uid, self.get_token(), vin_info.vin, application_id,
+                                                   application_data_protocol_version, 9, chrg_heat_req_msg)
+        if event_id is not None:
+            chrg_heat_req_msg.body.event_id = event_id
+        self.publish_json_request(application_id, application_data_protocol_version, chrg_heat_req_msg.get_data())
+        chrg_heat_req_msg_hex = self.message_V3_0_coder.encode_request(chrg_heat_req_msg)
+        self.publish_raw_request(application_id, application_data_protocol_version, chrg_heat_req_msg_hex)
+        chrg_heat_rsp_msg_hex = self.send_request(chrg_heat_req_msg_hex,
+                                                  urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mpv30'))
+        self.publish_raw_response(application_id, application_data_protocol_version, chrg_heat_rsp_msg_hex)
+        chrg_heat_rsp_msg = MessageV30(MessageBodyV30(), OtaChrgHeatResp())
+        self.message_V3_0_coder.decode_response(chrg_heat_rsp_msg_hex, chrg_heat_rsp_msg)
+        self.publish_json_response(application_id, application_data_protocol_version, chrg_heat_rsp_msg.get_data())
+        return chrg_heat_rsp_msg
+
+    def control_charging_port_lock(self, unlock: bool, vin_info: VinInfo, event_id: str = None):
+        chrg_ctrl_req = OtaChrgCtrlReq()
+        chrg_ctrl_req.chrgCtrlReq = 0
+        chrg_ctrl_req.tboxV2XReq = 0
+        chrg_ctrl_req.tboxEleccLckCtrlReq = 2 if unlock else 1
+        chrg_ctrl_req_msg = MessageV30(MessageBodyV30(), chrg_ctrl_req)
+        application_id = '516'
+        application_data_protocol_version = 768
+        self.message_V3_0_coder.initialize_message(self.uid, self.get_token(), vin_info.vin, application_id,
+                                                   application_data_protocol_version, 7, chrg_ctrl_req_msg)
+        if event_id is not None:
+            chrg_ctrl_req_msg.body.event_id = event_id
+        self.publish_json_request(application_id, application_data_protocol_version, chrg_ctrl_req_msg.get_data())
+        chrg_ctrl_req_msg_hex = self.message_V3_0_coder.encode_request(chrg_ctrl_req_msg)
+        self.publish_raw_request(application_id, application_data_protocol_version, chrg_ctrl_req_msg_hex)
+        chrg_ctrl_rsp_msg_hex = self.send_request(chrg_ctrl_req_msg_hex,
+                                                  urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mpv30'))
+        self.publish_raw_response(application_id, application_data_protocol_version, chrg_ctrl_rsp_msg_hex)
+        chrg_ctrl_rsp_msg = MessageV30(MessageBodyV30(), OtaChrgCtrlStsResp())
+        self.message_V3_0_coder.decode_response(chrg_ctrl_rsp_msg_hex, chrg_ctrl_rsp_msg)
+        self.publish_json_response(application_id, application_data_protocol_version, chrg_ctrl_rsp_msg.get_data())
+        return chrg_ctrl_rsp_msg
+
+    def control_charging(self, stop_charging: bool, vin_info: VinInfo, event_id: str = None):
+        chrg_ctrl_req = OtaChrgCtrlReq()
+        chrg_ctrl_req.chrgCtrlReq = 2 if stop_charging else 1
+        chrg_ctrl_req.tboxV2XReq = 0
+        chrg_ctrl_req.tboxEleccLckCtrlReq = 0
+        chrg_ctrl_req_msg = MessageV30(MessageBodyV30(), chrg_ctrl_req)
+        application_id = '516'
+        application_data_protocol_version = 768
+        self.message_V3_0_coder.initialize_message(self.uid, self.get_token(), vin_info.vin, application_id,
+                                                   application_data_protocol_version, 7, chrg_ctrl_req_msg)
+        if event_id is not None:
+            chrg_ctrl_req_msg.body.event_id = event_id
+        self.publish_json_request(application_id, application_data_protocol_version, chrg_ctrl_req_msg.get_data())
+        chrg_ctrl_req_msg_hex = self.message_V3_0_coder.encode_request(chrg_ctrl_req_msg)
+        self.publish_raw_request(application_id, application_data_protocol_version, chrg_ctrl_req_msg_hex)
+        chrg_ctrl_rsp_msg_hex = self.send_request(chrg_ctrl_req_msg_hex,
+                                                  urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mpv30'))
+        self.publish_raw_response(application_id, application_data_protocol_version, chrg_ctrl_rsp_msg_hex)
+        chrg_ctrl_rsp_msg = MessageV30(MessageBodyV30(), OtaChrgCtrlStsResp())
+        self.message_V3_0_coder.decode_response(chrg_ctrl_rsp_msg_hex, chrg_ctrl_rsp_msg)
+        self.publish_json_response(application_id, application_data_protocol_version, chrg_ctrl_rsp_msg.get_data())
+        return chrg_ctrl_rsp_msg
+
+    def set_target_battery_soc(self, target_soc: TargetBatteryCode, vin_info: VinInfo, event_id: str = None):
+        chrg_setng_req = OtaChrgSetngReq()
+        chrg_setng_req.onBdChrgTrgtSOCReq = target_soc.value
+        chrg_setng_req.altngChrgCrntReq = 4
+        chrg_setng_req.tboxV2XSpSOCReq = 0
+        chrg_setng_req_msg = MessageV30(MessageBodyV30(), chrg_setng_req)
+        application_id = '516'
+        application_data_protocol_version = 768
+        self.message_V3_0_coder.initialize_message(self.uid, self.get_token(), vin_info.vin, application_id,
+                                                   application_data_protocol_version, 3, chrg_setng_req_msg)
+        if event_id is not None:
+            chrg_setng_req_msg.body.event_id = event_id
+        self.publish_json_request(application_id, application_data_protocol_version, chrg_setng_req_msg.get_data())
+        chrg_setng_req_msg_hex = self.message_V3_0_coder.encode_request(chrg_setng_req_msg)
+        self.publish_raw_request(application_id, application_data_protocol_version, chrg_setng_req_msg_hex)
+        chrg_setng_rsp_msg_hex = self.send_request(chrg_setng_req_msg_hex,
+                                                   urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mpv30'))
+        self.publish_raw_response(application_id, application_data_protocol_version, chrg_setng_rsp_msg_hex)
+        chrg_setng_rsp_msg = MessageV30(MessageBodyV30(), OtaChrgSetngResp())
+        self.message_V3_0_coder.decode_response(chrg_setng_rsp_msg_hex, chrg_setng_rsp_msg)
+        self.publish_json_response(application_id, application_data_protocol_version, chrg_setng_rsp_msg.get_data())
+        return chrg_setng_rsp_msg
+
+    def set_schedule_charging(self, start_time: datetime.time, end_time: datetime.time,
+                              mode: ScheduledChargingMode,
+                              vin_info: VinInfo,
+                              event_id: str = None):
+        start_hour = start_time.hour
+        start_minute = start_time.minute
+        end_hour = end_time.hour
+        end_minute = end_time.minute
+        mode_value = mode.value
+        chrg_rsvan_req = OtaChrgRsvanReq()
+        chrg_rsvan_req.rsvanStHour = start_hour
+        chrg_rsvan_req.rsvanStMintu = start_minute
+        chrg_rsvan_req.rsvanSpHour = end_hour
+        chrg_rsvan_req.rsvanSpMintu = end_minute
+        chrg_rsvan_req.tboxAdpPubChrgSttnReq = 1
+        chrg_rsvan_req.tboxReserCtrlReq = mode_value
+        chrg_rsvan_msg = MessageV30(MessageBodyV30(), chrg_rsvan_req)
+        application_id = '516'
+        application_data_protocol_version = 768
+        self.message_V3_0_coder.initialize_message(self.uid, self.get_token(), vin_info.vin, application_id,
+                                                   application_data_protocol_version, 1, chrg_rsvan_msg)
+        if event_id is not None:
+            chrg_rsvan_msg.body.event_id = event_id
+        self.publish_json_request(application_id, application_data_protocol_version, chrg_rsvan_msg.get_data())
+        chrg_rsvan_req_msg_hex = self.message_V3_0_coder.encode_request(chrg_rsvan_msg)
+        self.publish_raw_request(application_id, application_data_protocol_version, chrg_rsvan_req_msg_hex)
+        chrg_rsvan_rsp_msg_hex = self.send_request(chrg_rsvan_req_msg_hex,
+                                                   urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mpv30'))
+        self.publish_raw_response(application_id, application_data_protocol_version, chrg_rsvan_rsp_msg_hex)
+        chrg_rsvan_rsp_msg = MessageV30(MessageBodyV30(), OtaChrgRsvanResp())
+        self.message_V3_0_coder.decode_response(chrg_rsvan_rsp_msg_hex, chrg_rsvan_rsp_msg)
+        self.publish_json_response(application_id, application_data_protocol_version, chrg_rsvan_rsp_msg.get_data())
+        return chrg_rsvan_rsp_msg
+
+    # Messages
     def get_message_list(self, event_id: str = None) -> MessageV11:
+        return self.get_alarm_list(1, 5, event_id)
+
+    def get_alarm_list(self, start: int, end: int, event_id: str = None) -> MessageV11:
+        return self.__get_message_list_of_group(start, end, 'ALARM', event_id)
+
+    def get_command_list(self, start: int, end: int, event_id: str = None) -> MessageV11:
+        return self.__get_message_list_of_group(start, end, 'COMMAND', event_id)
+
+    def get_news_list(self, start: int, end: int, event_id: str = None) -> MessageV11:
+        return self.__get_message_list_of_group(start, end, 'NEWS', event_id)
+
+    def __get_message_list_of_group(self, start: int, end: int, message_group: str, event_id: str = None) -> MessageV11:
         message_list_request = MessageListReq()
         message_list_request.start_end_number = StartEndNumber()
-        message_list_request.start_end_number.start_number = 1
-        message_list_request.start_end_number.end_number = 5
-        message_list_request.message_group = 'ALARM'
+        message_list_request.start_end_number.start_number = start
+        message_list_request.start_end_number.end_number = end
+        message_list_request.message_group = message_group
 
         header = Header()
         header.protocol_version = 18
         message_body = MessageBodyV11()
         message_list_req_msg = MessageV11(header, message_body, message_list_request)
         application_id = '531'
         application_data_protocol_version = 513
@@ -510,18 +757,34 @@
                                                  urllib.parse.urljoin(self.saic_uri, '/TAP.Web/ota.mp'))
         self.publish_raw_response(application_id, application_data_protocol_version, message_list_rsp_hex)
         message_list_rsp_msg = MessageV11(header, MessageBodyV11(), MessageListResp())
         self.message_v1_1_coder.decode_response(message_list_rsp_hex, message_list_rsp_msg)
         self.publish_json_response(application_id, application_data_protocol_version, message_list_rsp_msg.get_data())
         return message_list_rsp_msg
 
-    def delete_message(self, message_id: int, event_id: str = None) -> None:
+    def delete_all_alarms(self, event_id: str = None):
+        self.__change_message_status(None, 'DELETE_ALARM', event_id)
+
+    def delete_all_commands(self, event_id: str = None):
+        self.__change_message_status(None, 'DELETE_COMMAND', event_id)
+
+    def delete_all_news(self, event_id: str = None):
+        self.__change_message_status(None, 'DELETE_NEWS', event_id)
+
+    def read_message(self, message_id: int, event_id: str = None):
+        self.__change_message_status(message_id, 'READ', event_id)
+
+    def delete_message(self, message_id: int, event_id: str = None):
+        self.__change_message_status(message_id, 'DELETE', event_id)
+
+    def __change_message_status(self, message_id: int | None, action_type: str, event_id: str = None):
         abort_send_msg_req = AbortSendMessageReq()
-        abort_send_msg_req.action_type = 'DELETE'
-        abort_send_msg_req.message_id = message_id
+        abort_send_msg_req.action_type = action_type
+        if message_id is not None:
+            abort_send_msg_req.message_id = message_id
 
         header = Header()
         header.protocol_version = 17
         message_body = MessageBodyV11()
         message_delete_req_msg = MessageV11(header, message_body, abort_send_msg_req)
         application_id = '615'
         application_protocol_version = 513
@@ -597,18 +860,18 @@
         if self.token_expiration is not None:
             token_expiration = cast(Timestamp, self.token_expiration)
             if token_expiration.get_timestamp() < datetime.datetime.now():
                 self.login()
         return self.token
 
     def handle_error(self, message_body: AbstractMessageBody):
-        message = f'application ID: {message_body.application_id},'\
-              + f' protocol version: {message_body.application_data_protocol_version},'\
-              + f' message: {message_body.error_message.decode()}'\
-              + f' result code: {message_body.result}'
+        message = f'application ID: {message_body.application_id},' \
+                  + f' protocol version: {message_body.application_data_protocol_version},' \
+                  + f' message: {message_body.error_message.decode()}' \
+                  + f' result code: {message_body.result}'
 
         if message_body.result == 2:
             # re-login
             logging.debug(message)
             if self.relogin_delay > 0:
                 logging.warning(f'The SAIC user has been logged out. '
                                 + f'Waiting {self.relogin_delay} seconds before attempting another login')
@@ -620,14 +883,22 @@
             time.sleep(float(AVG_SMS_DELIVERY_TIME))
         elif message_body.result == -1:
             logging.warning(message)
         else:
             logging.error(message)
 
 
+def bool_to_bit(flag):
+    return b'\x01' if flag else b'\x00'
+
+
+def bool_to_int(flag):
+    return 1 if flag else 0
+
+
 def hash_md5(password: str) -> str:
     return hashlib.md5(password.encode('utf-8')).hexdigest()
 
 
 def create_alarm_switch(alarm_setting_type: MpAlarmSettingType) -> AlarmSwitch:
     alarm_switch = AlarmSwitch()
     alarm_switch.alarm_setting_type = alarm_setting_type.value
```

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client.egg-info/PKG-INFO` & `saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic-ismart-client
-Version: 1.3.0
+Version: 1.4.0
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.3.0/src/saic_ismart_client.egg-info/SOURCES.txt` & `saic_ismart_client-1.4.0/src/saic_ismart_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/tests/test_Message_v1_1.py` & `saic_ismart_client-1.4.0/tests/test_Message_v1_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/tests/test_Message_v2_1.py` & `saic_ismart_client-1.4.0/tests/test_Message_v2_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/tests/test_Message_v3_0.py` & `saic_ismart_client-1.4.0/tests/test_Message_v3_0.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/tests/test_abrp_api.py` & `saic_ismart_client-1.4.0/tests/test_abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.3.0/tests/test_saic_api.py` & `saic_ismart_client-1.4.0/tests/test_saic_api.py`

 * *Files identical despite different names*

