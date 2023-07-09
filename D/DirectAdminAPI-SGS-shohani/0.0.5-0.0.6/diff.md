# Comparing `tmp/directadminapi_sgs_shohani-0.0.5.tar.gz` & `tmp/directadminapi_sgs_shohani-0.0.6.tar.gz`

## Comparing `directadminapi_sgs_shohani-0.0.5.tar` & `directadminapi_sgs_shohani-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.5/build_upload.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.5/src/DirectAdminAPI_SGS_shohani/__init__.py
--rw-r--r--   0        0        0     8285 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.5/src/DirectAdminAPI_SGS_shohani/api.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.5/tests/test.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.5/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.5/LICENSE
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.5/README.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.6/build_upload.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.6/src/DirectAdminAPI_SGS_shohani/__init__.py
+-rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.6/src/DirectAdminAPI_SGS_shohani/api.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.6/tests/test.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.6/LICENSE
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.6/README.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 directadminapi_sgs_shohani-0.0.6/PKG-INFO
```

### Comparing `directadminapi_sgs_shohani-0.0.5/src/DirectAdminAPI_SGS_shohani/api.py` & `directadminapi_sgs_shohani-0.0.6/src/DirectAdminAPI_SGS_shohani/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,14 +249,23 @@
         return self.cmd_all_user_show(
             page=1,            
             ipp=1000 ,#item per page
             bytes='yes',
             GET_METHOD = True
         )
 
+    def get_domains(self):
+        '''Get protected directory users list'''
+        return self.CMD_ADDITIONAL_DOMAINS(
+            page=1,     
+            ipp=1000 ,#item per page
+            bytes='yes',
+            GET_METHOD = True
+        )  
+
     def get_user_domains(self, user):
         '''Get protected directory users list'''
         return self.CMD_API_SHOW_USER_DOMAINS(
             page=1,     
             user=user,       
             ipp=1000 ,#item per page
             bytes='yes',
@@ -268,8 +277,10 @@
         return self.CMD_DNS_CONTROL(
             page=1,            
             ipp=1000 ,#item per page
             GET_METHOD = True,
             full_mx_records='yes',
             ttl='yes',
             domain=domain
-        )
+        )
+
+
```

### Comparing `directadminapi_sgs_shohani-0.0.5/tests/test.py` & `directadminapi_sgs_shohani-0.0.6/tests/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 #res_enable = api.enable_ssl('androidsoftware.ir')
 #res = api.enable_letsencrypt_ssl('androidsoftware.ir','name','sadegh.tkd@gmail.com',["androidsoftware.ir","www.androidsoftware.ir","mail.androidsoftware.ir"])
 
 #da_files = api.search_files(input('Enter path to list files:'),'a.txt' , recursive=True)
 
 #for key in da_files:
     #print(da_files[key])
-#res = api.get_user_domains('sadegh')
-#print(res["domains"])
+res = api.get_domains()
+print(res)
 
 res = api.get_user_dns('ghanbari.ir')
 print(res)
```

### Comparing `directadminapi_sgs_shohani-0.0.5/LICENSE` & `directadminapi_sgs_shohani-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `directadminapi_sgs_shohani-0.0.5/README.md` & `directadminapi_sgs_shohani-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `directadminapi_sgs_shohani-0.0.5/pyproject.toml` & `directadminapi_sgs_shohani-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "DirectAdminAPI_SGS_shohani"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Sadegh Ghanbari Shohani", email="sadegh.tkd@gmail.com" },
 ]
 description = "DirectAdmin API for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `directadminapi_sgs_shohani-0.0.5/PKG-INFO` & `directadminapi_sgs_shohani-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DirectAdminAPI_SGS_shohani
-Version: 0.0.5
+Version: 0.0.6
 Summary: DirectAdmin API for Python
 Project-URL: Homepage, https://github.com/sadeghtkd/DirectAdminAPI_SGS
 Project-URL: Bug Tracker, https://github.com/sadeghtkd/DirectAdminAPI_SGS/issues
 Author-email: Sadegh Ghanbari Shohani <sadegh.tkd@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

