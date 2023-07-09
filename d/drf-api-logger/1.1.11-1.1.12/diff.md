# Comparing `tmp/drf_api_logger-1.1.11.tar.gz` & `tmp/drf_api_logger-1.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\drf_api_logger-1.1.11.tar", last modified: Sat Sep 17 20:56:53 2022, max compression
+gzip compressed data, was "dist\drf_api_logger-1.1.12.tar", last modified: Wed Jan 18 18:04:28 2023, max compression
```

## Comparing `drf_api_logger-1.1.11.tar` & `drf_api_logger-1.1.12.tar`

### file list

```diff
@@ -1,35 +1,41 @@
-drwxrwxrwx   0        0        0        0 2022-09-17 20:56:53.446900 drf_api_logger-1.1.11/
--rw-rw-rw-   0        0        0     1085 2021-04-03 08:51:43.000000 drf_api_logger-1.1.11/LICENSE
--rw-rw-rw-   0        0        0      145 2021-04-03 08:51:43.000000 drf_api_logger-1.1.11/MANIFEST.in
--rw-rw-rw-   0        0        0    11066 2022-09-17 20:56:53.446900 drf_api_logger-1.1.11/PKG-INFO
--rw-rw-rw-   0        0        0    10459 2022-09-17 17:29:00.000000 drf_api_logger-1.1.11/README.md
-drwxrwxrwx   0        0        0        0 2022-09-17 20:56:53.423896 drf_api_logger-1.1.11/drf_api_logger/
--rw-rw-rw-   0        0        0      196 2021-02-22 18:36:39.000000 drf_api_logger-1.1.11/drf_api_logger/__init__.py
--rw-rw-rw-   0        0        0     7133 2022-09-17 20:49:38.000000 drf_api_logger-1.1.11/drf_api_logger/admin.py
--rw-rw-rw-   0        0        0      137 2021-01-14 00:49:47.000000 drf_api_logger-1.1.11/drf_api_logger/apps.py
--rw-rw-rw-   0        0        0      171 2021-01-14 01:48:24.000000 drf_api_logger-1.1.11/drf_api_logger/collectstatic.py
--rw-rw-rw-   0        0        0     2992 2021-01-14 00:49:47.000000 drf_api_logger-1.1.11/drf_api_logger/events.py
--rw-rw-rw-   0        0        0     2527 2022-01-27 17:48:49.000000 drf_api_logger-1.1.11/drf_api_logger/insert_log_into_database.py
-drwxrwxrwx   0        0        0        0 2022-09-17 20:56:53.443899 drf_api_logger-1.1.11/drf_api_logger/middleware/
--rw-rw-rw-   0        0        0        0 2021-01-14 00:49:47.000000 drf_api_logger-1.1.11/drf_api_logger/middleware/__init__.py
--rw-rw-rw-   0        0        0     6478 2022-09-17 18:08:13.000000 drf_api_logger-1.1.11/drf_api_logger/middleware/api_logger_middleware.py
-drwxrwxrwx   0        0        0        0 2022-09-17 20:56:53.445400 drf_api_logger-1.1.11/drf_api_logger/migrations/
--rw-rw-rw-   0        0        0     1303 2021-12-21 16:56:15.000000 drf_api_logger-1.1.11/drf_api_logger/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      426 2022-04-12 16:33:11.000000 drf_api_logger-1.1.11/drf_api_logger/migrations/0002_auto_20211221_2155.py
--rw-rw-rw-   0        0        0        0 2021-01-14 00:49:47.000000 drf_api_logger-1.1.11/drf_api_logger/migrations/__init__.py
--rw-rw-rw-   0        0        0     1328 2022-04-12 16:33:11.000000 drf_api_logger-1.1.11/drf_api_logger/models.py
--rw-rw-rw-   0        0        0      596 2022-09-17 20:09:19.000000 drf_api_logger-1.1.11/drf_api_logger/start_logger_when_server_starts.py
-drwxrwxrwx   0        0        0        0 2022-09-17 20:56:53.446400 drf_api_logger-1.1.11/drf_api_logger/templates/
--rw-rw-rw-   0        0        0      203 2022-04-12 16:33:11.000000 drf_api_logger-1.1.11/drf_api_logger/templates/change_form.html
--rw-rw-rw-   0        0        0     2817 2022-09-17 20:49:49.000000 drf_api_logger-1.1.11/drf_api_logger/templates/charts_change_list.html
--rw-rw-rw-   0        0        0        0 2021-01-14 00:49:47.000000 drf_api_logger-1.1.11/drf_api_logger/tests.py
--rw-rw-rw-   0        0        0     2134 2022-04-12 16:33:11.000000 drf_api_logger-1.1.11/drf_api_logger/utils.py
-drwxrwxrwx   0        0        0        0 2022-09-17 20:56:53.442399 drf_api_logger-1.1.11/drf_api_logger.egg-info/
--rw-rw-rw-   0        0        0    11066 2022-09-17 20:56:53.000000 drf_api_logger-1.1.11/drf_api_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      862 2022-09-17 20:56:53.000000 drf_api_logger-1.1.11/drf_api_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-17 20:56:53.000000 drf_api_logger-1.1.11/drf_api_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2022-09-17 20:56:53.000000 drf_api_logger-1.1.11/drf_api_logger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-09-17 20:56:53.000000 drf_api_logger-1.1.11/drf_api_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       69 2021-04-03 08:51:43.000000 drf_api_logger-1.1.11/pyproject.toml
--rw-rw-rw-   0        0        0       80 2022-09-17 20:56:53.450901 drf_api_logger-1.1.11/setup.cfg
--rw-rw-rw-   0        0        0     1632 2022-04-22 16:47:20.000000 drf_api_logger-1.1.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-18 18:04:28.385357 drf_api_logger-1.1.12/
+-rw-rw-rw-   0        0        0     1085 2021-04-03 08:51:43.000000 drf_api_logger-1.1.12/LICENSE
+-rw-rw-rw-   0        0        0      145 2021-04-03 08:51:43.000000 drf_api_logger-1.1.12/MANIFEST.in
+-rw-rw-rw-   0        0        0    11066 2023-01-18 18:04:28.385357 drf_api_logger-1.1.12/PKG-INFO
+-rw-rw-rw-   0        0        0    10459 2023-01-18 17:36:23.000000 drf_api_logger-1.1.12/README.md
+drwxrwxrwx   0        0        0        0 2023-01-18 18:04:28.366283 drf_api_logger-1.1.12/drf_api_logger/
+-rw-rw-rw-   0        0        0      196 2021-02-22 18:36:39.000000 drf_api_logger-1.1.12/drf_api_logger/__init__.py
+-rw-rw-rw-   0        0        0     7133 2022-09-17 20:49:38.000000 drf_api_logger-1.1.12/drf_api_logger/admin.py
+-rw-rw-rw-   0        0        0      137 2021-01-14 00:49:47.000000 drf_api_logger-1.1.12/drf_api_logger/apps.py
+-rw-rw-rw-   0        0        0      171 2021-01-14 01:48:24.000000 drf_api_logger-1.1.12/drf_api_logger/collectstatic.py
+-rw-rw-rw-   0        0        0     2992 2021-01-14 00:49:47.000000 drf_api_logger-1.1.12/drf_api_logger/events.py
+-rw-rw-rw-   0        0        0     2527 2022-01-27 17:48:49.000000 drf_api_logger-1.1.12/drf_api_logger/insert_log_into_database.py
+drwxrwxrwx   0        0        0        0 2023-01-18 18:04:28.381141 drf_api_logger-1.1.12/drf_api_logger/middleware/
+-rw-rw-rw-   0        0        0        0 2021-01-14 00:49:47.000000 drf_api_logger-1.1.12/drf_api_logger/middleware/__init__.py
+-rw-rw-rw-   0        0        0     6705 2023-01-18 17:35:32.000000 drf_api_logger-1.1.12/drf_api_logger/middleware/api_logger_middleware.py
+drwxrwxrwx   0        0        0        0 2023-01-18 18:04:28.382660 drf_api_logger-1.1.12/drf_api_logger/migrations/
+-rw-rw-rw-   0        0        0     1303 2021-12-21 16:56:15.000000 drf_api_logger-1.1.12/drf_api_logger/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      426 2022-04-12 16:33:11.000000 drf_api_logger-1.1.12/drf_api_logger/migrations/0002_auto_20211221_2155.py
+-rw-rw-rw-   0        0        0        0 2021-01-14 00:49:47.000000 drf_api_logger-1.1.12/drf_api_logger/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1328 2022-04-12 16:33:11.000000 drf_api_logger-1.1.12/drf_api_logger/models.py
+-rw-rw-rw-   0        0        0      596 2022-09-17 20:09:19.000000 drf_api_logger-1.1.12/drf_api_logger/start_logger_when_server_starts.py
+drwxrwxrwx   0        0        0        0 2023-01-18 18:04:28.357086 drf_api_logger-1.1.12/drf_api_logger/static/
+drwxrwxrwx   0        0        0        0 2023-01-18 18:04:28.357589 drf_api_logger-1.1.12/drf_api_logger/static/drf_api_logger/
+drwxrwxrwx   0        0        0        0 2023-01-18 18:04:28.383321 drf_api_logger-1.1.12/drf_api_logger/static/drf_api_logger/css/
+-rw-rw-rw-   0        0        0      521 2023-01-18 17:33:50.000000 drf_api_logger-1.1.12/drf_api_logger/static/drf_api_logger/css/Chart.min.css
+drwxrwxrwx   0        0        0        0 2023-01-18 18:04:28.383827 drf_api_logger-1.1.12/drf_api_logger/static/drf_api_logger/js/
+-rw-rw-rw-   0        0        0   210031 2023-01-18 17:33:50.000000 drf_api_logger-1.1.12/drf_api_logger/static/drf_api_logger/js/Chart.bundle.min.js
+drwxrwxrwx   0        0        0        0 2023-01-18 18:04:28.384845 drf_api_logger-1.1.12/drf_api_logger/templates/
+-rw-rw-rw-   0        0        0      203 2022-04-12 16:33:11.000000 drf_api_logger-1.1.12/drf_api_logger/templates/change_form.html
+-rw-rw-rw-   0        0        0     2778 2023-01-18 17:33:50.000000 drf_api_logger-1.1.12/drf_api_logger/templates/charts_change_list.html
+-rw-rw-rw-   0        0        0        0 2021-01-14 00:49:47.000000 drf_api_logger-1.1.12/drf_api_logger/tests.py
+-rw-rw-rw-   0        0        0     2562 2023-01-18 17:35:32.000000 drf_api_logger-1.1.12/drf_api_logger/utils.py
+drwxrwxrwx   0        0        0        0 2023-01-18 18:04:28.379243 drf_api_logger-1.1.12/drf_api_logger.egg-info/
+-rw-rw-rw-   0        0        0    11066 2023-01-18 18:04:28.000000 drf_api_logger-1.1.12/drf_api_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      977 2023-01-18 18:04:28.000000 drf_api_logger-1.1.12/drf_api_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-18 18:04:28.000000 drf_api_logger-1.1.12/drf_api_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-01-18 18:04:28.000000 drf_api_logger-1.1.12/drf_api_logger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-01-18 18:04:28.000000 drf_api_logger-1.1.12/drf_api_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       69 2021-04-03 08:51:43.000000 drf_api_logger-1.1.12/pyproject.toml
+-rw-rw-rw-   0        0        0       80 2023-01-18 18:04:28.388922 drf_api_logger-1.1.12/setup.cfg
+-rw-rw-rw-   0        0        0     1632 2023-01-18 17:36:23.000000 drf_api_logger-1.1.12/setup.py
```

### Comparing `drf_api_logger-1.1.11/LICENSE` & `drf_api_logger-1.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_api_logger-1.1.11/PKG-INFO` & `drf_api_logger-1.1.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf_api_logger
-Version: 1.1.11
+Version: 1.1.12
 Summary: An API Logger for your Django Rest Framework project.
 Home-page: https://github.com/vishalanandl177/DRF-API-Logger
 Author: Vishal Anand
 Author-email: vishalanandl177@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DRF API Logger
