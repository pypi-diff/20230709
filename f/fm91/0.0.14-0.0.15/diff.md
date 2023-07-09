# Comparing `tmp/fm91-0.0.14.tar.gz` & `tmp/fm91-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fm91-0.0.14.tar", max compression
+gzip compressed data, was "fm91-0.0.15.tar", max compression
```

## Comparing `fm91-0.0.14.tar` & `fm91-0.0.15.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-09 06:14:10.961033 fm91-0.0.14/fm91/__init__.py
--rw-r--r--   0        0        0       48 2023-07-09 07:05:18.792985 fm91-0.0.14/fm91/__main__.py
--rw-r--r--   0        0        0    10847 2023-07-09 07:19:35.248188 fm91-0.0.14/fm91/main.py
--rw-r--r--   0        0        0      429 2023-07-09 07:19:54.792063 fm91-0.0.14/pyproject.toml
--rw-r--r--   0        0        0     5312 2023-07-09 07:13:47.845484 fm91-0.0.14/README.md
--rw-r--r--   0        0        0     5457 1970-01-01 00:00:00.000000 fm91-0.0.14/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-09 06:14:10.961033 fm91-0.0.15/fm91/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-09 07:05:18.792985 fm91-0.0.15/fm91/__main__.py
+-rw-r--r--   0        0        0    10847 2023-07-09 07:19:35.248188 fm91-0.0.15/fm91/main.py
+-rw-r--r--   0        0        0      429 2023-07-09 07:21:35.726092 fm91-0.0.15/pyproject.toml
+-rw-r--r--   0        0        0     5648 2023-07-09 07:21:21.821375 fm91-0.0.15/README.md
+-rw-r--r--   0        0        0     5779 1970-01-01 00:00:00.000000 fm91-0.0.15/PKG-INFO
```

### Comparing `fm91-0.0.14/fm91/main.py` & `fm91-0.0.15/fm91/main.py`

 * *Files identical despite different names*

### Comparing `fm91-0.0.14/README.md` & `fm91-0.0.15/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `add-dependency`: Add a dependency to the requirements.txt...
 * `add-environment-variable`: Add an environment variable to the .env file.
 * `add-subdirectory`: Add a subdirectory to the Python path.
-* `create-handler`
+* `create-handler`: Create a new handler file.
 * `create-project`: Create a new project directory with the...
-* `create-route`
-* `create-structure`
-* `delete-handler`
+* `create-route`: Create a new route file.
+* `create-structure`: Create a new structure file.
+* `delete-handler`: Delete a handler file.
 * `delete-project`: Delete the project directory with the...
-* `delete-route`
-* `delete-structure`
+* `delete-route`: Delete a route file.
+* `delete-structure`: Delete a structure file.
 * `remove-dependency`: Remove a dependency from the...
 * `remove-environment-variable`: Remove an environment variable from the...
 * `remove-subdirectory`: Remove a subdirectory from the Python path.
 * `sync`: Impport the project's dependencies,...
 
 ## `fm91 add-dependency`
 
@@ -85,14 +85,17 @@
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 ## `fm91 create-handler`
 
+Create a new handler file.
+    
+
 **Usage**:
 
 ```console
 $ fm91 create-handler [OPTIONS] PROJECT_NAME HANDLER_NAME
 ```
 
 **Arguments**:
@@ -120,14 +123,16 @@
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 ## `fm91 create-route`
 
+Create a new route file.
+
 **Usage**:
 
 ```console
 $ fm91 create-route [OPTIONS] PROJECT_NAME ROUTE_NAME
 ```
 
 **Arguments**:
@@ -137,14 +142,16 @@
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 ## `fm91 create-structure`
 
+Create a new structure file.
+
 **Usage**:
 
 ```console
 $ fm91 create-structure [OPTIONS] PROJECT_NAME STRUCTURE_NAME
 ```
 
 **Arguments**:
