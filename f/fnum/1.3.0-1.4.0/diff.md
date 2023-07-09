# Comparing `tmp/fnum-1.3.0-py3-none-any.whl.zip` & `tmp/fnum-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5857 bytes, number of entries: 11
--rw-r--r--  2.0 unx     4398 b- defN 23-Jul-09 09:20 fnum/__init__.py
--rw-r--r--  2.0 unx       29 b- defN 23-Jul-09 09:20 fnum/__main__.py
--rw-r--r--  2.0 unx     2116 b- defN 23-Jul-09 09:20 fnum/cli.py
--rw-r--r--  2.0 unx       41 b- defN 23-Jul-09 09:20 fnum/exceptions.py
--rw-r--r--  2.0 unx     2116 b- defN 23-Jul-09 09:20 fnum/metadata.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-09 09:20 fnum-1.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1038 b- defN 23-Jul-09 09:20 fnum-1.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 09:20 fnum-1.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-09 09:20 fnum-1.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-09 09:20 fnum-1.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      820 b- defN 23-Jul-09 09:20 fnum-1.3.0.dist-info/RECORD
-11 files, 11762 bytes uncompressed, 4483 bytes compressed:  61.9%
+Zip file size: 5953 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     4271 b- defN 23-Jul-09 19:55 fnum/__init__.py
+-rw-r--r--  2.0 unx       29 b- defN 23-Jul-09 19:55 fnum/__main__.py
+-rw-r--r--  2.0 unx     2511 b- defN 23-Jul-09 19:55 fnum/cli.py
+-rw-r--r--  2.0 unx       41 b- defN 23-Jul-09 19:55 fnum/exceptions.py
+-rw-r--r--  2.0 unx     2116 b- defN 23-Jul-09 19:55 fnum/metadata.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-09 19:56 fnum-1.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1038 b- defN 23-Jul-09 19:56 fnum-1.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 19:56 fnum-1.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-09 19:56 fnum-1.4.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-09 19:56 fnum-1.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jul-09 19:56 fnum-1.4.0.dist-info/RECORD
+11 files, 12030 bytes uncompressed, 4579 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: fnum/exceptions.py
 Comment: 
 
 Filename: fnum/metadata.py
 Comment: 
 
-Filename: fnum-1.3.0.dist-info/LICENSE
+Filename: fnum-1.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: fnum-1.3.0.dist-info/METADATA
+Filename: fnum-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: fnum-1.3.0.dist-info/WHEEL
+Filename: fnum-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: fnum-1.3.0.dist-info/entry_points.txt
+Filename: fnum-1.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: fnum-1.3.0.dist-info/top_level.txt
+Filename: fnum-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fnum-1.3.0.dist-info/RECORD
+Filename: fnum-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fnum/__init__.py

```diff
@@ -1,20 +1,24 @@
+import logging
 from pathlib import Path
 from contextlib import contextmanager
 from imeta import ImageMetadata
 
 from .exceptions import FnumException
 from .metadata import FnumMetadata, FnumMax
 
 
-__version__ = "1.3.0"
+__version__ = "1.4.0"
 
+_log = logging.getLogger(__name__)
 
-def number_files(dirpath, suffixes, progressbar=None, include_imeta=False):
+
+def number_files(dirpath, suffixes, include_imeta=False):
     dirpath = Path(dirpath)
+    _log.info("Analyzing files...")
 
     try:
         metadata = FnumMetadata.from_file(dirpath)
         regen_meta = False
     except FileNotFoundError:
         metadata = FnumMetadata.get_default()
         regen_meta = True
@@ -50,14 +54,16 @@
             continue
 
         if filenum > nummax:
             nummax = filenum
 
     def move_file(filepath):
         newpath = numpath(filepath.suffix)
+        if newpath.exists():
+            raise FnumException("Can't override existing file {newpath.name}")
 
         try:
             order_index = metadata.order.index(filepath.name)
             metadata.order[order_index] = newpath.name
         except ValueError:
             metadata.order.append(newpath.name)
         try:
@@ -107,33 +113,22 @@
         filepath = used_suffixes[0]
         move_file(filepath)
         num += 1
         if int(filepath.stem) == nummax:
             break
 
     # Find new files
-    files = list(dirpath.iterdir())
-    if not progressbar:
-
-        @contextmanager
-        def noop_progressbar(*args, **kwargs):
-            yield args[0]
-
-        progressbar = noop_progressbar
-    with progressbar(
-        files, length=len(files), label="Processing files", update_min_steps=10
-    ) as bar:
-        for filepath in bar:
-            if not filepath.is_file() or filepath.suffix not in suffixes:
+    _log.info("Processing files...")
+    for filepath in dirpath.iterdir():
+        if not filepath.is_file() or filepath.suffix not in suffixes:
+            continue
+        try:
+            if int(filepath.stem) <= num:
                 continue
+        except ValueError:
+            pass
 
-            try:
-                if int(filepath.stem) <= num:
-                    continue
-            except ValueError:
-                pass
-
-            move_file(filepath)
-            num += 1
+        move_file(filepath)
+        num += 1
 
     metadata.max = num - 1
     return metadata
```

