# Comparing `tmp/idownload-1.0.0-py3-none-any.whl.zip` & `tmp/idownload-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5568 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-09 06:22 idownload/__init__.py
--rw-r--r--  2.0 unx       29 b- defN 23-Jul-09 06:22 idownload/__main__.py
--rw-r--r--  2.0 unx     1018 b- defN 23-Jul-09 06:22 idownload/cli.py
--rw-r--r--  2.0 unx      241 b- defN 23-Jul-09 06:22 idownload/exceptions.py
--rw-r--r--  2.0 unx       69 b- defN 23-Jul-09 06:22 idownload/sources/__init__.py
--rw-r--r--  2.0 unx     3742 b- defN 23-Jul-09 06:22 idownload/sources/pinterest.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-09 06:23 idownload-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1351 b- defN 23-Jul-09 06:23 idownload-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 06:23 idownload-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Jul-09 06:23 idownload-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-09 06:23 idownload-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      968 b- defN 23-Jul-09 06:23 idownload-1.0.0.dist-info/RECORD
-12 files, 8659 bytes uncompressed, 3932 bytes compressed:  54.6%
+Zip file size: 5586 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-09 07:01 idownload/__init__.py
+-rw-r--r--  2.0 unx       29 b- defN 23-Jul-09 07:01 idownload/__main__.py
+-rw-r--r--  2.0 unx     1018 b- defN 23-Jul-09 07:01 idownload/cli.py
+-rw-r--r--  2.0 unx      241 b- defN 23-Jul-09 07:01 idownload/exceptions.py
+-rw-r--r--  2.0 unx       69 b- defN 23-Jul-09 07:01 idownload/sources/__init__.py
+-rw-r--r--  2.0 unx     3905 b- defN 23-Jul-09 07:01 idownload/sources/pinterest.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-09 07:01 idownload-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1351 b- defN 23-Jul-09 07:01 idownload-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 07:01 idownload-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Jul-09 07:01 idownload-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-09 07:01 idownload-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      968 b- defN 23-Jul-09 07:01 idownload-1.0.1.dist-info/RECORD
+12 files, 8822 bytes uncompressed, 3950 bytes compressed:  55.2%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: idownload/sources/__init__.py
 Comment: 
 
 Filename: idownload/sources/pinterest.py
 Comment: 
 
-Filename: idownload-1.0.0.dist-info/LICENSE
+Filename: idownload-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: idownload-1.0.0.dist-info/METADATA
+Filename: idownload-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: idownload-1.0.0.dist-info/WHEEL
+Filename: idownload-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: idownload-1.0.0.dist-info/entry_points.txt
+Filename: idownload-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: idownload-1.0.0.dist-info/top_level.txt
+Filename: idownload-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: idownload-1.0.0.dist-info/RECORD
+Filename: idownload-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## idownload/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.0"
+__version__ = "1.0.1"
```

## idownload/sources/pinterest.py

```diff
@@ -17,14 +17,19 @@
 stdout = io.StringIO()
 stderr = io.StringIO()
 try:
     with redirect_stdout(stdout), redirect_stderr(stderr):
         import nameattr
 except ImportError:
     pass
+except:
+    nameattr_out = stdout.getvalue()
+    nameattr_err = stderr.getvalue()
+    print(nameattr_err, end="")
+    print(nameattr_err, file=sys.stderr, end="")
 nameattr_out = stdout.getvalue()
 nameattr_err = stderr.getvalue()
 
 
 class PinterestSource:
     COMMAND = "pinterest"
     ARGS = ("username", "board", "dirpath")
```

## Comparing `idownload-1.0.0.dist-info/LICENSE` & `idownload-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `idownload-1.0.0.dist-info/METADATA` & `idownload-1.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idownload
-Version: 1.0.0
+Version: 1.0.1
 Summary: Downloads images and stores metadata about them in a JSON file
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/idownload
 Keywords: idownload,cli,utility,image,download,backup,archive,pinterest
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

## Comparing `idownload-1.0.0.dist-info/RECORD` & `idownload-1.0.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-idownload/__init__.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
+idownload/__init__.py,sha256=d4QHYmS_30j0hPN8NmNPnQ_Z0TphDRbu4MtQj9cT9e8,22
 idownload/__main__.py,sha256=VNXCcgJ6hm4LbZBeOMBPCzuFTICAcX2m_2ThvsGiB2M,29
 idownload/cli.py,sha256=4-baQmuaZhKB2xICp9YOvfedyzbz9xKMLam0ejdzTmo,1018
 idownload/exceptions.py,sha256=HCMziNWDLs85kKmyAd8KRKqLNttBtw38SMBrFzYzxCw,241
 idownload/sources/__init__.py,sha256=ueX9ofgR0hNk6kP1hOazFZc4V6alNJlzO2iSAwGmfNw,69
-idownload/sources/pinterest.py,sha256=8d-D5E1IKdRqcwYuANkA8RgbXjBdA7mPiTsSeh7Vq-0,3742
-idownload-1.0.0.dist-info/LICENSE,sha256=s1m2uS8ATMP1tmDdlqhtecX2AYDTccvP16kT1JtW7kM,1069
-idownload-1.0.0.dist-info/METADATA,sha256=nshOLi8zMRjo3tvNEM9K7SvAeD_g9_TaBFMtOyqRyOg,1351
-idownload-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-idownload-1.0.0.dist-info/entry_points.txt,sha256=KDq6QIybIzNOcikhtmF1AGljdRtpft5G1MmZOQwBAXk,48
-idownload-1.0.0.dist-info/top_level.txt,sha256=naaqaO3WgkP36-DF4qyxiZEZZyeNrtlrG68XGO_kOAw,10
-idownload-1.0.0.dist-info/RECORD,,
+idownload/sources/pinterest.py,sha256=dkSlPTS_soZ8vcPnRyK_NKkKCiQOjwXM6BJNq33qTZI,3905
+idownload-1.0.1.dist-info/LICENSE,sha256=s1m2uS8ATMP1tmDdlqhtecX2AYDTccvP16kT1JtW7kM,1069
+idownload-1.0.1.dist-info/METADATA,sha256=XoKHzhYTNeJvuE702daSPXA7d5MDLUJ6olBIf9adwAw,1351
+idownload-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+idownload-1.0.1.dist-info/entry_points.txt,sha256=KDq6QIybIzNOcikhtmF1AGljdRtpft5G1MmZOQwBAXk,48
+idownload-1.0.1.dist-info/top_level.txt,sha256=naaqaO3WgkP36-DF4qyxiZEZZyeNrtlrG68XGO_kOAw,10
+idownload-1.0.1.dist-info/RECORD,,
```

