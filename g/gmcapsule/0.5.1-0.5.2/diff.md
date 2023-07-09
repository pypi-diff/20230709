# Comparing `tmp/gmcapsule-0.5.1.tar.gz` & `tmp/gmcapsule-0.5.2.tar.gz`

## Comparing `gmcapsule-0.5.1.tar` & `gmcapsule-0.5.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/example.ini
--rw-r--r--   0        0        0    21706 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/gmcapsule/__init__.py
--rw-r--r--   0        0        0    33433 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/gmcapsule/gemini.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/gmcapsule/markdown.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/gmcapsule/modules/10_rewrite.py
--rwxr-xr-x   0        0        0    18619 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/gmcapsule/modules/80_gitview.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/gmcapsule/modules/90_cgi.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/gmcapsule/modules/99_static.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/.gitignore
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/README.md
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 gmcapsule-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/example.ini
+-rw-r--r--   0        0        0    21706 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/gmcapsule/__init__.py
+-rw-r--r--   0        0        0    33471 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/gmcapsule/gemini.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/gmcapsule/markdown.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/gmcapsule/modules/10_rewrite.py
+-rwxr-xr-x   0        0        0    18619 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/gmcapsule/modules/80_gitview.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/gmcapsule/modules/90_cgi.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/gmcapsule/modules/99_static.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/.gitignore
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/README.md
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/PKG-INFO
```

### Comparing `gmcapsule-0.5.1/example.ini` & `gmcapsule-0.5.2/example.ini`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.1/gmcapsule/__init__.py` & `gmcapsule-0.5.2/gmcapsule/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,15 +491,15 @@
 import subprocess
 from pathlib import Path
 
 from .gemini import Server, Cache, Context, Identity
 from .markdown import to_gemtext as markdown_to_gemtext
 
 
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 __all__ = [
     'Config', 'Cache', 'Context', 'Identity',
     'get_mime_type', 'markdown_to_gemtext'
 ]
 
 
 class Config:
```

### Comparing `gmcapsule-0.5.1/gmcapsule/gemini.py` & `gmcapsule-0.5.2/gmcapsule/gemini.py`

 * *Files 0% similar despite different names*

```diff
@@ -782,14 +782,15 @@
         self.jobs = job_queue
         self.results = result_queues
         self.context = None
 
     def _run(self):
         self.context = Context(self.cfg)
         self.context.load_modules()
+        self.context.set_quiet(False)
 
         # Wait for request processing jobs.
         try:
             while True:
                 job_id, request, queue_id = self.jobs.get()
                 if job_id is None:
                     break
```

### Comparing `gmcapsule-0.5.1/gmcapsule/markdown.py` & `gmcapsule-0.5.2/gmcapsule/markdown.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.1/gmcapsule/modules/10_rewrite.py` & `gmcapsule-0.5.2/gmcapsule/modules/10_rewrite.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,17 @@
             req.num_rewrites += 1
         else:
             req.num_rewrites = 1
         if req.num_rewrites == 100:
             return 40, "Stuck in rewrite loop: " + req.url()
 
         self.context.print("[rewrite]", old_path, "->", req.path)
-        return self.context.call_entrypoint(req)[0]
+        status, meta, path, _ = self.context.call_entrypoint(req)
+
+        return (status, meta, path)
 
 
 class Responder:
     def __init__(self, code, meta):
         self.code = code
         self.meta = meta
```

### Comparing `gmcapsule-0.5.1/gmcapsule/modules/80_gitview.py` & `gmcapsule-0.5.2/gmcapsule/modules/80_gitview.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.1/gmcapsule/modules/90_cgi.py` & `gmcapsule-0.5.2/gmcapsule/modules/90_cgi.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.1/gmcapsule/modules/99_static.py` & `gmcapsule-0.5.2/gmcapsule/modules/99_static.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.1/README.md` & `gmcapsule-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,18 @@
 * API change: Extension modules get initialized separately in each worker thread. Instead of a `Capsule`, the extension module `init` method is passed a `Context`. `Capsule` is no longer available as global state.
 * API change: `Identity` no longer contains OpenSSL objects for the certificate and public key. Instead, they are provided as serialized in DER format.
 
 v0.5.1:
 
 * `Identity` class is available when importing the `gmcapsule` module.
 
+v0.5.2:
+
+* Fixed error in the "rewrite" module (Codeberg PR #1).
+
 ### v0.4
 
 * Added built-in module "rewrite" that matches regular expressions against the request path and can rewrite the path or return a custom status for redirection, "Gone" messages, or other exceptional situations.
 * Extension module load order is determined after locating all modules from all directories. Previously, the order was local to each directory.
 * Added a new configuration section `[priority]` for overriding default module priorities determined from file names. This is useful for changing the priority of the built-in modules.
 
 v0.4.1:
```

### Comparing `gmcapsule-0.5.1/pyproject.toml` & `gmcapsule-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.1/PKG-INFO` & `gmcapsule-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmcapsule
-Version: 0.5.1
+Version: 0.5.2
 Summary: Extensible Gemini/Titan server
 Project-URL: Home-page, https://geminispace.org/gmcapsule/
 Project-URL: Documentation, https://geminispace.org/gmcapsule/gmcapsule.html
 Project-URL: Source, https://codeberg.org/skyjake/gmcapsule
 Project-URL: Issues, https://codeberg.org/skyjake/gmcapsule/issues
 Author-email: Jaakko Keränen <jaakko.keranen@iki.fi>
 Keywords: gemini,internet,server,titan
@@ -77,14 +77,18 @@
 * API change: Extension modules get initialized separately in each worker thread. Instead of a `Capsule`, the extension module `init` method is passed a `Context`. `Capsule` is no longer available as global state.
 * API change: `Identity` no longer contains OpenSSL objects for the certificate and public key. Instead, they are provided as serialized in DER format.
 
 v0.5.1:
 
 * `Identity` class is available when importing the `gmcapsule` module.
 
+v0.5.2:
+
+* Fixed error in the "rewrite" module (Codeberg PR #1).
+
 ### v0.4
 
 * Added built-in module "rewrite" that matches regular expressions against the request path and can rewrite the path or return a custom status for redirection, "Gone" messages, or other exceptional situations.
 * Extension module load order is determined after locating all modules from all directories. Previously, the order was local to each directory.
 * Added a new configuration section `[priority]` for overriding default module priorities determined from file names. This is useful for changing the priority of the built-in modules.
 
 v0.4.1:
```

