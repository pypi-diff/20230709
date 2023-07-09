# Comparing `tmp/fbn-0.1.0-py3-none-any.whl.zip` & `tmp/fbn-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 8559 bytes, number of entries: 12
--rw-r--r--  2.0 unx       81 b- defN 23-Jul-09 20:47 fbn/__init__.py
--rw-r--r--  2.0 unx       61 b- defN 23-Jul-09 20:47 fbn/__main__.py
--rw-r--r--  2.0 unx     2686 b- defN 23-Jul-09 20:47 fbn/cli.py
--rw-r--r--  2.0 unx       78 b- defN 23-Jul-09 20:47 fbn/constants.py
--rw-r--r--  2.0 unx      406 b- defN 23-Jul-09 20:47 fbn/exceptions.py
--rw-r--r--  2.0 unx     7376 b- defN 23-Jul-09 20:47 fbn/fb.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Jul-09 20:47 fbn-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5020 b- defN 23-Jul-09 20:47 fbn-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 20:47 fbn-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       42 b- defN 23-Jul-09 20:47 fbn-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Jul-09 20:47 fbn-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      873 b- defN 23-Jul-09 20:47 fbn-0.1.0.dist-info/RECORD
-12 files, 17784 bytes uncompressed, 7111 bytes compressed:  60.0%
+Zip file size: 8554 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       81 b- defN 23-Jul-09 20:55 fbn/__init__.py
+-rw-r--r--  2.0 unx       61 b- defN 23-Jul-09 20:55 fbn/__main__.py
+-rw-r--r--  2.0 unx     2686 b- defN 23-Jul-09 20:55 fbn/cli.py
+-rw-r--r--  2.0 unx       78 b- defN 23-Jul-09 20:55 fbn/constants.py
+-rw-r--r--  2.0 unx      406 b- defN 23-Jul-09 20:55 fbn/exceptions.py
+-rw-r--r--  2.0 unx     7374 b- defN 23-Jul-09 20:55 fbn/fb.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jul-09 20:55 fbn-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5020 b- defN 23-Jul-09 20:55 fbn-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 20:55 fbn-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 23-Jul-09 20:55 fbn-0.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-09 20:55 fbn-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      873 b- defN 23-Jul-09 20:55 fbn-0.1.1.dist-info/RECORD
+12 files, 17782 bytes uncompressed, 7106 bytes compressed:  60.0%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: fbn/exceptions.py
 Comment: 
 
 Filename: fbn/fb.py
 Comment: 
 
-Filename: fbn-0.1.0.dist-info/LICENSE
+Filename: fbn-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: fbn-0.1.0.dist-info/METADATA
+Filename: fbn-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: fbn-0.1.0.dist-info/WHEEL
+Filename: fbn-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: fbn-0.1.0.dist-info/entry_points.txt
+Filename: fbn-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: fbn-0.1.0.dist-info/top_level.txt
+Filename: fbn-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: fbn-0.1.0.dist-info/RECORD
+Filename: fbn-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbn/__init__.py

```diff
@@ -1,3 +1,3 @@
 __author__ = "Visesh Prasad"
 __email__ = "visesh@live.com"
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## fbn/fb.py

```diff
@@ -205,15 +205,15 @@
     check_fb(**kwargs)
     logger.debug("Creating schedule...")
     if frequency:
         interval, unit = parse_frequency(frequency)
         schedule_unit = SCHEDULE_UNIT_MAP[unit]
         getattr(schedule.every(int(interval)), schedule_unit).do(check_fb, **kwargs)
     else:  # randomize as the default
-        schedule.every(2).to(4).minutes.do(check_fb, **kwargs)
+        schedule.every(2).to(4).hours.do(check_fb, **kwargs)
     # run
     while True:
         logger.debug(f"Next check at {schedule.next_run()}...")
         n = schedule.idle_seconds()
         if n > 0:
             # sleep exactly the right amount of time
             time.sleep(n)
```

## Comparing `fbn-0.1.0.dist-info/LICENSE` & `fbn-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fbn-0.1.0.dist-info/METADATA` & `fbn-0.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbn
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tool to monitor fb groups and notify
 Home-page: https://github.com/viseshrp/fbn
 Author: Visesh Prasad
 Author-email: visesh@live.com
 Maintainer: Visesh Prasad
 Maintainer-email: visesh@live.com
 License: MIT license
```

## Comparing `fbn-0.1.0.dist-info/RECORD` & `fbn-0.1.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-fbn/__init__.py,sha256=a1_p7ryw-0GMPQwe9ReNGILPut4ExRIXvF3zHkwLjN4,81
+fbn/__init__.py,sha256=n_RcprRToTC1WU4QumeFXWop6H7YvKMc4uSUey_ou7Q,81
 fbn/__main__.py,sha256=MSmt_5Xg84uHqzTN38JwgseJK8rsJn_11A8WD99VtEo,61
 fbn/cli.py,sha256=Hg0l2gxOrO_TT_RjdjU4iQnjLcIuaXLKXM3qPYDZp3Y,2686
 fbn/constants.py,sha256=cMQzDOJVV3vm3P1UqY1DKpB5OfhLdT5fbLEM6tAu6l8,78
 fbn/exceptions.py,sha256=8yan1cmPUJEbiTW12adRoyWF48zb3L2SCKEW1trobyA,406
-fbn/fb.py,sha256=Dy5xg37m1iRsn7P4AP-BozEt6ZHlckWbusSESJZI-OQ,7376
-fbn-0.1.0.dist-info/LICENSE,sha256=25qEHPeTSJTu_3MheLT2jl_taHxPcxlaORhLfxGDbTU,1065
-fbn-0.1.0.dist-info/METADATA,sha256=tMR-b7BqOAETIvU2G2wrYUBAeX9d52q3xhddLOr9xIk,5020
-fbn-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fbn-0.1.0.dist-info/entry_points.txt,sha256=PjZFFzJbekNwM2i-9gSHHb6eQsIP6NRMgcoF98ysoZM,42
-fbn-0.1.0.dist-info/top_level.txt,sha256=Cekq2PfsBF7azxMgcSBWbU_elQ_WUTGuY37h4zY5Cu8,4
-fbn-0.1.0.dist-info/RECORD,,
+fbn/fb.py,sha256=A5F-TSLKuramGwsMAYLGOB-zgyzNeO_tvHnrq58kkWA,7374
+fbn-0.1.1.dist-info/LICENSE,sha256=25qEHPeTSJTu_3MheLT2jl_taHxPcxlaORhLfxGDbTU,1065
+fbn-0.1.1.dist-info/METADATA,sha256=TlRmL8O9sdFe5OIU3pNCgfuHQuZrELjUgPf-afCmiZA,5020
+fbn-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fbn-0.1.1.dist-info/entry_points.txt,sha256=PjZFFzJbekNwM2i-9gSHHb6eQsIP6NRMgcoF98ysoZM,42
+fbn-0.1.1.dist-info/top_level.txt,sha256=Cekq2PfsBF7azxMgcSBWbU_elQ_WUTGuY37h4zY5Cu8,4
+fbn-0.1.1.dist-info/RECORD,,
```

