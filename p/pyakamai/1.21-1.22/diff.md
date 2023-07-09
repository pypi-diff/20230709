# Comparing `tmp/pyakamai-1.21-py3-none-any.whl.zip` & `tmp/pyakamai-1.22-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 27952 bytes, number of entries: 19
+Zip file size: 28025 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      454 b- defN 23-May-01 03:11 pyakamai/__init__.py
--rw-r--r--  2.0 unx     3821 b- defN 23-May-01 03:18 pyakamai/akamaicasemanagement.py
+-rw-r--r--  2.0 unx     3819 b- defN 23-Jul-09 12:14 pyakamai/akamaicasemanagement.py
 -rw-r--r--  2.0 unx     1473 b- defN 23-May-01 03:29 pyakamai/akamaicpcode.py
 -rw-r--r--  2.0 unx     2332 b- defN 23-Apr-30 11:30 pyakamai/akamaicps.py
 -rw-r--r--  2.0 unx     9439 b- defN 23-Jun-08 00:37 pyakamai/akamaidatastream.py
 -rw-r--r--  2.0 unx     4408 b- defN 23-Apr-30 10:57 pyakamai/akamaiedns.py
 -rw-r--r--  2.0 unx     2843 b- defN 23-Apr-30 15:28 pyakamai/akamaiehn.py
 -rw-r--r--  2.0 unx    14193 b- defN 23-May-01 03:54 pyakamai/akamaiksd1.py
 -rw-r--r--  2.0 unx     5689 b- defN 23-May-01 03:31 pyakamai/akamaiksd2.py
 -rw-r--r--  2.0 unx     2443 b- defN 23-Jul-09 11:44 pyakamai/akamailds.py
 -rw-r--r--  2.0 unx     3878 b- defN 23-Jun-08 00:38 pyakamai/akamaimsl.py
 -rw-r--r--  2.0 unx    29604 b- defN 23-Jul-04 02:23 pyakamai/akamaiproperty.py
 -rw-r--r--  2.0 unx     3506 b- defN 23-Apr-30 15:04 pyakamai/akamaipurge.py
 -rw-r--r--  2.0 unx     8058 b- defN 23-Jun-20 14:25 pyakamai/http_calls.py
 -rw-r--r--  2.0 unx     2624 b- defN 23-Jun-08 00:08 pyakamai/pyakamai.py
--rw-r--r--  2.0 unx    11111 b- defN 23-Jul-09 11:49 pyakamai-1.21.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 11:49 pyakamai-1.21.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 11:49 pyakamai-1.21.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1499 b- defN 23-Jul-09 11:49 pyakamai-1.21.dist-info/RECORD
-19 files, 107476 bytes uncompressed, 25540 bytes compressed:  76.2%
+-rw-r--r--  2.0 unx    11384 b- defN 23-Jul-09 12:19 pyakamai-1.22.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 12:19 pyakamai-1.22.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 12:19 pyakamai-1.22.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1499 b- defN 23-Jul-09 12:19 pyakamai-1.22.dist-info/RECORD
+19 files, 107747 bytes uncompressed, 25613 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: pyakamai/http_calls.py
 Comment: 
 
 Filename: pyakamai/pyakamai.py
 Comment: 
 
-Filename: pyakamai-1.21.dist-info/METADATA
+Filename: pyakamai-1.22.dist-info/METADATA
 Comment: 
 
-Filename: pyakamai-1.21.dist-info/WHEEL
+Filename: pyakamai-1.22.dist-info/WHEEL
 Comment: 
 
-Filename: pyakamai-1.21.dist-info/top_level.txt
+Filename: pyakamai-1.22.dist-info/top_level.txt
 Comment: 
 
-Filename: pyakamai-1.21.dist-info/RECORD
+Filename: pyakamai-1.22.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyakamai/akamaicasemanagement.py

```diff
@@ -33,30 +33,30 @@
         self._prdHttpCaller = prdHttpCaller
         self.accountSwitchKey = accountSwitchKey
         return None
 
     def createCase(self,caseDetailsFile):  
         fp = open(caseDetailsFile,'r')
         data = json.load(fp)
-        caseobj_json = json.dumps(caseobj)
+        caseobj_json = json.dumps(data)
 
         headers = {
             "Accept": "application/json",
             "Content-Type": "application/json"
         }
         ep = "/case-management/v2/cases"
 
         if self.accountSwitchKey:
             params = {'accountSwitchKey': self.accountSwitchKey}
             status,response = self._prdHttpCaller.postResult(ep,caseobj_json,headers=headers,params=params)
         else:
             status,response = self._prdHttpCaller.postResult(ep,caseobj_json,headers=headers)
 
         if status == 200:
-           return reponse['caseId']
+           return response['caseId']
         else:
             return ''
 
     def listmyActiveCases(self,accountIds=None,limit=50,duration=30):
         ep = '/case-management/v3/cases'
         params = {}
         if accountIds != None:
```

