# Comparing `tmp/dynamic-service-1.4.0.tar.gz` & `tmp/dynamic-service-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-service-1.4.0.tar", last modified: Sat Jul  8 16:06:07 2023, max compression
+gzip compressed data, was "dynamic-service-1.4.1.tar", last modified: Sat Jul  8 16:23:04 2023, max compression
```

## Comparing `dynamic-service-1.4.0.tar` & `dynamic-service-1.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.432208 dynamic-service-1.4.0/
--rw-rw-rw-   0        0        0      236 2023-07-08 16:06:07.000000 dynamic-service-1.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2023 2023-07-08 16:06:07.431201 dynamic-service-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.4.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.4.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.378543 dynamic-service-1.4.0/dynamic_service/
--rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.4.0/dynamic_service/base.py
-drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.416293 dynamic-service-1.4.0/dynamic_service/endpoints/
--rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.4.0/dynamic_service/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.4.0/dynamic_service/endpoints/data.py
--rw-rw-rw-   0        0        0     8954 2023-07-08 15:55:29.000000 dynamic-service-1.4.0/dynamic_service/endpoints/engine.py
--rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.4.0/dynamic_service/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.4.0/dynamic_service/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.426185 dynamic-service-1.4.0/dynamic_service/service/
--rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.4.0/dynamic_service/service/__init__.py
--rw-rw-rw-   0        0        0    20599 2023-07-08 16:05:28.000000 dynamic-service-1.4.0/dynamic_service/service/rest.py
--rw-rw-rw-   0        0        0     3387 2023-07-08 10:41:33.000000 dynamic-service-1.4.0/dynamic_service/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.368055 dynamic-service-1.4.0/dynamic_service/source/
-drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.368055 dynamic-service-1.4.0/dynamic_service/source/assets/
-drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.430215 dynamic-service-1.4.0/dynamic_service/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.4.0/dynamic_service/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.4.0/dynamic_service/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-07-08 16:06:07.392599 dynamic-service-1.4.0/dynamic_service.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-07-08 16:06:07.000000 dynamic-service-1.4.0/dynamic_service.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-07-08 16:06:07.000000 dynamic-service-1.4.0/dynamic_service.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 16:06:07.000000 dynamic-service-1.4.0/dynamic_service.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-07-08 16:06:07.000000 dynamic-service-1.4.0/dynamic_service.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-08 16:06:07.000000 dynamic-service-1.4.0/dynamic_service.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      627 2023-07-08 16:06:07.000000 dynamic-service-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       92 2023-07-08 15:54:50.000000 dynamic-service-1.4.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       76 2023-07-08 15:54:50.000000 dynamic-service-1.4.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 16:06:07.432208 dynamic-service-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-07-08 16:06:01.000000 dynamic-service-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:23:04.811273 dynamic-service-1.4.1/
+-rw-rw-rw-   0        0        0      236 2023-07-08 16:23:04.000000 dynamic-service-1.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-07-08 16:23:04.810275 dynamic-service-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.4.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.4.1/build.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:23:04.792130 dynamic-service-1.4.1/dynamic_service/
+-rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.4.1/dynamic_service/base.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:23:04.806299 dynamic-service-1.4.1/dynamic_service/endpoints/
+-rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.4.1/dynamic_service/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.4.1/dynamic_service/endpoints/data.py
+-rw-rw-rw-   0        0        0     8954 2023-07-08 15:55:29.000000 dynamic-service-1.4.1/dynamic_service/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.4.1/dynamic_service/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.4.1/dynamic_service/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:23:04.808274 dynamic-service-1.4.1/dynamic_service/service/
+-rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.4.1/dynamic_service/service/__init__.py
+-rw-rw-rw-   0        0        0    20817 2023-07-08 16:22:39.000000 dynamic-service-1.4.1/dynamic_service/service/rest.py
+-rw-rw-rw-   0        0        0     3419 2023-07-08 16:21:14.000000 dynamic-service-1.4.1/dynamic_service/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:23:04.786126 dynamic-service-1.4.1/dynamic_service/source/
+drwxrwxrwx   0        0        0        0 2023-07-08 16:23:04.787137 dynamic-service-1.4.1/dynamic_service/source/assets/
+drwxrwxrwx   0        0        0        0 2023-07-08 16:23:04.809274 dynamic-service-1.4.1/dynamic_service/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.4.1/dynamic_service/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.4.1/dynamic_service/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-07-08 16:23:04.802275 dynamic-service-1.4.1/dynamic_service.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-08 16:23:04.000000 dynamic-service-1.4.1/dynamic_service.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-07-08 16:23:04.000000 dynamic-service-1.4.1/dynamic_service.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 16:23:04.000000 dynamic-service-1.4.1/dynamic_service.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-07-08 16:23:04.000000 dynamic-service-1.4.1/dynamic_service.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-08 16:23:04.000000 dynamic-service-1.4.1/dynamic_service.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      627 2023-07-08 16:23:04.000000 dynamic-service-1.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       92 2023-07-08 15:54:50.000000 dynamic-service-1.4.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       76 2023-07-08 15:54:50.000000 dynamic-service-1.4.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 16:23:04.811273 dynamic-service-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-07-08 16:23:01.000000 dynamic-service-1.4.1/setup.py
```

### Comparing `dynamic-service-1.4.0/PKG-INFO` & `dynamic-service-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.4.0
+Version: 1.4.1
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.4.0/README.md` & `dynamic-service-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.0/build.py` & `dynamic-service-1.4.1/build.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.0/dynamic_service/base.py` & `dynamic-service-1.4.1/dynamic_service/base.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.0/dynamic_service/endpoints/data.py` & `dynamic-service-1.4.1/dynamic_service/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.0/dynamic_service/endpoints/engine.py` & `dynamic-service-1.4.1/dynamic_service/endpoints/engine.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.0/dynamic_service/endpoints/exceptions.py` & `dynamic-service-1.4.1/dynamic_service/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.0/dynamic_service/endpoints/process.py` & `dynamic-service-1.4.1/dynamic_service/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.0/dynamic_service/service/rest.py` & `dynamic-service-1.4.1/dynamic_service/service/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,20 @@
     ICON = icons() + "\\icon.ico"
     VERSION = "0.0.0"
     DESCRIPTION = ""
     NAME = "Dynamic-Service"
 
     __modifiers__ = Modifiers(excluded=["app", "server"])
 
