# Comparing `tmp/django_hmac_authentication-1.4.0.tar.gz` & `tmp/django_hmac_authentication-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hmac_authentication-1.4.0.tar", last modified: Sat Jul  8 02:31:08 2023, max compression
+gzip compressed data, was "django_hmac_authentication-1.4.1.tar", last modified: Sun Jul  9 03:59:01 2023, max compression
```

## Comparing `django_hmac_authentication-1.4.0.tar` & `django_hmac_authentication-1.4.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 02:31:08.624911 django_hmac_authentication-1.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6871 2023-07-08 02:31:08.624911 django_hmac_authentication-1.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6333 2023-07-08 02:05:32.000000 django_hmac_authentication-1.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-07-08 02:25:39.000000 django_hmac_authentication-1.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-08 02:31:08.624911 django_hmac_authentication-1.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 02:31:08.616911 django_hmac_authentication-1.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 02:31:08.620911 django_hmac_authentication-1.4.0/src/django_hmac_authentication/
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-08 02:25:39.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-06 00:58:59.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/aes.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-06-26 08:22:01.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     4447 2023-07-08 02:05:32.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     3335 2023-07-08 02:05:32.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/checks.py
--rw-rw-rw-   0 root         (0) root         (0)     2817 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/client_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2023-06-15 10:03:50.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 02:31:08.624911 django_hmac_authentication-1.4.0/src/django_hmac_authentication/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 02:30:31.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 02:31:08.624911 django_hmac_authentication-1.4.0/src/django_hmac_authentication/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 02:30:31.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 02:31:08.624911 django_hmac_authentication-1.4.0/src/django_hmac_authentication/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-05 22:40:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-08 02:30:31.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1229 2023-06-05 22:40:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/models.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/padding.py
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     3111 2023-07-08 02:05:32.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/server_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-08 02:31:08.624911 django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6871 2023-07-08 02:31:08.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1312 2023-07-08 02:31:08.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-08 02:31:08.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-08 02:31:08.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-08 02:31:08.000000 django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:59:01.213156 django_hmac_authentication-1.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6871 2023-07-09 03:59:01.213156 django_hmac_authentication-1.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6333 2023-07-08 02:05:32.000000 django_hmac_authentication-1.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-07-09 03:52:15.000000 django_hmac_authentication-1.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-09 03:59:01.213156 django_hmac_authentication-1.4.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:59:01.205156 django_hmac_authentication-1.4.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:59:01.209156 django_hmac_authentication-1.4.1/src/django_hmac_authentication/
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-09 03:52:15.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-06 00:58:59.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/aes.py
+-rw-rw-rw-   0 root         (0) root         (0)      455 2023-07-09 03:21:53.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     4447 2023-07-08 02:05:32.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     3403 2023-07-09 03:21:53.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2817 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/client_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2023-06-15 10:03:50.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:59:01.209156 django_hmac_authentication-1.4.1/src/django_hmac_authentication/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 03:58:21.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:59:01.209156 django_hmac_authentication-1.4.1/src/django_hmac_authentication/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 03:58:21.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:59:01.213156 django_hmac_authentication-1.4.1/src/django_hmac_authentication/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-05 22:40:36.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 03:58:21.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2023-06-05 22:40:36.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/padding.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3111 2023-07-08 02:05:32.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/server_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-07-09 03:21:53.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-06-04 10:27:36.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-09 03:59:01.209156 django_hmac_authentication-1.4.1/src/django_hmac_authentication.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6871 2023-07-09 03:59:01.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-07-09 03:59:01.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-09 03:59:01.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-09 03:59:01.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-09 03:59:01.000000 django_hmac_authentication-1.4.1/src/django_hmac_authentication.egg-info/top_level.txt
```

### Comparing `django_hmac_authentication-1.4.0/LICENSE` & `django_hmac_authentication-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.4.0/PKG-INFO` & `django_hmac_authentication-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_hmac_authentication
-Version: 1.4.0
+Version: 1.4.1
 Summary: Django HMAC authentication using shared secret
 Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
