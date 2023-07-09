# Comparing `tmp/atro_victoria-0.0.1.tar.gz` & `tmp/atro_victoria-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro_victoria-0.0.1.tar", max compression
+gzip compressed data, was "atro_victoria-0.0.2.tar", max compression
```

## Comparing `atro_victoria-0.0.1.tar` & `atro_victoria-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-09 16:47:06.656790 atro_victoria-0.0.1/README.md
--rw-r--r--   0        0        0     1736 2023-07-09 16:50:09.007275 atro_victoria-0.0.1/atro_victoria/__init__.py
--rw-r--r--   0        0        0      409 2023-07-09 16:46:06.495530 atro_victoria-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 atro_victoria-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-09 16:47:06.656790 atro_victoria-0.0.2/README.md
+-rw-r--r--   0        0        0     1723 2023-07-09 17:54:53.428384 atro_victoria-0.0.2/atro_victoria/__init__.py
+-rw-r--r--   0        0        0      409 2023-07-09 17:54:45.411547 atro_victoria-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 atro_victoria-0.0.2/PKG-INFO
```

### Comparing `atro_victoria-0.0.1/atro_victoria/__init__.py` & `atro_victoria-0.0.2/atro_victoria/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     if output == "":
       raise Exception("No values to format")
     return output[1:]
 
   def data_as_csv(self):
     vals = self.model_dump()
     vals.pop('url')
-    vals['timestamp'] = VmCsvRowBase.strigify_datetime(vals['timestamp'])
+    vals['timestamp'] = strigify_datetime(vals['timestamp'])
     output = ""
     for val in vals.values():
       
       output += "," + str(val)
     if output == "":
       raise Exception("No values to format")
     return output[1:]
```