## fnum/cli.py

```diff
@@ -1,14 +1,23 @@
 import sys
 import click
+import logging
+import io
 
-from . import __version__, number_files
+from . import __version__, number_files, _log
 from .exceptions import FnumException
 
 
+class _ClickFormatter(logging.Formatter):
+    def format(self, record):
+        log_str = super().format(record)
+        click.echo(log_str)
+        return log_str
+
+
 @click.command(
     help="""
 Renames files in a directory using sequential integers.\n
 Suffixes is a comma separated list of file extensions to rename (eg. .jpg,.gif).\n
 Dirpath is a directory to rename files in.
 """,
     context_settings={
@@ -45,23 +54,29 @@
 )
 def cli(**kwargs):
     dirpath = kwargs["dirpath"]
     if "/" in kwargs["suffixes"]:
         click.echo("Suffixes contains a '/', did you mean ','?", err=True)
     suffixes = kwargs["suffixes"].split(",")
 
-    click.echo("Analyzing files...")
+    _log.setLevel(logging.INFO)
+    handler = logging.StreamHandler(io.StringIO())
+    handler.setFormatter(_ClickFormatter())
+    _log.addHandler(handler)
+
     try:
-        metadata = number_files(
-            dirpath=dirpath,
-            suffixes=suffixes,
-            progressbar=click.progressbar,
-            include_imeta=kwargs["include_imeta"],
-        )
-    except FnumException as e:
-        click.echo(str(e))
+        try:
+            metadata = number_files(
+                dirpath=dirpath,
+                suffixes=suffixes,
+                include_imeta=kwargs["include_imeta"],
+            )
+        finally:
+            _log.removeHandler(handler)
+    except (FnumException, FileNotFoundError) as e:
+        click.echo(str(e), err=True)
         sys.exit(1)
 
     if kwargs["write_max"]:
         metadata.get_max().to_file(dirpath)
     if kwargs["write_metadata"]:
         metadata.to_file(dirpath)
```

## Comparing `fnum-1.3.0.dist-info/LICENSE` & `fnum-1.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fnum-1.3.0.dist-info/METADATA` & `fnum-1.4.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnum
-Version: 1.3.0
+Version: 1.4.0
 Summary: Renames files in a directory using sequential integers
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/fnum
 Keywords: fnum,cli,utility,file,rename,sequential,order
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

## Comparing `fnum-1.3.0.dist-info/RECORD` & `fnum-1.4.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-fnum/__init__.py,sha256=lULYFuEY1FfVjBJwAweKKUmNWzgPy0HgKabhFMtJH3Q,4398
+fnum/__init__.py,sha256=VXqIdkLAA8XzWuJ2LcAh_Y3dHt57K_Q-IiTzktBTPTc,4271
 fnum/__main__.py,sha256=VNXCcgJ6hm4LbZBeOMBPCzuFTICAcX2m_2ThvsGiB2M,29
-fnum/cli.py,sha256=IRajKptRGnBqqrs7wLh-raNSaJ5-8hF-hHKEWHJLaFk,2116
+fnum/cli.py,sha256=tdTmqDEqe68lSugOl6h86l1FPqHssxdrnRZvI650-cU,2511
 fnum/exceptions.py,sha256=LYhcKutJUeBI2IYzIfH22L6tvt5rMz3zJSEjvoEkyAE,41
 fnum/metadata.py,sha256=3mswzDJGOMIRi4iNWhoqMmSK6GIGndD-MggKhJ9dyd8,2116
-fnum-1.3.0.dist-info/LICENSE,sha256=s1m2uS8ATMP1tmDdlqhtecX2AYDTccvP16kT1JtW7kM,1069
-fnum-1.3.0.dist-info/METADATA,sha256=Zpwhlc8e5IGt33icUx-c9EmuO5rODtyGO9UTP_Nlcyg,1038
-fnum-1.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fnum-1.3.0.dist-info/entry_points.txt,sha256=dPzJb98QpJdUrE4WPwvxwjoVBhPzI6KmnQdouKkPWyY,38
-fnum-1.3.0.dist-info/top_level.txt,sha256=jlmSGzNC8ba9j-R7Daca1UHvfQnC6GLcwDO97-SQLE4,5
-fnum-1.3.0.dist-info/RECORD,,
+fnum-1.4.0.dist-info/LICENSE,sha256=s1m2uS8ATMP1tmDdlqhtecX2AYDTccvP16kT1JtW7kM,1069
+fnum-1.4.0.dist-info/METADATA,sha256=EHpxRnkt32O3MK4b_ol6DVGBU573SoCyTDWJqwovwyM,1038
+fnum-1.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fnum-1.4.0.dist-info/entry_points.txt,sha256=dPzJb98QpJdUrE4WPwvxwjoVBhPzI6KmnQdouKkPWyY,38
+fnum-1.4.0.dist-info/top_level.txt,sha256=jlmSGzNC8ba9j-R7Daca1UHvfQnC6GLcwDO97-SQLE4,5
+fnum-1.4.0.dist-info/RECORD,,
```