```

### Comparing `django_hmac_authentication-1.4.0/README.md` & `django_hmac_authentication-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.4.0/pyproject.toml` & `django_hmac_authentication-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["django_hmac_authentication*"]
 namespaces = false
 
 [project]
 name = "django_hmac_authentication"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
   { name="Harisankar Krishna Swamy", email="harisankar.krishna@outlook.com" },
 ]
 description = "Django HMAC authentication using shared secret"
 readme = "README.md"
 requires-python = ">=3.9.2"
 dependencies = [
```

### Comparing `django_hmac_authentication-1.4.0/src/django_hmac_authentication/admin.py` & `django_hmac_authentication-1.4.1/src/django_hmac_authentication/admin.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.4.0/src/django_hmac_authentication/aes.py` & `django_hmac_authentication-1.4.1/src/django_hmac_authentication/aes.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.4.0/src/django_hmac_authentication/authentication.py` & `django_hmac_authentication-1.4.1/src/django_hmac_authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.4.0/src/django_hmac_authentication/checks.py` & `django_hmac_authentication-1.4.1/src/django_hmac_authentication/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,25 +54,26 @@
                 obj=repr(hmac_auth_failed_attempts_threshold),
                 id='django_hmac_authentication.E003',
             )
         )
 
     # HMAC_EXPIRES_IN
     hmac_expires_in = getattr(settings, 'HMAC_EXPIRES_IN', None)
-    try:
-        timedelta_from_config(hmac_expires_in)
-    except (TypeError, ValueError):
-        errors.append(
-            Error(
-                f'If set, HMAC_EXPIRES_IN expire keys after interval in hours, minutes or seconds.  Found {repr(hmac_expires_in)}',
-                hint="Example '1h', '5m', '3600s'",
-                obj=repr(hmac_expires_in),
-                id='django_hmac_authentication.E004',
+    if hmac_expires_in:
+        try:
+            timedelta_from_config(hmac_expires_in)
+        except (TypeError, ValueError):
+            errors.append(
+                Error(
+                    f'If set, HMAC_EXPIRES_IN expire keys after interval in hours, minutes or seconds.  Found {repr(hmac_expires_in)}',
+                    hint="Example '1h', '5m', '3600s'",
+                    obj=repr(hmac_expires_in),
+                    id='django_hmac_authentication.E004',
+                )
             )
-        )
 
     # HMAC_CACHE_ALIAS
     hmac_cache_alias = getattr(settings, 'HMAC_CACHE_ALIAS', None)
     if hmac_cache_alias and hmac_cache_alias not in settings.CACHES:
         errors.append(
             Error(
                 f'Missing entry in settings.py CACHES for HMAC_CACHE_ALIAS "{hmac_cache_alias}"',
```

### Comparing `django_hmac_authentication-1.4.0/src/django_hmac_authentication/client_utils.py` & `django_hmac_authentication-1.4.1/src/django_hmac_authentication/client_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.4.0/src/django_hmac_authentication/exceptions.py` & `django_hmac_authentication-1.4.1/src/django_hmac_authentication/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.4.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py` & `django_hmac_authentication-1.4.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.4.0/src/django_hmac_authentication/migrations/0001_initial.py` & `django_hmac_authentication-1.4.1/src/django_hmac_authentication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.4.0/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py` & `django_hmac_authentication-1.4.1/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.4.0/src/django_hmac_authentication/models.py` & `django_hmac_authentication-1.4.1/src/django_hmac_authentication/models.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.4.0/src/django_hmac_authentication/server_utils.py` & `django_hmac_authentication-1.4.1/src/django_hmac_authentication/server_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.4.0/src/django_hmac_authentication/views.py` & `django_hmac_authentication-1.4.1/src/django_hmac_authentication/views.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/PKG-INFO` & `django_hmac_authentication-1.4.1/src/django_hmac_authentication.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hmac-authentication
-Version: 1.4.0
+Version: 1.4.1
 Summary: Django HMAC authentication using shared secret
 Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
```

### Comparing `django_hmac_authentication-1.4.0/src/django_hmac_authentication.egg-info/SOURCES.txt` & `django_hmac_authentication-1.4.1/src/django_hmac_authentication.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/django_hmac_authentication/checks.py
 src/django_hmac_authentication/client_utils.py
 src/django_hmac_authentication/exceptions.py
 src/django_hmac_authentication/models.py
 src/django_hmac_authentication/padding.py
 src/django_hmac_authentication/serializers.py
 src/django_hmac_authentication/server_utils.py
+src/django_hmac_authentication/signals.py
 src/django_hmac_authentication/views.py
 src/django_hmac_authentication.egg-info/PKG-INFO
 src/django_hmac_authentication.egg-info/SOURCES.txt
 src/django_hmac_authentication.egg-info/dependency_links.txt
 src/django_hmac_authentication.egg-info/requires.txt
 src/django_hmac_authentication.egg-info/top_level.txt
 src/django_hmac_authentication/management/__init__.py
```