+    __slots__ = (
+        "name", "version", "endpoints", "description", "icon",
+        "home", "debug", "app", "service", "_root", "server",
+        "_serving_process", "_running_parameters", "_serving"
+    )
+
     def __init__(
             self,
             name: Optional[str] = None,
             version: Optional[str] = None,
             endpoints: Optional[EndpointsContainer] = None,
             root: Optional[str] = None,
             description: Optional[str] = None,
```

### Comparing `dynamic-service-1.4.0/dynamic_service/service/sockets.py` & `dynamic-service-1.4.1/dynamic_service/service/sockets.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     >>> service = SocketService(
     >>>     endpoints=[endpoint]
     >>> )
     >>>
     >>> service.run()
     """
 
+    __slots__ = "endpoints",
+
     def __init__(
             self,
             connection: Optional[Socket] = None, *,
             host: Optional[Host] = None,
             port: Optional[Port] = None,
             endpoints: Optional[EndpointsContainer] = None
     ) -> None:
```

### Comparing `dynamic-service-1.4.0/dynamic_service/source/assets/icon/icon.ico` & `dynamic-service-1.4.1/dynamic_service/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.0/dynamic_service/source/assets/icon/icon.png` & `dynamic-service-1.4.1/dynamic_service/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.0/dynamic_service.egg-info/PKG-INFO` & `dynamic-service-1.4.1/dynamic_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.4.0
+Version: 1.4.1
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.4.0/dynamic_service.egg-info/SOURCES.txt` & `dynamic-service-1.4.1/dynamic_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.4.0/pyproject.toml` & `dynamic-service-1.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'dynamic-service'
-version = '1.4.0'
+version = '1.4.1'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `dynamic-service-1.4.0/setup.py` & `dynamic-service-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "dynamic_service/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='dynamic-service',
-        version='1.4.0',
+        version='1.4.1',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

