# Comparing `tmp/va_mvg-0.9.6-py3-none-any.whl.zip` & `tmp/va_mvg-0.9.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 29076 bytes, number of entries: 16
--rw-r--r--  2.0 unx       69 b- defN 21-Nov-04 11:07 mvg/__init__.py
--rw-r--r--  2.0 unx     2134 b- defN 21-Nov-04 11:07 mvg/analysis_classes.py
--rw-r--r--  2.0 unx    31236 b- defN 21-Nov-04 11:07 mvg/mvg.py
--rw-r--r--  2.0 unx    17485 b- defN 21-Nov-04 11:07 mvg/plotting.py
--rw-r--r--  2.0 unx        0 b- defN 21-Nov-04 11:07 mvg/features/__init__.py
--rw-r--r--  2.0 unx     9767 b- defN 21-Nov-04 11:07 mvg/features/analysis.py
--rw-r--r--  2.0 unx     5916 b- defN 21-Nov-04 11:07 mvg/features/blacksheep.py
--rw-r--r--  2.0 unx     2040 b- defN 21-Nov-04 11:07 mvg/features/kpidemo.py
--rw-r--r--  2.0 unx     1997 b- defN 21-Nov-04 11:07 mvg/features/label_propagation.py
--rw-r--r--  2.0 unx     5778 b- defN 21-Nov-04 11:07 mvg/features/modeid.py
--rw-r--r--  2.0 unx     2413 b- defN 21-Nov-04 11:07 mvg/features/rms.py
--rw-r--r--  2.0 unx    11349 b- defN 21-Nov-04 11:09 va_mvg-0.9.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     4945 b- defN 21-Nov-04 11:09 va_mvg-0.9.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Nov-04 11:09 va_mvg-0.9.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 21-Nov-04 11:09 va_mvg-0.9.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1239 b- defN 21-Nov-04 11:09 va_mvg-0.9.6.dist-info/RECORD
-16 files, 96464 bytes uncompressed, 27062 bytes compressed:  71.9%
+Zip file size: 29210 bytes, number of entries: 16
+-rw-r--r--  2.0 unx       69 b- defN 21-Nov-10 15:42 mvg/__init__.py
+-rw-r--r--  2.0 unx     2134 b- defN 21-Nov-10 15:42 mvg/analysis_classes.py
+-rw-r--r--  2.0 unx    32085 b- defN 21-Nov-10 15:42 mvg/mvg.py
+-rw-r--r--  2.0 unx    17485 b- defN 21-Nov-10 15:42 mvg/plotting.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Nov-10 15:42 mvg/features/__init__.py
+-rw-r--r--  2.0 unx     9767 b- defN 21-Nov-10 15:42 mvg/features/analysis.py
+-rw-r--r--  2.0 unx     5916 b- defN 21-Nov-10 15:42 mvg/features/blacksheep.py
+-rw-r--r--  2.0 unx     2040 b- defN 21-Nov-10 15:42 mvg/features/kpidemo.py
+-rw-r--r--  2.0 unx     1997 b- defN 21-Nov-10 15:42 mvg/features/label_propagation.py
+-rw-r--r--  2.0 unx     5778 b- defN 21-Nov-10 15:42 mvg/features/modeid.py
+-rw-r--r--  2.0 unx     2413 b- defN 21-Nov-10 15:42 mvg/features/rms.py
+-rw-r--r--  2.0 unx    11349 b- defN 21-Nov-10 15:43 va_mvg-0.9.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4945 b- defN 21-Nov-10 15:43 va_mvg-0.9.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Nov-10 15:43 va_mvg-0.9.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 21-Nov-10 15:43 va_mvg-0.9.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1239 b- defN 21-Nov-10 15:43 va_mvg-0.9.7.dist-info/RECORD
+16 files, 97313 bytes uncompressed, 27196 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: mvg/features/modeid.py
 Comment: 
 
 Filename: mvg/features/rms.py
 Comment: 
 
