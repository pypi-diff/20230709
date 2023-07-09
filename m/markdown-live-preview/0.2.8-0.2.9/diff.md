# Comparing `tmp/markdown-live-preview-0.2.8.tar.gz` & `tmp/markdown-live-preview-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-live-preview-0.2.8.tar", last modified: Wed Jun 23 07:28:54 2021, max compression
+gzip compressed data, was "markdown-live-preview-0.2.9.tar", last modified: Wed Jun 23 07:37:50 2021, max compression
```

## Comparing `markdown-live-preview-0.2.8.tar` & `markdown-live-preview-0.2.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 07:28:54.666904 markdown-live-preview-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2021-06-23 07:28:54.666904 markdown-live-preview-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      954 2021-06-23 07:28:06.000000 markdown-live-preview-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 07:28:54.662904 markdown-live-preview-0.2.8/markdown_live_preview/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-23 07:28:06.000000 markdown-live-preview-0.2.8/markdown_live_preview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-06-23 07:28:06.000000 markdown-live-preview-0.2.8/markdown_live_preview/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 07:28:54.662904 markdown-live-preview-0.2.8/markdown_live_preview/js/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-23 07:28:06.000000 markdown-live-preview-0.2.8/markdown_live_preview/js/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 07:28:54.666904 markdown-live-preview-0.2.8/markdown_live_preview/server/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-23 07:28:06.000000 markdown-live-preview-0.2.8/markdown_live_preview/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-06-23 07:28:06.000000 markdown-live-preview-0.2.8/markdown_live_preview/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-06-23 07:28:06.000000 markdown-live-preview-0.2.8/markdown_live_preview/server/consts.py
--rw-r--r--   0 runner    (1001) docker     (121)     3316 2021-06-23 07:28:06.000000 markdown-live-preview-0.2.8/markdown_live_preview/server/html_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     2472 2021-06-23 07:28:06.000000 markdown-live-preview-0.2.8/markdown_live_preview/server/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2021-06-23 07:28:06.000000 markdown-live-preview-0.2.8/markdown_live_preview/server/reconciliate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2149 2021-06-23 07:28:06.000000 markdown-live-preview-0.2.8/markdown_live_preview/server/render.py
--rw-r--r--   0 runner    (1001) docker     (121)     3014 2021-06-23 07:28:06.000000 markdown-live-preview-0.2.8/markdown_live_preview/server/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2021-06-23 07:28:06.000000 markdown-live-preview-0.2.8/markdown_live_preview/server/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 07:28:54.662904 markdown-live-preview-0.2.8/markdown_live_preview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2021-06-23 07:28:54.000000 markdown-live-preview-0.2.8/markdown_live_preview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      723 2021-06-23 07:28:54.000000 markdown-live-preview-0.2.8/markdown_live_preview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-23 07:28:54.000000 markdown-live-preview-0.2.8/markdown_live_preview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-06-23 07:28:54.000000 markdown-live-preview-0.2.8/markdown_live_preview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-06-23 07:28:54.000000 markdown-live-preview-0.2.8/markdown_live_preview.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 07:28:54.666904 markdown-live-preview-0.2.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)       67 2021-06-23 07:28:06.000000 markdown-live-preview-0.2.8/scripts/mlp
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-23 07:28:54.666904 markdown-live-preview-0.2.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      952 2021-06-23 07:28:06.000000 markdown-live-preview-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 07:37:50.074730 markdown-live-preview-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2021-06-23 07:37:50.074730 markdown-live-preview-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      954 2021-06-23 07:36:58.000000 markdown-live-preview-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 07:37:50.074730 markdown-live-preview-0.2.9/markdown_live_preview/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-23 07:36:58.000000 markdown-live-preview-0.2.9/markdown_live_preview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2021-06-23 07:36:58.000000 markdown-live-preview-0.2.9/markdown_live_preview/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 07:37:50.074730 markdown-live-preview-0.2.9/markdown_live_preview/js/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-23 07:36:58.000000 markdown-live-preview-0.2.9/markdown_live_preview/js/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 07:37:50.074730 markdown-live-preview-0.2.9/markdown_live_preview/server/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-23 07:36:58.000000 markdown-live-preview-0.2.9/markdown_live_preview/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2021-06-23 07:36:58.000000 markdown-live-preview-0.2.9/markdown_live_preview/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-06-23 07:36:58.000000 markdown-live-preview-0.2.9/markdown_live_preview/server/consts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3325 2021-06-23 07:36:58.000000 markdown-live-preview-0.2.9/markdown_live_preview/server/html_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2472 2021-06-23 07:36:58.000000 markdown-live-preview-0.2.9/markdown_live_preview/server/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1545 2021-06-23 07:36:58.000000 markdown-live-preview-0.2.9/markdown_live_preview/server/reconciliate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2149 2021-06-23 07:36:58.000000 markdown-live-preview-0.2.9/markdown_live_preview/server/render.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3014 2021-06-23 07:36:58.000000 markdown-live-preview-0.2.9/markdown_live_preview/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1495 2021-06-23 07:36:58.000000 markdown-live-preview-0.2.9/markdown_live_preview/server/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 07:37:50.074730 markdown-live-preview-0.2.9/markdown_live_preview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2021-06-23 07:37:49.000000 markdown-live-preview-0.2.9/markdown_live_preview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2021-06-23 07:37:50.000000 markdown-live-preview-0.2.9/markdown_live_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-23 07:37:49.000000 markdown-live-preview-0.2.9/markdown_live_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2021-06-23 07:37:49.000000 markdown-live-preview-0.2.9/markdown_live_preview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-06-23 07:37:49.000000 markdown-live-preview-0.2.9/markdown_live_preview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-23 07:37:50.074730 markdown-live-preview-0.2.9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       67 2021-06-23 07:36:58.000000 markdown-live-preview-0.2.9/scripts/mlp
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-23 07:37:50.074730 markdown-live-preview-0.2.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)      952 2021-06-23 07:36:58.000000 markdown-live-preview-0.2.9/setup.py
```

### Comparing `markdown-live-preview-0.2.8/PKG-INFO` & `markdown-live-preview-0.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-live-preview
-Version: 0.2.8
+Version: 0.2.9
 Summary: live web preview of markdown docs
 Home-page: https://github.com/ms-jpq/markdown-live-preview
 Author: ms-jpq
 Author-email: github@bigly.dog
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8.0
```

### Comparing `markdown-live-preview-0.2.8/README.md` & `markdown-live-preview-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `markdown-live-preview-0.2.8/markdown_live_preview/server/html_to_dict.py` & `markdown-live-preview-0.2.9/markdown_live_preview/server/html_to_dict.py`

 * *Files 14% similar despite different names*