@@ -154,14 +161,17 @@
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 ## `fm91 delete-handler`
 
+Delete a handler file.
+    
+
 **Usage**:
 
 ```console
 $ fm91 delete-handler [OPTIONS] PROJECT_NAME HANDLER_NAME
 ```
 
 **Arguments**:
@@ -189,14 +199,16 @@
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 ## `fm91 delete-route`
 
+Delete a route file.
+
 **Usage**:
 
 ```console
 $ fm91 delete-route [OPTIONS] PROJECT_NAME ROUTE_NAME
 ```
 
 **Arguments**:
@@ -206,14 +218,16 @@
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 ## `fm91 delete-structure`
 
+Delete a structure file.
+
 **Usage**:
 
 ```console
 $ fm91 delete-structure [OPTIONS] PROJECT_NAME STRUCTURE_NAME
 ```
 
 **Arguments**:
```

### Comparing `fm91-0.0.14/PKG-INFO` & `fm91-0.0.15/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fm91
-Version: 0.0.14
+Version: 0.0.15
 Summary: A simple fastapi manager
 Author: abirmunna
 Author-email: mtmunna82@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -27,22 +27,22 @@
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `add-dependency`: Add a dependency to the requirements.txt...
 * `add-environment-variable`: Add an environment variable to the .env file.
 * `add-subdirectory`: Add a subdirectory to the Python path.
-* `create-handler`
+* `create-handler`: Create a new handler file.
 * `create-project`: Create a new project directory with the...
-* `create-route`
-* `create-structure`
-* `delete-handler`
+* `create-route`: Create a new route file.
+* `create-structure`: Create a new structure file.
+* `delete-handler`: Delete a handler file.
 * `delete-project`: Delete the project directory with the...
-* `delete-route`
-* `delete-structure`
+* `delete-route`: Delete a route file.
+* `delete-structure`: Delete a structure file.
 * `remove-dependency`: Remove a dependency from the...
 * `remove-environment-variable`: Remove an environment variable from the...
 * `remove-subdirectory`: Remove a subdirectory from the Python path.
 * `sync`: Impport the project's dependencies,...
 
 ## `fm91 add-dependency`
 
@@ -99,14 +99,17 @@
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 ## `fm91 create-handler`
 
+Create a new handler file.
+    
+
 **Usage**:
 
 ```console
 $ fm91 create-handler [OPTIONS] PROJECT_NAME HANDLER_NAME
 ```
 
 **Arguments**:
@@ -134,14 +137,16 @@
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 ## `fm91 create-route`
 
+Create a new route file.
+
 **Usage**:
 
 ```console
 $ fm91 create-route [OPTIONS] PROJECT_NAME ROUTE_NAME
 ```
 
 **Arguments**:
@@ -151,14 +156,16 @@
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 ## `fm91 create-structure`
 
+Create a new structure file.
+
 **Usage**:
 
 ```console
 $ fm91 create-structure [OPTIONS] PROJECT_NAME STRUCTURE_NAME
 ```
 
 **Arguments**:
@@ -168,14 +175,17 @@
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 ## `fm91 delete-handler`
 
+Delete a handler file.
+    
+
 **Usage**:
 
 ```console
 $ fm91 delete-handler [OPTIONS] PROJECT_NAME HANDLER_NAME
 ```
 
 **Arguments**:
@@ -203,14 +213,16 @@
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 ## `fm91 delete-route`
 
+Delete a route file.
+
 **Usage**:
 
 ```console
 $ fm91 delete-route [OPTIONS] PROJECT_NAME ROUTE_NAME
 ```
 
 **Arguments**:
@@ -220,14 +232,16 @@
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 ## `fm91 delete-structure`
 
+Delete a structure file.
+
 **Usage**:
 
 ```console
 $ fm91 delete-structure [OPTIONS] PROJECT_NAME STRUCTURE_NAME
 ```
 
 **Arguments**:
```

