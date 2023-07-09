# Comparing `tmp/xmod-1.4.0.tar.gz` & `tmp/xmod-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmod-1.4.0.tar", max compression
+gzip compressed data, was "xmod-1.5.0.tar", max compression
```

## Comparing `xmod-1.4.0.tar` & `xmod-1.5.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-02-07 13:16:13.496824 xmod-1.4.0/LICENSE
--rw-r--r--   0        0        0     1003 2023-02-23 19:48:24.721916 xmod-1.4.0/README.md
--rw-r--r--   0        0        0      536 2023-02-23 19:58:33.129370 xmod-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     5760 2023-02-18 18:11:25.162690 xmod-1.4.0/xmod.py
--rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 xmod-1.4.0/setup.py
--rw-r--r--   0        0        0     1621 1970-01-01 00:00:00.000000 xmod-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 13:16:13.496824 xmod-1.5.0/LICENSE
+-rw-r--r--   0        0        0     1046 2023-03-09 20:44:30.536777 xmod-1.5.0/README.md
+-rw-r--r--   0        0        0      517 2023-07-09 14:49:10.504168 xmod-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5761 2023-03-08 12:32:21.553611 xmod-1.5.0/xmod.py
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 xmod-1.5.0/PKG-INFO
```

### Comparing `xmod-1.4.0/LICENSE` & `xmod-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmod-1.4.0/README.md` & `xmod-1.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# 🌱 Turn any object into a module 🌱
+
 Callable modules!  Indexable modules!?
 
 Ever wanted to call a module directly, or index it?  Or just sick of seeing
 `from foo import foo` in your examples?
 
 Give your module the awesome power of an object, or maybe just save a
 little typing, with `xmod`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xmod-1.4.0/pyproject.toml` & `xmod-1.5.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 target-version = ['py37']
 
 [tool.doks]
 auto = true
 
 [tool.poetry]
 name = "xmod"
-version = "1.4.0"
+version = "1.5.0"
 description = "🌱 Turn any object into a module 🌱"
 authors = ["Tom Ritchford <tom@swirly.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-dek = "^1.0.2"
+python = ">3.7"
+dek = "*"
 
 [tool.poetry.group.dev.dependencies]
-coverage = "^7.1.0"
-flake8 = "5.0.4"
-pytest = "^7.2.1"
+coverage = "*"
+flake8 = "*"
+pytest = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `xmod-1.4.0/xmod.py` & `xmod-1.5.0/xmod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-🌱 Turn any object into a module 🌱
+# 🌱 Turn any object into a module 🌱
 
 Callable modules!  Indexable modules!?
 
 Ever wanted to call a module directly, or index it?  Or just sick of seeing
 `from foo import foo` in your examples?
 
 Give your module the awesome power of an object, or maybe just save a
@@ -100,15 +100,15 @@
         If `None`, the default, add the extension if it's a callable, otherwise
         extend the module with all members of `extension`.
 
       mutable: If `True`, the attributes on the proxy are mutable and write
         through to the underlying module.  If `False`, the default, attributes
         on the proxy cannot be changed.
 
-      omit: A list of methods _not_ to delegate from the proxy to the extension.
+      omit: A list of methods _not_ to delegate from the proxy to the extension
 
         If `omit` is None, it defaults to `xmod.OMIT`, which seems to
         work well.
 
     Returns:
         `extension`, the original item that got decorated
     """
```

### Comparing `xmod-1.4.0/PKG-INFO` & `xmod-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: xmod
-Version: 1.4.0
+Version: 1.5.0
 Summary: 🌱 Turn any object into a module 🌱
 License: MIT
 Author: Tom Ritchford
 Author-email: tom@swirly.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dek (>=1.0.2,<2.0.0)
+Requires-Dist: dek
 Description-Content-Type: text/markdown
 
+# 🌱 Turn any object into a module 🌱
+
 Callable modules!  Indexable modules!?
 
 Ever wanted to call a module directly, or index it?  Or just sick of seeing
 `from foo import foo` in your examples?
 
 Give your module the awesome power of an object, or maybe just save a
 little typing, with `xmod`.
```