```diff
@@ -111,21 +111,22 @@
 def unparse(node: Node) -> str:
     attrs = " ".join(
         f'{k}="{v}"' if v else k
         for k, v in chain(
             node.attrs.items(), (("diff", str(True)),) if node.diff else ()
         )
     )
-    opening = f"<{node.tag} {attrs}>"
-    closing = f"</{node.tag}>"
-    middle = "".join(
+    kids = "".join(
         unparse(child)
         if isinstance(child, Node)
         else (
             f'<span diff="{True}">{escape(child.text)}</span>'
             if child.diff
             else escape(child.text)
         )
         for child in node.children
     )
-    return f"{opening}{middle}{closing}"
+    if kids:
+        return f"<{node.tag} {attrs}>{kids}</{node.tag}>"
+    else:
+        return f"<{node.tag} {attrs}/>"
```

### Comparing `markdown-live-preview-0.2.8/markdown_live_preview/server/main.py` & `markdown-live-preview-0.2.9/markdown_live_preview/server/main.py`

 * *Files identical despite different names*

### Comparing `markdown-live-preview-0.2.8/markdown_live_preview/server/reconciliate.py` & `markdown-live-preview-0.2.9/markdown_live_preview/server/reconciliate.py`

 * *Files identical despite different names*

### Comparing `markdown-live-preview-0.2.8/markdown_live_preview/server/render.py` & `markdown-live-preview-0.2.9/markdown_live_preview/server/render.py`

 * *Files identical despite different names*

### Comparing `markdown-live-preview-0.2.8/markdown_live_preview/server/server.py` & `markdown-live-preview-0.2.9/markdown_live_preview/server/server.py`

 * *Files identical despite different names*

### Comparing `markdown-live-preview-0.2.8/markdown_live_preview/server/watch.py` & `markdown-live-preview-0.2.9/markdown_live_preview/server/watch.py`

 * *Files identical despite different names*

### Comparing `markdown-live-preview-0.2.8/markdown_live_preview.egg-info/PKG-INFO` & `markdown-live-preview-0.2.9/markdown_live_preview.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-live-preview
-Version: 0.2.8
+Version: 0.2.9
 Summary: live web preview of markdown docs
 Home-page: https://github.com/ms-jpq/markdown-live-preview
 Author: ms-jpq
 Author-email: github@bigly.dog
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8.0
```

### Comparing `markdown-live-preview-0.2.8/markdown_live_preview.egg-info/SOURCES.txt` & `markdown-live-preview-0.2.9/markdown_live_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `markdown-live-preview-0.2.8/setup.py` & `markdown-live-preview-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     for pkg in packages
 }
 install_requires = Path("requirements.txt").read_text().splitlines()
 
 setup(
     name="markdown-live-preview",
     python_requires=">=3.8.0",
-    version="0.2.8",
+    version="0.2.9",
     description="live web preview of markdown docs",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     author="ms-jpq",
     author_email="github@bigly.dog",
     url="https://github.com/ms-jpq/markdown-live-preview",
     packages=packages,
```