## Comparing `pyakamai-1.21.dist-info/METADATA` & `pyakamai-1.22.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyakamai
-Version: 1.21
+Version: 1.22
 Summary: A Boto3 like SDK for Akamai
 Home-page: https://github.com/Achuthananda/pyakamai
 Author: Achuthananda M P
 Author-email: achuthadivine@gmail.com
 Project-URL: Source, https://github.com/Achuthananda/pyakamai
 Keywords: Akamai Python CDN SDK Edge
 Classifier: Programming Language :: Python :: 3
@@ -332,7 +332,19 @@
         "method": "DELETE",
         "title": "Delete Log Configuration"
       }
     ]
   },
 
 ```
+
+## Using Akamai Case Management
+
+```
+from pyakamai import pyakamai
+import json
+pyakamaiObj = pyakamai()
+caseManagementClient = pyakamaiObj.client('case')
+caseList = caseManagementClient.listAllActiveCases(accountIds='F-AC879800')
+print(json.dumps(caseList,indent=2))
+
+```
```

## Comparing `pyakamai-1.21.dist-info/RECORD` & `pyakamai-1.22.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 pyakamai/__init__.py,sha256=JER0abqNyr-F_5XlBsXxh3NEbppAZa4pygHLoBmtMEU,454
-pyakamai/akamaicasemanagement.py,sha256=DcNQenKNSNpW4buRbb6kQPMMymyteiKTbBT165i12SE,3821
+pyakamai/akamaicasemanagement.py,sha256=WHZt-mfILmuhnOaiiuLZrXZ9gK--uICyM0DURpOod_Q,3819
 pyakamai/akamaicpcode.py,sha256=yQ31HE7krGBo_7tn8iGBwt0UtBHMM-wnTP33hwsamiI,1473
 pyakamai/akamaicps.py,sha256=6WOARWxWlkauMawOH4BE2-VJKdMgpqKdtcX8TXLKIgs,2332
 pyakamai/akamaidatastream.py,sha256=TaU8glzaoiZMdwk3n1vdzsOKAP1nWhfEBQSz0lki9F8,9439
 pyakamai/akamaiedns.py,sha256=ROh3xQjOxalGnya97FyxE-iYZgZniD8GAGH1mhwjvRs,4408
 pyakamai/akamaiehn.py,sha256=aZ2U6YG54IKP5vuQPd5GygalsJqVuEzvCnALjjszRFI,2843
 pyakamai/akamaiksd1.py,sha256=7RslIDB6oR3KA4nyC7infxXqH4Jr7dM0t3znyDfCUPI,14193
 pyakamai/akamaiksd2.py,sha256=CWo_ejWDPoyiTWROrbc_OTmcq7RXZBb8n8xOYVXQ3w8,5689
 pyakamai/akamailds.py,sha256=Rt4Lp4Hmu6T5sx0jCp3iB7YMowKSdIrk6E2NP_JWYXA,2443
 pyakamai/akamaimsl.py,sha256=ykRv_yy-qVWs37Wu2auDddX4IEuSWiO-1g9p59LTYww,3878
 pyakamai/akamaiproperty.py,sha256=jh1ooqCel03ADDtKhTOWUoW_F03ez-SH2U5iaqhF3cs,29604
 pyakamai/akamaipurge.py,sha256=FLwfjbhjn0PZyRRq68SpKFF9f8JPk76DKvCmmVg2NtU,3506
 pyakamai/http_calls.py,sha256=vH5oWXTuMtSq64crAycijH5EFQC-9QAQf--Da-qlS-I,8058
 pyakamai/pyakamai.py,sha256=xqX5Ms9Rcl4qTxkvpI5tm_AUI0qgIEyf0Jda6b-gP9c,2624
-pyakamai-1.21.dist-info/METADATA,sha256=x3nVFvOKnuDsU-qX6o0jIQu8aZdoIs5RlS3HV4LXyGI,11111
-pyakamai-1.21.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyakamai-1.21.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
-pyakamai-1.21.dist-info/RECORD,,
+pyakamai-1.22.dist-info/METADATA,sha256=cVni7SP_EXY4210bUnEaKQq__NSuJ8h7QpWqSu-G3QQ,11384
+pyakamai-1.22.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyakamai-1.22.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
+pyakamai-1.22.dist-info/RECORD,,
```

