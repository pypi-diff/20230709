# Comparing `tmp/pyakamai-1.2-py3-none-any.whl.zip` & `tmp/pyakamai-1.21-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 27953 bytes, number of entries: 19
+Zip file size: 27952 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      454 b- defN 23-May-01 03:11 pyakamai/__init__.py
 -rw-r--r--  2.0 unx     3821 b- defN 23-May-01 03:18 pyakamai/akamaicasemanagement.py
 -rw-r--r--  2.0 unx     1473 b- defN 23-May-01 03:29 pyakamai/akamaicpcode.py
 -rw-r--r--  2.0 unx     2332 b- defN 23-Apr-30 11:30 pyakamai/akamaicps.py
 -rw-r--r--  2.0 unx     9439 b- defN 23-Jun-08 00:37 pyakamai/akamaidatastream.py
 -rw-r--r--  2.0 unx     4408 b- defN 23-Apr-30 10:57 pyakamai/akamaiedns.py
 -rw-r--r--  2.0 unx     2843 b- defN 23-Apr-30 15:28 pyakamai/akamaiehn.py
@@ -10,12 +10,12 @@
 -rw-r--r--  2.0 unx     5689 b- defN 23-May-01 03:31 pyakamai/akamaiksd2.py
 -rw-r--r--  2.0 unx     2443 b- defN 23-Jul-09 11:44 pyakamai/akamailds.py
 -rw-r--r--  2.0 unx     3878 b- defN 23-Jun-08 00:38 pyakamai/akamaimsl.py
 -rw-r--r--  2.0 unx    29604 b- defN 23-Jul-04 02:23 pyakamai/akamaiproperty.py
 -rw-r--r--  2.0 unx     3506 b- defN 23-Apr-30 15:04 pyakamai/akamaipurge.py
 -rw-r--r--  2.0 unx     8058 b- defN 23-Jun-20 14:25 pyakamai/http_calls.py
 -rw-r--r--  2.0 unx     2624 b- defN 23-Jun-08 00:08 pyakamai/pyakamai.py
--rw-r--r--  2.0 unx    11111 b- defN 23-Jul-09 11:47 pyakamai-1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 11:47 pyakamai-1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 11:47 pyakamai-1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1495 b- defN 23-Jul-09 11:47 pyakamai-1.2.dist-info/RECORD
-19 files, 107472 bytes uncompressed, 25549 bytes compressed:  76.2%
+-rw-r--r--  2.0 unx    11111 b- defN 23-Jul-09 11:49 pyakamai-1.21.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 11:49 pyakamai-1.21.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 11:49 pyakamai-1.21.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1499 b- defN 23-Jul-09 11:49 pyakamai-1.21.dist-info/RECORD
+19 files, 107476 bytes uncompressed, 25540 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: pyakamai/http_calls.py
 Comment: 
 
 Filename: pyakamai/pyakamai.py
 Comment: 
 
-Filename: pyakamai-1.2.dist-info/METADATA
+Filename: pyakamai-1.21.dist-info/METADATA
 Comment: 
 
-Filename: pyakamai-1.2.dist-info/WHEEL
+Filename: pyakamai-1.21.dist-info/WHEEL
 Comment: 
 
-Filename: pyakamai-1.2.dist-info/top_level.txt
+Filename: pyakamai-1.21.dist-info/top_level.txt
 Comment: 
 
-Filename: pyakamai-1.2.dist-info/RECORD
+Filename: pyakamai-1.21.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyakamai-1.2.dist-info/METADATA` & `pyakamai-1.21.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyakamai
-Version: 1.2
+Version: 1.21
 Summary: A Boto3 like SDK for Akamai
 Home-page: https://github.com/Achuthananda/pyakamai
 Author: Achuthananda M P
 Author-email: achuthadivine@gmail.com
 Project-URL: Source, https://github.com/Achuthananda/pyakamai
 Keywords: Akamai Python CDN SDK Edge
 Classifier: Programming Language :: Python :: 3
@@ -145,15 +145,15 @@
 >>> print(purgeClient.deletebyCacheTag(['acmpjs','acmpimages'],'staging'))
 {'httpStatus': 201, 'detail': 'Request accepted', 'supportId': 'edts-NhiHSoKVaXULwJj9eS48EU', 'purgeId': 'edts-NhiHSoKVaXULwJj9eS48EU', 'estimatedSeconds': 5}
 >>> print(purgeClient.invalidatebyCacheTag(['acmpjs','acmpimages'],'production'))
 {'httpStatus': 201, 'detail': 'Request accepted', 'supportId': 'eitp-PYjibvc6uyRKcM31gn5GxY', 'purgeId': 'eitp-PYjibvc6uyRKcM31gn5GxY', 'estimatedSeconds': 5}
 ```
 
 ## Using Akamai CPS
-'''
+```
 >>> from pyakamai import pyakamai
 >>> pyakamaiObj = pyakamai('B-3-16OEUPX') 
 >>> cpsClient = pyakamaiObj.client('cps')
 >>> 
 >>> 
 >>> enrollments = cpsClient.listEnrollments()
 
@@ -172,16 +172,15 @@
         "geography": "core",
         "secureNetwork": "enhanced-tls",
         "mustHaveCiphers": "ak-akamai-2020q1",
         "preferredCiphers": "ak-akamai-2020q1",
         "disallowedTlsVersions": [
           "TLSv1",
           "TLSv1_1"]}}]}
-'''
-
+```
 
 ## Using Akamai LDS
 
 ```
 >>> from pyakamai import pyakamai
 >>> pyakamaiObj = pyakamai('B-3-16OEUPX') 
 >>> ldsClient = pyakamaiObj.client('lds')
```

## Comparing `pyakamai-1.2.dist-info/RECORD` & `pyakamai-1.21.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 pyakamai/akamaiksd2.py,sha256=CWo_ejWDPoyiTWROrbc_OTmcq7RXZBb8n8xOYVXQ3w8,5689
 pyakamai/akamailds.py,sha256=Rt4Lp4Hmu6T5sx0jCp3iB7YMowKSdIrk6E2NP_JWYXA,2443
 pyakamai/akamaimsl.py,sha256=ykRv_yy-qVWs37Wu2auDddX4IEuSWiO-1g9p59LTYww,3878
 pyakamai/akamaiproperty.py,sha256=jh1ooqCel03ADDtKhTOWUoW_F03ez-SH2U5iaqhF3cs,29604
 pyakamai/akamaipurge.py,sha256=FLwfjbhjn0PZyRRq68SpKFF9f8JPk76DKvCmmVg2NtU,3506
 pyakamai/http_calls.py,sha256=vH5oWXTuMtSq64crAycijH5EFQC-9QAQf--Da-qlS-I,8058
 pyakamai/pyakamai.py,sha256=xqX5Ms9Rcl4qTxkvpI5tm_AUI0qgIEyf0Jda6b-gP9c,2624
-pyakamai-1.2.dist-info/METADATA,sha256=i1uHYBsIRi6GMRnlGJkMbuWSHDdhQhf3TBwjXpMorxg,11111
-pyakamai-1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyakamai-1.2.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
-pyakamai-1.2.dist-info/RECORD,,
+pyakamai-1.21.dist-info/METADATA,sha256=x3nVFvOKnuDsU-qX6o0jIQu8aZdoIs5RlS3HV4LXyGI,11111
+pyakamai-1.21.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyakamai-1.21.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
+pyakamai-1.21.dist-info/RECORD,,
```