-![version](https://img.shields.io/badge/version-1.1.11-blue.svg)
+![version](https://img.shields.io/badge/version-1.1.12-blue.svg)
 [![Downloads](https://static.pepy.tech/personalized-badge/drf-api-logger?period=total&units=none&left_color=black&right_color=orange&left_text=Downloads%20Total)](http://pepy.tech/project/drf-api-logger)
 [![Downloads](https://static.pepy.tech/personalized-badge/drf-api-logger?period=month&units=none&left_color=black&right_color=orange&left_text=Downloads%20Last%20Month)](https://pepy.tech/project/drf-api-logger)
 [![Downloads](https://static.pepy.tech/personalized-badge/drf-api-logger?period=week&units=none&left_color=black&right_color=orange&left_text=Downloads%20Last%20Week)](https://pepy.tech/project/drf-api-logger)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 [![Donate](https://img.shields.io/badge/$-support-ff69b4.svg?style=flat)](https://paypal.me/chynybekov)  
 
 <a href="https://discord.gg/eeYansFDCT"><img src="https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white" alt="Join Community Badge"/></a>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: drf_api_logger Version: 1.1.11 Summary: An API
+Metadata-Version: 2.1 Name: drf_api_logger Version: 1.1.12 Summary: An API
 Logger for your Django Rest Framework project. Home-page: https://github.com/
 vishalanandl177/DRF-API-Logger Author: Vishal Anand Author-email:
 vishalanandl177@gmail.com License: MIT Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Operating System :: OS Independent Requires-Python:
 >=3.6 Description-Content-Type: text/markdown License-File: LICENSE # DRF API
-Logger ![version](https://img.shields.io/badge/version-1.1.11-blue.svg) [!
+Logger ![version](https://img.shields.io/badge/version-1.1.12-blue.svg) [!
 [Downloads](https://static.pepy.tech/personalized-badge/drf-api-
 logger?period=total&units=none&left_color=black&right_color=orange&left_text=Downloads%20Total)]
 (http://pepy.tech/project/drf-api-logger) [![Downloads](https://
 static.pepy.tech/personalized-badge/drf-api-
 logger?period=month&units=none&left_color=black&right_color=orange&left_text=Downloads%20Last%20Month)]
 (https://pepy.tech/project/drf-api-logger) [![Downloads](https://
 static.pepy.tech/personalized-badge/drf-api-
```

### Comparing `drf_api_logger-1.1.11/README.md` & `drf_api_logger-1.1.12/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DRF API Logger
-![version](https://img.shields.io/badge/version-1.1.11-blue.svg)
+![version](https://img.shields.io/badge/version-1.1.12-blue.svg)
 [![Downloads](https://static.pepy.tech/personalized-badge/drf-api-logger?period=total&units=none&left_color=black&right_color=orange&left_text=Downloads%20Total)](http://pepy.tech/project/drf-api-logger)
 [![Downloads](https://static.pepy.tech/personalized-badge/drf-api-logger?period=month&units=none&left_color=black&right_color=orange&left_text=Downloads%20Last%20Month)](https://pepy.tech/project/drf-api-logger)
 [![Downloads](https://static.pepy.tech/personalized-badge/drf-api-logger?period=week&units=none&left_color=black&right_color=orange&left_text=Downloads%20Last%20Week)](https://pepy.tech/project/drf-api-logger)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 [![Donate](https://img.shields.io/badge/$-support-ff69b4.svg?style=flat)](https://paypal.me/chynybekov)  
 
 <a href="https://discord.gg/eeYansFDCT"><img src="https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white" alt="Join Community Badge"/></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-# DRF API Logger ![version](https://img.shields.io/badge/version-1.1.11-
+# DRF API Logger ![version](https://img.shields.io/badge/version-1.1.12-
 blue.svg) [![Downloads](https://static.pepy.tech/personalized-badge/drf-api-
 logger?period=total&units=none&left_color=black&right_color=orange&left_text=Downloads%20Total)]
 (http://pepy.tech/project/drf-api-logger) [![Downloads](https://
 static.pepy.tech/personalized-badge/drf-api-
 logger?period=month&units=none&left_color=black&right_color=orange&left_text=Downloads%20Last%20Month)]
 (https://pepy.tech/project/drf-api-logger) [![Downloads](https://
 static.pepy.tech/personalized-badge/drf-api-
```

### Comparing `drf_api_logger-1.1.11/drf_api_logger/admin.py` & `drf_api_logger-1.1.12/drf_api_logger/admin.py`

 * *Files identical despite different names*

### Comparing `drf_api_logger-1.1.11/drf_api_logger/events.py` & `drf_api_logger-1.1.12/drf_api_logger/events.py`

 * *Files identical despite different names*

### Comparing `drf_api_logger-1.1.11/drf_api_logger/insert_log_into_database.py` & `drf_api_logger-1.1.12/drf_api_logger/insert_log_into_database.py`

 * *Files identical despite different names*

### Comparing `drf_api_logger-1.1.11/drf_api_logger/middleware/api_logger_middleware.py` & `drf_api_logger-1.1.12/drf_api_logger/middleware/api_logger_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import time
+import re
 from django.conf import settings
 from django.urls import resolve
 from django.utils import timezone
 
 from drf_api_logger import API_LOGGER_SIGNAL
 from drf_api_logger.start_logger_when_server_starts import LOGGER_THREAD
 from drf_api_logger.utils import get_headers, get_client_ip, mask_sensitive_data
@@ -97,16 +98,19 @@
             headers = get_headers(request=request)
             method = request.method
 
             # Log only registered methods if available.
             if len(self.DRF_API_LOGGER_METHODS) > 0 and method not in self.DRF_API_LOGGER_METHODS:
                 return response
 
-            if response.get('content-type') in ('application/json', 'application/vnd.api+json',):
-                if getattr(response, 'streaming', False):
+            if response.get('content-type') in ('application/json', 'application/vnd.api+json', 'application/gzip'):
+                
+                if response.get('content-type') == 'application/gzip':
+                    response_body = '** GZIP Archive **'
+                elif getattr(response, 'streaming', False):
                     response_body = '** Streaming **'
                 else:
                     if type(response.content) == bytes:
                         response_body = json.loads(response.content.decode())
                     else:
                         response_body = json.loads(response.content)
                 if self.DRF_API_LOGGER_PATH_TYPE == 'ABSOLUTE':
@@ -115,15 +119,15 @@
                     api = request.get_full_path()
                 elif self.DRF_API_LOGGER_PATH_TYPE == 'RAW_URI':
                     api = request.get_raw_uri()
                 else:
                     api = request.build_absolute_uri()
 
                 data = dict(
-                    api=api,
+                    api=mask_sensitive_data(api, mask_api_parameters=True),
                     headers=mask_sensitive_data(headers),
                     body=mask_sensitive_data(request_data),
                     method=method,
                     client_ip_address=get_client_ip(request),
                     response=mask_sensitive_data(response_body),
                     status_code=response.status_code,
                     execution_time=time.time() - start_time,
```

### Comparing `drf_api_logger-1.1.11/drf_api_logger/migrations/0001_initial.py` & `drf_api_logger-1.1.12/drf_api_logger/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf_api_logger-1.1.11/drf_api_logger/models.py` & `drf_api_logger-1.1.12/drf_api_logger/models.py`

 * *Files identical despite different names*

### Comparing `drf_api_logger-1.1.11/drf_api_logger/start_logger_when_server_starts.py` & `drf_api_logger-1.1.12/drf_api_logger/start_logger_when_server_starts.py`

 * *Files identical despite different names*

### Comparing `drf_api_logger-1.1.11/drf_api_logger/templates/charts_change_list.html` & `drf_api_logger-1.1.12/drf_api_logger/templates/charts_change_list.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends "admin/change_list.html" %}
 {% load static %}
 
 <!-- Override extrahead to add Chart.js -->
 {% block extrahead %}
 {{ block.super }}
-<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.8.0/Chart.min.css" />
-<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.8.0/Chart.bundle.min.js"></script>
+<link rel="stylesheet" href="{% static "drf_api_logger/css/Chart.min.css" %}" />
+<script src="{% static "drf_api_logger/js/Chart.bundle.min.js" %}"></script>
 <script>
 
 document.addEventListener('DOMContentLoaded', () => {
   const ctx = document.getElementById('countChart').getContext('2d');
 
   const chartData = [
     {% for item in analytics %}
@@ -102,8 +102,8 @@
   <canvas style="margin-bottom: 30px; width: 60%; height: 50%;" id="countChart"></canvas>
 </div>
 <div style="width: 80%; margin-top: 24px;">
   <canvas style="margin-bottom: 30px; width: 60%; height: 50%;" id="statusCodeChart"></canvas>
 </div>
 <!-- Render the rest of the ChangeList view -->
 {{ block.super }}
-{% endblock %}
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,4 +1,6 @@
 {% extends "admin/change_list.html" %} {% load static %}  {% block extrahead %}
 {{ block.super }}
+ss/Chart.min.css" %}" />
+s/Chart.bundle.min.js" %}">
  {% endblock %} {% block content %}
  {{ block.super }} {% endblock %}
```

### Comparing `drf_api_logger-1.1.11/drf_api_logger.egg-info/PKG-INFO` & `drf_api_logger-1.1.12/drf_api_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-api-logger
-Version: 1.1.11
+Version: 1.1.12
 Summary: An API Logger for your Django Rest Framework project.
 Home-page: https://github.com/vishalanandl177/DRF-API-Logger
 Author: Vishal Anand
 Author-email: vishalanandl177@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DRF API Logger
-![version](https://img.shields.io/badge/version-1.1.11-blue.svg)
+![version](https://img.shields.io/badge/version-1.1.12-blue.svg)
 [![Downloads](https://static.pepy.tech/personalized-badge/drf-api-logger?period=total&units=none&left_color=black&right_color=orange&left_text=Downloads%20Total)](http://pepy.tech/project/drf-api-logger)
 [![Downloads](https://static.pepy.tech/personalized-badge/drf-api-logger?period=month&units=none&left_color=black&right_color=orange&left_text=Downloads%20Last%20Month)](https://pepy.tech/project/drf-api-logger)
 [![Downloads](https://static.pepy.tech/personalized-badge/drf-api-logger?period=week&units=none&left_color=black&right_color=orange&left_text=Downloads%20Last%20Week)](https://pepy.tech/project/drf-api-logger)
 [![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
 [![Donate](https://img.shields.io/badge/$-support-ff69b4.svg?style=flat)](https://paypal.me/chynybekov)  
 
 <a href="https://discord.gg/eeYansFDCT"><img src="https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white" alt="Join Community Badge"/></a>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: drf-api-logger Version: 1.1.11 Summary: An API
+Metadata-Version: 2.1 Name: drf-api-logger Version: 1.1.12 Summary: An API
 Logger for your Django Rest Framework project. Home-page: https://github.com/
 vishalanandl177/DRF-API-Logger Author: Vishal Anand Author-email:
 vishalanandl177@gmail.com License: MIT Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Operating System :: OS Independent Requires-Python:
 >=3.6 Description-Content-Type: text/markdown License-File: LICENSE # DRF API
-Logger ![version](https://img.shields.io/badge/version-1.1.11-blue.svg) [!
+Logger ![version](https://img.shields.io/badge/version-1.1.12-blue.svg) [!
 [Downloads](https://static.pepy.tech/personalized-badge/drf-api-
 logger?period=total&units=none&left_color=black&right_color=orange&left_text=Downloads%20Total)]
 (http://pepy.tech/project/drf-api-logger) [![Downloads](https://
 static.pepy.tech/personalized-badge/drf-api-
 logger?period=month&units=none&left_color=black&right_color=orange&left_text=Downloads%20Last%20Month)]
 (https://pepy.tech/project/drf-api-logger) [![Downloads](https://
 static.pepy.tech/personalized-badge/drf-api-
```

### Comparing `drf_api_logger-1.1.11/drf_api_logger.egg-info/SOURCES.txt` & `drf_api_logger-1.1.12/drf_api_logger.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -20,9 +20,11 @@
 drf_api_logger.egg-info/requires.txt
 drf_api_logger.egg-info/top_level.txt
 drf_api_logger/middleware/__init__.py
 drf_api_logger/middleware/api_logger_middleware.py
 drf_api_logger/migrations/0001_initial.py
 drf_api_logger/migrations/0002_auto_20211221_2155.py
 drf_api_logger/migrations/__init__.py
+drf_api_logger/static/drf_api_logger/css/Chart.min.css
+drf_api_logger/static/drf_api_logger/js/Chart.bundle.min.js
 drf_api_logger/templates/change_form.html
 drf_api_logger/templates/charts_change_list.html
```

### Comparing `drf_api_logger-1.1.11/setup.py` & `drf_api_logger-1.1.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
     return long_description
 
 
 setuptools.setup(
     name="drf_api_logger",
-    version="1.1.11",
+    version="1.1.12",
     author="Vishal Anand",
     author_email="vishalanandl177@gmail.com",
     description="An API Logger for your Django Rest Framework project.",
     long_description=get_long_desc(),
     long_description_content_type="text/markdown",
     url="https://github.com/vishalanandl177/DRF-API-Logger",
     packages=setuptools.find_packages(),
```

