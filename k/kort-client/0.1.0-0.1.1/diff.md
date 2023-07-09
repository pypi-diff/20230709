# Comparing `tmp/kort_client-0.1.0.tar.gz` & `tmp/kort_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kort_client-0.1.0.tar", max compression
+gzip compressed data, was "kort_client-0.1.1.tar", max compression
```

## Comparing `kort_client-0.1.0.tar` & `kort_client-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       22 2022-03-19 20:12:26.755333 kort_client-0.1.0/kort_client/__init__.py
--rw-r--r--   0        0        0     3511 2023-06-17 19:45:23.809166 kort_client-0.1.0/kort_client/api.py
--rw-r--r--   0        0        0     4181 2023-06-17 19:45:23.805165 kort_client-0.1.0/kort_client/card_detectors.py
--rw-r--r--   0        0        0     1479 2023-06-17 15:35:35.077161 kort_client-0.1.0/kort_client/cli.py
--rw-r--r--   0        0        0      267 2022-12-04 11:56:13.071238 kort_client-0.1.0/kort_client/config.py
--rw-r--r--   0        0        0     6506 2023-06-17 19:45:23.817166 kort_client-0.1.0/kort_client/run.py
--rw-r--r--   0        0        0        0 2022-04-11 13:40:18.178000 kort_client-0.1.0/kort_client/usb_barcode_scanner/__init__.py
--rwxr-xr-x   0        0        0     3742 2022-05-28 14:33:45.427410 kort_client-0.1.0/kort_client/usb_barcode_scanner/scanner.py
--rw-r--r--   0        0        0      883 2023-06-17 19:52:56.219169 kort_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 kort_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2022-03-19 20:12:26.755333 kort_client-0.1.1/kort_client/__init__.py
+-rw-r--r--   0        0        0     3403 2023-07-09 09:19:47.499107 kort_client-0.1.1/kort_client/api.py
+-rw-r--r--   0        0        0     4181 2023-06-17 19:45:23.805165 kort_client-0.1.1/kort_client/card_detectors.py
+-rw-r--r--   0        0        0     1479 2023-06-17 15:35:35.077161 kort_client-0.1.1/kort_client/cli.py
+-rw-r--r--   0        0        0      267 2022-12-04 11:56:13.071238 kort_client-0.1.1/kort_client/config.py
+-rw-r--r--   0        0        0     6506 2023-06-17 19:45:23.817166 kort_client-0.1.1/kort_client/run.py
+-rw-r--r--   0        0        0        0 2022-04-11 13:40:18.178000 kort_client-0.1.1/kort_client/usb_barcode_scanner/__init__.py
+-rwxr-xr-x   0        0        0     3742 2022-05-28 14:33:45.427410 kort_client-0.1.1/kort_client/usb_barcode_scanner/scanner.py
+-rw-r--r--   0        0        0      883 2023-07-09 09:19:54.739485 kort_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 kort_client-0.1.1/PKG-INFO
```

### Comparing `kort_client-0.1.0/kort_client/api.py` & `kort_client-0.1.1/kort_client/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,16 +73,14 @@
     def _validate_settings(self):
         if not self.settings.client_id:
             raise ConfigurationException("No client_id set.")
         if not self.settings.client_secret:
             raise ConfigurationException("No client_secret set.")
         if not self.settings.base_url:
             raise ConfigurationException("No base_url set.")
-        if not self.settings.access_token:
-            raise ConfigurationException("No access_token set.")
 
     def _do_request(
         self, method: str, url: str, attrs: Optional[Sequence] = None, **kwargs
     ) -> dict[str, Any]:
         if url in self.URLS:
             url = self.URLS[url]
         if attrs:
```

### Comparing `kort_client-0.1.0/kort_client/card_detectors.py` & `kort_client-0.1.1/kort_client/card_detectors.py`

 * *Files identical despite different names*

### Comparing `kort_client-0.1.0/kort_client/cli.py` & `kort_client-0.1.1/kort_client/cli.py`

 * *Files identical despite different names*

### Comparing `kort_client-0.1.0/kort_client/run.py` & `kort_client-0.1.1/kort_client/run.py`

 * *Files identical despite different names*

### Comparing `kort_client-0.1.0/kort_client/usb_barcode_scanner/scanner.py` & `kort_client-0.1.1/kort_client/usb_barcode_scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `kort_client-0.1.0/pyproject.toml` & `kort_client-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kort-client"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Jonathan Weth <git@jonathanweth.de>"]
 
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 secondary = true
```

### Comparing `kort_client-0.1.0/PKG-INFO` & `kort_client-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kort-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Jonathan Weth
 Author-email: git@jonathanweth.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

