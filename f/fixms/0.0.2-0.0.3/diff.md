# Comparing `tmp/fixms-0.0.2.tar.gz` & `tmp/fixms-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixms-0.0.2.tar", max compression
+gzip compressed data, was "fixms-0.0.3.tar", max compression
```

## Comparing `fixms-0.0.2.tar` & `fixms-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-07-07 08:10:30.113801 fixms-0.0.2/LICENSE
--rw-r--r--   0        0        0     3097 2023-07-07 08:10:30.113801 fixms-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-07-07 08:10:30.113801 fixms-0.0.2/fixms/__init__.py
--rw-r--r--   0        0        0    12138 2023-07-07 08:10:30.113801 fixms-0.0.2/fixms/fix_ms_corrs.py
--rw-r--r--   0        0        0    12457 2023-07-07 08:10:30.113801 fixms-0.0.2/fixms/fix_ms_dir.py
--rw-r--r--   0        0        0      729 2023-07-07 08:10:30.113801 fixms-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3742 1970-01-01 00:00:00.000000 fixms-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-09 12:05:08.417412 fixms-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3097 2023-07-09 12:05:08.417412 fixms-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 12:05:08.417412 fixms-0.0.3/fixms/__init__.py
+-rw-r--r--   0        0        0    12266 2023-07-09 12:05:08.417412 fixms-0.0.3/fixms/fix_ms_corrs.py
+-rw-r--r--   0        0        0    12469 2023-07-09 12:05:08.417412 fixms-0.0.3/fixms/fix_ms_dir.py
+-rw-r--r--   0        0        0      729 2023-07-09 12:05:08.417412 fixms-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3742 1970-01-01 00:00:00.000000 fixms-0.0.3/PKG-INFO
```

### Comparing `fixms-0.0.2/LICENSE` & `fixms-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fixms-0.0.2/README.md` & `fixms-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fixms-0.0.2/fixms/fix_ms_corrs.py` & `fixms-0.0.3/fixms/fix_ms_corrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
     Returns:
         int: Number of chunks in a measurement set
     """
     with table(ms.as_posix(), readonly=True, ack=False) as tab:
         return int(np.ceil(len(tab.__getattr__(data_column)) / chunksize))
 
 
-def main(
+def fix_ms_corrs(
     ms: Path,
     chunksize: int = 10_000,
     data_column: str = "DATA",
     corrected_data_column: str = "CORRECTED_DATA",
 ) -> None:
     """Apply corrections to the ASKAP visibilities to bring them inline with
     what is expectede from other imagers, including CASA and WSClean. The
@@ -277,15 +277,15 @@
 def cli():
     import argparse
 
     parser = argparse.ArgumentParser(
         description=__doc__,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument("ms", type=str, help="The MS to fix")
+    parser.add_argument("ms", type=Path, help="The MS to fix")
     parser.add_argument(
         "--chunksize",
         type=int,
         default=1000,
         help="The chunksize to use when reading the MS",
     )
     parser.add_argument(
@@ -294,12 +294,17 @@
     parser.add_argument(
         "--corrected-data-column",
         type=str,
         default="CORRECTED_DATA",
         help="The column to write the corrected data to",
     )
     args = parser.parse_args()
-    main(Path(args.ms), args.chunksize, args.data_column)
+    fix_ms_corrs(
+        Path(args.ms),
+        chunksize=args.chunksize,
+        data_column=args.data_column,
+        corrected_data_column=args.corrected_data_column,
+    )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `fixms-0.0.2/fixms/fix_ms_dir.py` & `fixms-0.0.3/fixms/fix_ms_dir.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     ss = float(c)
     r = (ss + 60.0 * (mm + 60.0 * dd)) * 2.0 * math.pi / 1296000.0
     if dec_string[0] == "-":
         r = -r
     return r
 
 
-def main(ms):
+def fix_ms_dir(ms):
     # Check that the observation wasn't in pol_fixed mode
     with table("%s/ANTENNA" % (ms), readonly=True, ack=False) as ta:
         ant_mount = ta.getcol("MOUNT", 0, 1)
         if ant_mount[0] != "equatorial":
             sys.exit(f"{ms} doesn't support pol_fixed mode")
 
     # Work out which beam is in this MS
@@ -362,12 +362,12 @@
     parser.add_argument(
         "ms", help="Measurement set to update", type=str, default=None, nargs="?"
     )
     # Parse the command line
     args = parser.parse_args()
 
     # Call the main function
-    main(args.ms)
+    fix_ms_dir(args.ms)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `fixms-0.0.2/pyproject.toml` & `fixms-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fixms"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Alec Thomson (S&A, Kensington WA) <alec.thomson@csiro.au>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `fixms-0.0.2/PKG-INFO` & `fixms-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixms
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 License: MIT
 Author: Alec Thomson (S&A, Kensington WA)
 Author-email: alec.thomson@csiro.au
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

