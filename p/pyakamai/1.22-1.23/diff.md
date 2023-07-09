# Comparing `tmp/pyakamai-1.22-py3-none-any.whl.zip` & `tmp/pyakamai-1.23-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 28025 bytes, number of entries: 19
+Zip file size: 28266 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      454 b- defN 23-May-01 03:11 pyakamai/__init__.py
 -rw-r--r--  2.0 unx     3819 b- defN 23-Jul-09 12:14 pyakamai/akamaicasemanagement.py
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
--rw-r--r--  2.0 unx    11384 b- defN 23-Jul-09 12:19 pyakamai-1.22.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 12:19 pyakamai-1.22.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 12:19 pyakamai-1.22.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1499 b- defN 23-Jul-09 12:19 pyakamai-1.22.dist-info/RECORD
-19 files, 107747 bytes uncompressed, 25613 bytes compressed:  76.2%
+-rw-r--r--  2.0 unx    12832 b- defN 23-Jul-09 14:37 pyakamai-1.23.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 14:37 pyakamai-1.23.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 14:37 pyakamai-1.23.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1499 b- defN 23-Jul-09 14:37 pyakamai-1.23.dist-info/RECORD
+19 files, 109195 bytes uncompressed, 25854 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: pyakamai/http_calls.py
 Comment: 
 
 Filename: pyakamai/pyakamai.py
 Comment: 
 
-Filename: pyakamai-1.22.dist-info/METADATA
+Filename: pyakamai-1.23.dist-info/METADATA
 Comment: 
 
-Filename: pyakamai-1.22.dist-info/WHEEL
+Filename: pyakamai-1.23.dist-info/WHEEL
 Comment: 
 
-Filename: pyakamai-1.22.dist-info/top_level.txt
+Filename: pyakamai-1.23.dist-info/top_level.txt
 Comment: 
 
-Filename: pyakamai-1.22.dist-info/RECORD
+Filename: pyakamai-1.23.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyakamai-1.22.dist-info/METADATA` & `pyakamai-1.23.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyakamai
-Version: 1.22
+Version: 1.23
 Summary: A Boto3 like SDK for Akamai
 Home-page: https://github.com/Achuthananda/pyakamai
 Author: Achuthananda M P
 Author-email: achuthadivine@gmail.com
 Project-URL: Source, https://github.com/Achuthananda/pyakamai
 Keywords: Akamai Python CDN SDK Edge
 Classifier: Programming Language :: Python :: 3
@@ -57,31 +57,76 @@
 # Using pyakamai
 
 ## Using AkamaiProperty
 
 ### Print Hostnames
 ```
 >>> from pyakamai import pyakamai
+>>> pyakamaiObj = pyakamai()
 >>> akamaiconfig = pyakamaiObj.client('property')
 >>> akamaiconfig.config('test_bulkseach_update_1')
 >>> hostnamesList = akamaiconfig.getHostNames(akamaiconfig.getProductionVersion())
->>> for hostname in hostnamesList:
->>>     print(hostname)
+>>> print(hostnamesList)
+>>> ['www.achuth-purgetest.edgesuite-staging.net', 'www.achuth-purgetest.edgesuite.net', 'www.geethapriya-purge.edgesuite-staging.net', 'www.geethapriya-purge.edgesuite.net']
 ```
 
 ### Print Basic Information
 ```
 >>> akamaiconfig.printPropertyInfo()
 Property Name: test_bulkseach_update_1
 Contract Id: ctr_C-1IE2OHM
 Group Id: grp_163363
 Active Staging Version: 18
 Active Production Version: 18
 ```
 
+### Get the Delivery Product
+```
+>>> from pyakamai import pyakamai
+>>> pyakamaiObj = pyakamai()
+>>> akamaiconfig = pyakamaiObj.client('property')
+>>> akamaiconfig.config('achuth-purgetest.com')
+>>> version = akamaiconfig.getProductionVersion()
+>>> 
+>>> product = akamaiconfig.getProduct()
+>>> print(product)
+Dynamic Site Accelerator
+```
+
+### List the CP Codes of the Config
+```
+>>> from pyakamai import pyakamai
+>>> pyakamaiObj = pyakamai()
+>>> akamaiconfig = pyakamaiObj.client('property')
+>>> akamaiconfig.config('achuth-purgetest.com')
+>>> akamaiconfig.getCPCodes(akamaiconfig.getProductionVersion())
+[912248,566814,4512345,127890]
+```
+
+### List the Origins of the Config
+```
+>>> from pyakamai import pyakamai
+>>> pyakamaiObj = pyakamai()
+>>> akamaiconfig = pyakamaiObj.client('property')
+>>> akamaiconfig.config('achuth-purgetest.com')
+>>> akamaiconfig.getOrigins(akamaiconfig.getProductionVersion())
+['www.gsshappylearning.com','gssflowershop.com','origin-acmp.requestcatcher.com']
+```
+
+### To Search a hostname in the Account
+```
+>>> from pyakamai import pyakamai
+>>> pyakamaiObj = pyakamai() 
+>>> akamaiconfig = pyakamaiObj.client('property')
+>>> configName = akamaiconfig.search('www.achuth-purgetest.edgesuite.net')
+>>> print(configName)
+>>> achuth-purgetest.com
+```
+
+
 ### Create a new version
 ```
 >>> akamaiconfig.createVersion(18)
 '78'
 ```
 
 ### Get rule Tree
```

## Comparing `pyakamai-1.22.dist-info/RECORD` & `pyakamai-1.23.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 pyakamai/akamaiksd2.py,sha256=CWo_ejWDPoyiTWROrbc_OTmcq7RXZBb8n8xOYVXQ3w8,5689
 pyakamai/akamailds.py,sha256=Rt4Lp4Hmu6T5sx0jCp3iB7YMowKSdIrk6E2NP_JWYXA,2443
 pyakamai/akamaimsl.py,sha256=ykRv_yy-qVWs37Wu2auDddX4IEuSWiO-1g9p59LTYww,3878
 pyakamai/akamaiproperty.py,sha256=jh1ooqCel03ADDtKhTOWUoW_F03ez-SH2U5iaqhF3cs,29604
 pyakamai/akamaipurge.py,sha256=FLwfjbhjn0PZyRRq68SpKFF9f8JPk76DKvCmmVg2NtU,3506
 pyakamai/http_calls.py,sha256=vH5oWXTuMtSq64crAycijH5EFQC-9QAQf--Da-qlS-I,8058
 pyakamai/pyakamai.py,sha256=xqX5Ms9Rcl4qTxkvpI5tm_AUI0qgIEyf0Jda6b-gP9c,2624
-pyakamai-1.22.dist-info/METADATA,sha256=cVni7SP_EXY4210bUnEaKQq__NSuJ8h7QpWqSu-G3QQ,11384
-pyakamai-1.22.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyakamai-1.22.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
-pyakamai-1.22.dist-info/RECORD,,
+pyakamai-1.23.dist-info/METADATA,sha256=e7QkyVwzQhKfSsXKTXOYyNzKkQfP6HbeZaZx2KEnrdc,12832
+pyakamai-1.23.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyakamai-1.23.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
+pyakamai-1.23.dist-info/RECORD,,
```

