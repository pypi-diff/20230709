# Comparing `tmp/key_switcheroo-0.0.5.tar.gz` & `tmp/key_switcheroo-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "key_switcheroo-0.0.5.tar", max compression
+gzip compressed data, was "key_switcheroo-0.0.6.tar", max compression
```

## Comparing `key_switcheroo-0.0.5.tar` & `key_switcheroo-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       71 2023-07-03 18:53:38.173952 key_switcheroo-0.0.5/README.md
--rw-r--r--   0        0        0      678 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.5/switcheroo/__init__.py
--rw-r--r--   0        0        0     3164 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/custom_keygen.py
--rw-r--r--   0        0        0       77 2023-07-07 03:40:51.516287 key_switcheroo-0.0.5/switcheroo/data_store/__init__.py
--rw-r--r--   0        0        0     3211 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/data_store/data_stores.py
--rw-r--r--   0        0        0     2939 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/data_store/s3.py
--rw-r--r--   0        0        0      311 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/exceptions.py
--rw-r--r--   0        0        0     1410 2023-07-07 03:40:51.516287 key_switcheroo-0.0.5/switcheroo/paths.py
--rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.5/switcheroo/publisher/__init__.py
--rw-r--r--   0        0        0     1570 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/publisher/__main__.py
--rw-r--r--   0        0        0     1617 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/publisher/key_publisher.py
--rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.5/switcheroo/server/__init__.py
--rwxr-xr-x   0        0        0     1915 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/server/__main__.py
--rw-r--r--   0        0        0     5045 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/server/server.py
--rw-r--r--   0        0        0     2658 2023-07-07 18:03:24.238887 key_switcheroo-0.0.5/switcheroo/util.py
--rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 key_switcheroo-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     5060 2023-07-09 19:13:51.612702 key_switcheroo-0.0.6/README.md
+-rw-r--r--   0        0        0      678 2023-07-07 18:03:24.238887 key_switcheroo-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.6/switcheroo/__init__.py
+-rw-r--r--   0        0        0     3164 2023-07-07 18:03:24.238887 key_switcheroo-0.0.6/switcheroo/custom_keygen.py
+-rw-r--r--   0        0        0       77 2023-07-07 03:40:51.516287 key_switcheroo-0.0.6/switcheroo/data_store/__init__.py
+-rw-r--r--   0        0        0     3307 2023-07-09 19:13:51.612702 key_switcheroo-0.0.6/switcheroo/data_store/data_stores.py
+-rw-r--r--   0        0        0     3024 2023-07-09 19:13:51.612702 key_switcheroo-0.0.6/switcheroo/data_store/s3.py
+-rw-r--r--   0        0        0      632 2023-07-09 19:13:51.612702 key_switcheroo-0.0.6/switcheroo/exceptions.py
+-rw-r--r--   0        0        0     1410 2023-07-07 03:40:51.516287 key_switcheroo-0.0.6/switcheroo/paths.py
+-rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.6/switcheroo/publisher/__init__.py
+-rw-r--r--   0        0        0     1570 2023-07-07 18:03:24.238887 key_switcheroo-0.0.6/switcheroo/publisher/__main__.py
+-rw-r--r--   0        0        0     1617 2023-07-07 18:03:24.238887 key_switcheroo-0.0.6/switcheroo/publisher/key_publisher.py
+-rw-r--r--   0        0        0        0 2023-07-05 19:39:01.733785 key_switcheroo-0.0.6/switcheroo/server/__init__.py
+-rwxr-xr-x   0        0        0     1915 2023-07-07 18:03:24.238887 key_switcheroo-0.0.6/switcheroo/server/__main__.py
+-rw-r--r--   0        0        0     5045 2023-07-07 18:03:24.238887 key_switcheroo-0.0.6/switcheroo/server/server.py
+-rw-r--r--   0        0        0     2658 2023-07-07 18:03:24.238887 key_switcheroo-0.0.6/switcheroo/util.py
+-rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 key_switcheroo-0.0.6/PKG-INFO
```

### Comparing `key_switcheroo-0.0.5/pyproject.toml` & `key_switcheroo-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.5/switcheroo/custom_keygen.py` & `key_switcheroo-0.0.6/switcheroo/custom_keygen.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.5/switcheroo/data_store/data_stores.py` & `key_switcheroo-0.0.6/switcheroo/data_store/data_stores.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,10 +74,10 @@
         return public_key.decode(), metadata
 
     def retrieve(self, host: str, user: str) -> str:
         key_path = paths.local_public_key_loc(host, user, home_dir=self.home_dir)
         try:
             with open(key_path, mode="rt", encoding="utf-8") as key_file:
                 return key_file.read()
-        except FileNotFoundError:
-            raise KeyNotFoundException()
-
+        except FileNotFoundError as exc:
+            exception_data = KeyNotFoundException.Data(user, host)
+            raise KeyNotFoundException(exception_data) from exc
```

### Comparing `key_switcheroo-0.0.5/switcheroo/data_store/s3.py` & `key_switcheroo-0.0.6/switcheroo/data_store/s3.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,16 @@
                 Bucket=self.s3_bucket_name,
                 Key=str(paths.cloud_public_key_loc(host, user)),
             )
             ssh_key = response["Body"].read().decode()
             return ssh_key
         except ClientError as exc:
             if exc.response["Error"]["Code"] == "NoSuchKey":
-                raise KeyNotFoundException() from exc
+                exception_data = KeyNotFoundException.Data(user, host)
+                raise KeyNotFoundException(exception_data) from exc
             raise exc
 
     def publish(
         self, host: str, user: str, metadata: KeyMetadata | None
     ) -> tuple[str, KeyMetadata]:
         if metadata is None:
             metadata = KeyMetadata.now_by_executing_user()
```

### Comparing `key_switcheroo-0.0.5/switcheroo/paths.py` & `key_switcheroo-0.0.6/switcheroo/paths.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.5/switcheroo/publisher/__main__.py` & `key_switcheroo-0.0.6/switcheroo/publisher/__main__.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.5/switcheroo/publisher/key_publisher.py` & `key_switcheroo-0.0.6/switcheroo/publisher/key_publisher.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.5/switcheroo/server/__main__.py` & `key_switcheroo-0.0.6/switcheroo/server/__main__.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.5/switcheroo/server/server.py` & `key_switcheroo-0.0.6/switcheroo/server/server.py`

 * *Files identical despite different names*

### Comparing `key_switcheroo-0.0.5/switcheroo/util.py` & `key_switcheroo-0.0.6/switcheroo/util.py`

 * *Files identical despite different names*

