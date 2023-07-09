# Comparing `tmp/sydeploy-0.2.2rc9-py3-none-any.whl.zip` & `tmp/sydeploy-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 7300 bytes, number of entries: 18
+Zip file size: 7258 bytes, number of entries: 18
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 17:49 sydeploy/__init__.py
 -rw-r--r--  2.0 unx      149 b- defN 23-Jul-09 17:49 sydeploy/errors.py
 -rw-r--r--  2.0 unx      132 b- defN 23-Jul-09 17:49 sydeploy/run.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 17:49 sydeploy/commands/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 17:49 sydeploy/commands/authenticate/__init__.py
 -rw-r--r--  2.0 unx     2018 b- defN 23-Jul-09 17:49 sydeploy/commands/authenticate/codeartifact.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 17:49 sydeploy/commands/build/__init__.py
 -rw-r--r--  2.0 unx     4370 b- defN 23-Jul-09 17:49 sydeploy/commands/build/python-package.py
 -rw-r--r--  2.0 unx      388 b- defN 23-Jul-09 17:49 sydeploy/templates/meta.yaml.dist
 -rw-r--r--  2.0 unx      287 b- defN 23-Jul-09 17:49 sydeploy/templates/setup.py.dist
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 17:49 sydeploy/utils/__init__.py
 -rw-r--r--  2.0 unx      807 b- defN 23-Jul-09 17:49 sydeploy/utils/simple.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jul-09 17:49 sydeploy-0.2.2rc9.dist-info/LICENSE
--rw-r--r--  2.0 unx      297 b- defN 23-Jul-09 17:49 sydeploy-0.2.2rc9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 17:49 sydeploy-0.2.2rc9.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-09 17:49 sydeploy-0.2.2rc9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 17:49 sydeploy-0.2.2rc9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1528 b- defN 23-Jul-09 17:49 sydeploy-0.2.2rc9.dist-info/RECORD
-18 files, 11192 bytes uncompressed, 4742 bytes compressed:  57.6%
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jul-09 17:50 sydeploy-0.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      294 b- defN 23-Jul-09 17:50 sydeploy-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 17:50 sydeploy-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-09 17:50 sydeploy-0.2.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 17:50 sydeploy-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1510 b- defN 23-Jul-09 17:50 sydeploy-0.2.3.dist-info/RECORD
+18 files, 11171 bytes uncompressed, 4736 bytes compressed:  57.6%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: sydeploy/utils/__init__.py
 Comment: 
 
 Filename: sydeploy/utils/simple.py
 Comment: 
 
-Filename: sydeploy-0.2.2rc9.dist-info/LICENSE
+Filename: sydeploy-0.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: sydeploy-0.2.2rc9.dist-info/METADATA
+Filename: sydeploy-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: sydeploy-0.2.2rc9.dist-info/WHEEL
+Filename: sydeploy-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: sydeploy-0.2.2rc9.dist-info/entry_points.txt
+Filename: sydeploy-0.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: sydeploy-0.2.2rc9.dist-info/top_level.txt
+Filename: sydeploy-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: sydeploy-0.2.2rc9.dist-info/RECORD
+Filename: sydeploy-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sydeploy-0.2.2rc9.dist-info/LICENSE` & `sydeploy-0.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sydeploy-0.2.2rc9.dist-info/RECORD` & `sydeploy-0.2.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 sydeploy/commands/authenticate/codeartifact.py,sha256=cJ70VKV3DUe6jzNW5tcS7zYdk6h0r6sdinAusIF2q4M,2018
 sydeploy/commands/build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/build/python-package.py,sha256=6ti1iLGToUVivx_b0x7SIuilpwU0fPBS4aFH_NKXDWU,4370
 sydeploy/templates/meta.yaml.dist,sha256=XkJkfyrFwtMQqhrZaRNiCx_1TCbSMT1gz7TX0ngQcmc,388
 sydeploy/templates/setup.py.dist,sha256=kN0BaVS5hPiiASND6SXelU40c5JdDnJ8z2XXRJDxsE0,287
 sydeploy/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/utils/simple.py,sha256=fabtM0DAnb9iF28FPIBzAax7isR-aEfTzcWPWyLqBjM,807
-sydeploy-0.2.2rc9.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
-sydeploy-0.2.2rc9.dist-info/METADATA,sha256=wxXKveIdCbsCXpTjoNPigVY0yPqF0q1j_TYO9qIGGAE,297
-sydeploy-0.2.2rc9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sydeploy-0.2.2rc9.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
-sydeploy-0.2.2rc9.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
-sydeploy-0.2.2rc9.dist-info/RECORD,,
+sydeploy-0.2.3.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
+sydeploy-0.2.3.dist-info/METADATA,sha256=r_em_ii20ZxQKy3Wh98JQLJCrtAa-WC1T-G-mhgQllQ,294
+sydeploy-0.2.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sydeploy-0.2.3.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
+sydeploy-0.2.3.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
+sydeploy-0.2.3.dist-info/RECORD,,
```