-Filename: va_mvg-0.9.6.dist-info/LICENSE
+Filename: va_mvg-0.9.7.dist-info/LICENSE
 Comment: 
 
-Filename: va_mvg-0.9.6.dist-info/METADATA
+Filename: va_mvg-0.9.7.dist-info/METADATA
 Comment: 
 
-Filename: va_mvg-0.9.6.dist-info/WHEEL
+Filename: va_mvg-0.9.7.dist-info/WHEEL
 Comment: 
 
-Filename: va_mvg-0.9.6.dist-info/top_level.txt
+Filename: va_mvg-0.9.7.dist-info/top_level.txt
 Comment: 
 
-Filename: va_mvg-0.9.6.dist-info/RECORD
+Filename: va_mvg-0.9.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mvg/mvg.py

```diff
@@ -49,16 +49,16 @@
             If a connection to the API cannot be established.
 
         """
 
         self.endpoint = endpoint
         self.token = token
 
-        self.mvg_version = self.parse_version("v0.9.6")
-        self.tested_api_version = self.parse_version("v0.2.6")
+        self.mvg_version = self.parse_version("v0.9.7")
+        self.tested_api_version = self.parse_version("v0.2.7")
 
         # Get API version
         try:
             response = self._request("get", "")
         except RequestException:
             raise requests.ConnectionError("Could not connect to the API.")
 
@@ -669,14 +669,15 @@
     def request_analysis(
         self,
         sid: str,
         feature: str,
         parameters: dict = None,
         start_timestamp: int = None,
         end_timestamp: int = None,
+        callback_url: str = None,
     ) -> dict:
         """Request an analysis on the given endpoint with given parameters.
 
         Parameters
         ----------
         sid : str
             source Id.
@@ -689,14 +690,19 @@
 
         start_timestamp : int
             start of analysis time window [optional].
 
         end_timestamp : int
             start of analysis time window [optional].
 
+        callback_url : str
+            Base URL to receieve a notification when the analysis job ends.
+            A POST reuest will be made to {callback_url}/analyses with payload
+            that includes the request_id and request_status of the job [optional].
+
         Returns
         -------
         request_id: analysis identifier
 
         """
         logger.info("endpoint %s", self.endpoint)
         logger.info("source id=%s", sid)
@@ -711,26 +717,31 @@
         analysis_info = {
             "source_id": sid,
             "feature": feature,
             "params": parameters,
             "start_timestamp": start_timestamp,
             "end_timestamp": end_timestamp,
         }
-
-        response = self._request("post", "/analyses/requests/", json=analysis_info)
+        params = None
+        if callback_url:
+            params = {"callback_url": callback_url}
+        response = self._request(
+            "post", "/analyses/requests/", json=analysis_info, params=params
+        )
 
         return response.json()
 
     def request_population_analysis(
         self,
         sids: List[str],
         feature: str,
         parameters: dict = None,
         start_timestamp: int = None,
         end_timestamp: int = None,
+        callback_url: str = None,
     ) -> str:
         """Request an population analysis on the given endpoint with given parameters.
 
         Parameters
         ----------
         sids : List[str]
             Source ids.
@@ -743,14 +754,19 @@
 
         start_timestamp : int
             start of analysis time window [optional].
 
         end_timestamp : int
             start of analysis time window [optional].
 
+        callback_url : str
+            Base URL to receieve a notification when the analysis job ends.
+            A POST reuest will be made to {callback_url}/analyses with payload
+            that includes the request_id and request_status of the job [optional].
+
         Returns
         -------
         request_id: analysis identifier
 
         """
         logger.info("endpoint %s", self.endpoint)
         logger.info("source ids=%s", sids)
@@ -766,16 +782,19 @@
             "source_ids": sids,
             "feature": feature,
             "params": parameters,
             "start_timestamp": start_timestamp,
             "end_timestamp": end_timestamp,
         }
 
+        params = None
+        if callback_url:
+            params = {"callback_url": callback_url}
         response = self._request(
-            "post", "/analyses/requests/population/", json=analysis_info
+            "post", "/analyses/requests/population/", json=analysis_info, params=params
         )
         return response.json()
 
     def list_analyses(self, sid: str, feature: str) -> list:
         """Retrieves list of analysis IDs associated with a source
         and a feature.
```

