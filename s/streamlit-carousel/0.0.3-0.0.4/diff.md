# Comparing `tmp/streamlit_carousel-0.0.3.tar.gz` & `tmp/streamlit_carousel-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_carousel-0.0.3.tar", last modified: Sat Jul  8 16:55:15 2023, max compression
+gzip compressed data, was "streamlit_carousel-0.0.4.tar", last modified: Sun Jul  9 20:51:43 2023, max compression
```

## Comparing `streamlit_carousel-0.0.3.tar` & `streamlit_carousel-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.273029 streamlit_carousel-0.0.3/
--rw-rw-rw-   0        0        0     1076 2023-07-03 17:27:05.000000 streamlit_carousel-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       53 2023-07-08 16:44:00.000000 streamlit_carousel-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4918 2023-07-08 16:55:15.272029 streamlit_carousel-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2997 2023-07-08 16:34:50.000000 streamlit_carousel-0.0.3/README.md
--rw-rw-rw-   0        0        0      907 2023-07-08 16:53:42.000000 streamlit_carousel-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-08 16:55:15.273029 streamlit_carousel-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      740 2023-07-08 16:53:38.000000 streamlit_carousel-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.219026 streamlit_carousel-0.0.3/streamlit_carousel/
--rw-rw-rw-   0        0        0     4866 2023-07-08 16:54:10.000000 streamlit_carousel-0.0.3/streamlit_carousel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.202027 streamlit_carousel-0.0.3/streamlit_carousel/carousel/
-drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.240027 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/
--rw-rw-rw-   0        0        0     1058 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/asset-manifest.json
--rw-rw-rw-   0        0        0     1946 2023-07-08 16:50:20.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/index.html
--rw-rw-rw-   0        0        0      660 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/precache-manifest.22851dbcebea0476fd3c97bc108bb6e8.js
--rw-rw-rw-   0        0        0     1183 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/service-worker.js
-drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.204027 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.245028 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/css/
--rw-rw-rw-   0        0        0   241050 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css
--rw-rw-rw-   0        0        0   583870 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css.map
-drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.270026 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/
--rw-rw-rw-   0        0        0   616599 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js
--rw-rw-rw-   0        0        0     2181 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1664534 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.map
--rw-rw-rw-   0        0        0     1351 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js
--rw-rw-rw-   0        0        0     3998 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js.map
--rw-rw-rw-   0        0        0     1578 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js
--rw-rw-rw-   0        0        0     8297 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js.map
-drwxrwxrwx   0        0        0        0 2023-07-08 16:55:15.231027 streamlit_carousel-0.0.3/streamlit_carousel.egg-info/
--rw-rw-rw-   0        0        0     4918 2023-07-08 16:55:15.000000 streamlit_carousel-0.0.3/streamlit_carousel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2023-07-08 16:55:15.000000 streamlit_carousel-0.0.3/streamlit_carousel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 16:55:15.000000 streamlit_carousel-0.0.3/streamlit_carousel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-08 16:55:15.000000 streamlit_carousel-0.0.3/streamlit_carousel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2023-07-08 16:55:15.000000 streamlit_carousel-0.0.3/streamlit_carousel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-08 16:55:15.000000 streamlit_carousel-0.0.3/streamlit_carousel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 20:51:43.604789 streamlit_carousel-0.0.4/
+-rw-rw-rw-   0        0        0     1076 2023-07-03 17:27:05.000000 streamlit_carousel-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       53 2023-07-08 16:44:00.000000 streamlit_carousel-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4918 2023-07-09 20:51:43.604789 streamlit_carousel-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2997 2023-07-08 16:34:50.000000 streamlit_carousel-0.0.4/README.md
+-rw-rw-rw-   0        0        0      907 2023-07-09 20:50:48.000000 streamlit_carousel-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 20:51:43.604789 streamlit_carousel-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      740 2023-07-09 20:50:46.000000 streamlit_carousel-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:51:43.557963 streamlit_carousel-0.0.4/streamlit_carousel/
+-rw-rw-rw-   0        0        0     4838 2023-07-09 20:48:14.000000 streamlit_carousel-0.0.4/streamlit_carousel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:51:43.542491 streamlit_carousel-0.0.4/streamlit_carousel/carousel/
+drwxrwxrwx   0        0        0        0 2023-07-09 20:51:43.573541 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/
+-rw-rw-rw-   0        0        0     1058 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     1946 2023-07-08 16:50:20.000000 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/index.html
+-rw-rw-rw-   0        0        0      660 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/precache-manifest.22851dbcebea0476fd3c97bc108bb6e8.js
+-rw-rw-rw-   0        0        0     1183 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/service-worker.js
+drwxrwxrwx   0        0        0        0 2023-07-09 20:51:43.542491 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-09 20:51:43.573541 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/css/
+-rw-rw-rw-   0        0        0   241050 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css
+-rw-rw-rw-   0        0        0   583870 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-07-09 20:51:43.604789 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/js/
+-rw-rw-rw-   0        0        0   616599 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js
+-rw-rw-rw-   0        0        0     2181 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1664534 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.map
+-rw-rw-rw-   0        0        0     1351 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js
+-rw-rw-rw-   0        0        0     3998 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js.map
+-rw-rw-rw-   0        0        0     1578 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js
+-rw-rw-rw-   0        0        0     8297 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js.map
+drwxrwxrwx   0        0        0        0 2023-07-09 20:51:43.557963 streamlit_carousel-0.0.4/streamlit_carousel.egg-info/
+-rw-rw-rw-   0        0        0     4918 2023-07-09 20:51:43.000000 streamlit_carousel-0.0.4/streamlit_carousel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2023-07-09 20:51:43.000000 streamlit_carousel-0.0.4/streamlit_carousel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 20:51:43.000000 streamlit_carousel-0.0.4/streamlit_carousel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-09 20:51:43.000000 streamlit_carousel-0.0.4/streamlit_carousel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2023-07-09 20:51:43.000000 streamlit_carousel-0.0.4/streamlit_carousel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-09 20:51:43.000000 streamlit_carousel-0.0.4/streamlit_carousel.egg-info/top_level.txt
```

### Comparing `streamlit_carousel-0.0.3/LICENSE` & `streamlit_carousel-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.3/PKG-INFO` & `streamlit_carousel-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_carousel
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Streamlit implementation of the React Bootstrap Carousel component.
 Home-page: https://github.com/thomasbs17/streamlit-contributions/bootstrap_carousel
 Author: Thomas Bouamoud
 Author-email: Thomas Bouamoud <thomas.bouamoud@gmail.com>
 License: Copyright (c) 2023 Thomas Bouamoud
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `streamlit_carousel-0.0.3/README.md` & `streamlit_carousel-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.3/pyproject.toml` & `streamlit_carousel-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit_carousel"
-version = "0.0.3"
+version = "0.0.4"
 description = "A Streamlit implementation of the React Bootstrap Carousel component."
 readme = "README.md"
 authors = [{ name = "Thomas Bouamoud", email = "thomas.bouamoud@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `streamlit_carousel-0.0.3/setup.py` & `streamlit_carousel-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit_carousel",
