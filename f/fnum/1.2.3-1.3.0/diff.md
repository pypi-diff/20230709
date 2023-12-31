# Comparing `tmp/fnum-1.2.3-py3-none-any.whl.zip` & `tmp/fnum-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5781 bytes, number of entries: 11
--rw-r--r--  2.0 unx     4363 b- defN 23-Jul-09 08:34 fnum/__init__.py
--rw-r--r--  2.0 unx       29 b- defN 23-Jul-09 08:34 fnum/__main__.py
--rw-r--r--  2.0 unx     1969 b- defN 23-Jul-09 08:34 fnum/cli.py
--rw-r--r--  2.0 unx       41 b- defN 23-Jul-09 08:34 fnum/exceptions.py
--rw-r--r--  2.0 unx     2116 b- defN 23-Jul-09 08:34 fnum/metadata.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-09 08:35 fnum-1.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1038 b- defN 23-Jul-09 08:35 fnum-1.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 08:35 fnum-1.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-09 08:35 fnum-1.2.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-09 08:35 fnum-1.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      820 b- defN 23-Jul-09 08:35 fnum-1.2.3.dist-info/RECORD
-11 files, 11580 bytes uncompressed, 4407 bytes compressed:  61.9%
+Zip file size: 5857 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     4398 b- defN 23-Jul-09 09:20 fnum/__init__.py
+-rw-r--r--  2.0 unx       29 b- defN 23-Jul-09 09:20 fnum/__main__.py
+-rw-r--r--  2.0 unx     2116 b- defN 23-Jul-09 09:20 fnum/cli.py
+-rw-r--r--  2.0 unx       41 b- defN 23-Jul-09 09:20 fnum/exceptions.py
+-rw-r--r--  2.0 unx     2116 b- defN 23-Jul-09 09:20 fnum/metadata.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-09 09:20 fnum-1.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1038 b- defN 23-Jul-09 09:20 fnum-1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 09:20 fnum-1.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-09 09:20 fnum-1.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-09 09:20 fnum-1.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jul-09 09:20 fnum-1.3.0.dist-info/RECORD
+11 files, 11762 bytes uncompressed, 4483 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: fnum/exceptions.py
 Comment: 
 
 Filename: fnum/metadata.py
 Comment: 
 
-Filename: fnum-1.2.3.dist-info/LICENSE
+Filename: fnum-1.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: fnum-1.2.3.dist-info/METADATA
+Filename: fnum-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: fnum-1.2.3.dist-info/WHEEL
+Filename: fnum-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: fnum-1.2.3.dist-info/entry_points.txt
+Filename: fnum-1.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: fnum-1.2.3.dist-info/top_level.txt
+Filename: fnum-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fnum-1.2.3.dist-info/RECORD
+Filename: fnum-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fnum/__init__.py

```diff
@@ -2,15 +2,15 @@
 from contextlib import contextmanager
 from imeta import ImageMetadata
 
 from .exceptions import FnumException
 from .metadata import FnumMetadata, FnumMax
 
 
-__version__ = "1.2.3"
+__version__ = "1.3.0"
 
 
 def number_files(dirpath, suffixes, progressbar=None, include_imeta=False):
     dirpath = Path(dirpath)
 
     try:
         metadata = FnumMetadata.from_file(dirpath)
@@ -115,15 +115,17 @@
     if not progressbar:
 
         @contextmanager
         def noop_progressbar(*args, **kwargs):
             yield args[0]
 
         progressbar = noop_progressbar
-    with progressbar(files, length=len(files), label="Processing files") as bar:
+    with progressbar(
+        files, length=len(files), label="Processing files", update_min_steps=10
+    ) as bar:
         for filepath in bar:
             if not filepath.is_file() or filepath.suffix not in suffixes:
                 continue
 
             try:
                 if int(filepath.stem) <= num:
                     continue
```

## fnum/cli.py

```diff
@@ -41,15 +41,19 @@
     default=False,
     help="""
 Also rename image metadata files generated by imeta.
     """,
 )
 def cli(**kwargs):
     dirpath = kwargs["dirpath"]
+    if "/" in kwargs["suffixes"]:
+        click.echo("Suffixes contains a '/', did you mean ','?", err=True)
     suffixes = kwargs["suffixes"].split(",")
+
+    click.echo("Analyzing files...")
     try:
         metadata = number_files(
             dirpath=dirpath,
             suffixes=suffixes,
             progressbar=click.progressbar,
             include_imeta=kwargs["include_imeta"],
         )
```

## Comparing `fnum-1.2.3.dist-info/LICENSE` & `fnum-1.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fnum-1.2.3.dist-info/METADATA` & `fnum-1.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnum
-Version: 1.2.3
+Version: 1.3.0
 Summary: Renames files in a directory using sequential integers
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/fnum
 Keywords: fnum,cli,utility,file,rename,sequential,order
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