## Comparing `va_mvg-0.9.6.dist-info/LICENSE` & `va_mvg-0.9.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `va_mvg-0.9.6.dist-info/METADATA` & `va_mvg-0.9.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: va-mvg
-Version: 0.9.6
+Version: 0.9.7
 Summary: MultiViz Analytics Engine library
 Home-page: https://github.com/vikinganalytics/mvg
 Author: Viking Analytics
 Author-email: info@vikinganalytics.se
 License: LICENSE
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `va_mvg-0.9.6.dist-info/RECORD` & `va_mvg-0.9.7.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 mvg/__init__.py,sha256=-cECv_br8fVdHirc4zHWxtphMq-iCilMjMpKOFJ8pAg,69
 mvg/analysis_classes.py,sha256=_uwHBuaEXlEYFMztR1V0fO-2IzksaO8HnREXZhO50P8,2134
-mvg/mvg.py,sha256=PzsYRzEd_K2prAdNtOwFF-9O44SNg6oqDR1VQbiV8mc,31236
+mvg/mvg.py,sha256=eJm7vYynXJDWG_TKSHAe2Mp7LdcorFKqkhiz4OCNX3E,32085
 mvg/plotting.py,sha256=v4PEW3ET2EbFvHhsGpeWeNbx2rB7CrhOstAPA3QV6_Q,17485
 mvg/features/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mvg/features/analysis.py,sha256=94Z5vyodp_dQZZ2epEKIMKS75AN0EzvWVAtKpZFbSIQ,9767
 mvg/features/blacksheep.py,sha256=DdhN6Y0N3EJCW1a7f2k6toYJbs59gYHAEyelQHdswhs,5916
 mvg/features/kpidemo.py,sha256=DT5cI--psd1HmFXqwJ6qwqHjXtUZp9RGgh73xn5pj3A,2040
 mvg/features/label_propagation.py,sha256=OyPX-sVSFrhKgsr83HFcVsPv7GzCmi76YGdN7zLu7Wc,1997
 mvg/features/modeid.py,sha256=DUTpysrRDtT0_At6Qcifm27cIkgILpGwq6i4qC-w2V0,5778
 mvg/features/rms.py,sha256=1V5tubtnJHFQURwPyh8i83oTIsdFeN8NEb4I0lZzVLQ,2413
-va_mvg-0.9.6.dist-info/LICENSE,sha256=pmaZ5UFog2le_qtXfYxin5lQXUaSMcY_wbWMY2d4y54,11349
-va_mvg-0.9.6.dist-info/METADATA,sha256=zA-yIGNghKR-bcuvdCy74UrmPpFyW3TIW5yRrItls2Y,4945
-va_mvg-0.9.6.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-va_mvg-0.9.6.dist-info/top_level.txt,sha256=D0NlO5S-Jv8LNhyMUU6mnY9uDURl50kdos0iLicL3E8,4
-va_mvg-0.9.6.dist-info/RECORD,,
+va_mvg-0.9.7.dist-info/LICENSE,sha256=pmaZ5UFog2le_qtXfYxin5lQXUaSMcY_wbWMY2d4y54,11349
+va_mvg-0.9.7.dist-info/METADATA,sha256=7-IFNmuaD419NQmPQxazoK44MiqxXAPL3W783EYYgk8,4945
+va_mvg-0.9.7.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+va_mvg-0.9.7.dist-info/top_level.txt,sha256=D0NlO5S-Jv8LNhyMUU6mnY9uDURl50kdos0iLicL3E8,4
+va_mvg-0.9.7.dist-info/RECORD,,
```