-    version="0.0.3",
+    version="0.0.4",
     author="Thomas Bouamoud",
     author_email="thomas.bouamoud@gmail.com",
     description="A Streamlit implementation of the React Bootstrap Carousel component.",
     long_description="https://react-bootstrap.netlify.app/docs/components/carousel/",
     long_description_content_type="text/plain",
     url="https://github.com/thomasbs17/streamlit-contributions/bootstrap_carousel",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel/__init__.py` & `streamlit_carousel-0.0.4/streamlit_carousel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     )
 
 
 class Item(TypedDict):
     title: str
     text: str
     img: str
-    interval: int | None
 
 
 def validate_items(items: List[Item]) -> List[Item]:
     for item in items:
         if "img" not in item:
             raise ValueError(
                 "Each item should include an 'img' key referring to an image url"
@@ -43,27 +42,27 @@
                 "Each item should include a 'title' key referring to a string variable"
             )
         if "text" not in item:
             raise ValueError(
                 "Each item should include a 'text' key referring to a string variable"
             )
         if "interval" not in item:
-            item["interval"] = False
+            item["interval"] = None
     return items
 
 
 def carousel(
     items: List[Item],
     slide: bool = True,
     fade: bool = False,
     controls: bool = True,
     indicators: bool = True,
     interval: int = 1000,
     pause: str = None,
-    wrap: bool = False,
+    wrap: bool = True,
     height: int = 400,
     width: float = 1,
     key=None,
 ) -> None:
     """
     Defines a Carousel component in the React Bootstrap framework.
```

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/asset-manifest.json` & `streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/index.html` & `streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/precache-manifest.22851dbcebea0476fd3c97bc108bb6e8.js` & `streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/precache-manifest.22851dbcebea0476fd3c97bc108bb6e8.js`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/service-worker.js` & `streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css` & `streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css.map` & `streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js` & `streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.LICENSE.txt` & `streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.map` & `streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js` & `streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js.map` & `streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js` & `streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js.map` & `streamlit_carousel-0.0.4/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js.map`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel.egg-info/PKG-INFO` & `streamlit_carousel-0.0.4/streamlit_carousel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-carousel
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Streamlit implementation of the React Bootstrap Carousel component.
 Home-page: https://github.com/thomasbs17/streamlit-contributions/bootstrap_carousel
 Author: Thomas Bouamoud
 Author-email: Thomas Bouamoud <thomas.bouamoud@gmail.com>
 License: Copyright (c) 2023 Thomas Bouamoud
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `streamlit_carousel-0.0.3/streamlit_carousel.egg-info/SOURCES.txt` & `streamlit_carousel-0.0.4/streamlit_carousel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

