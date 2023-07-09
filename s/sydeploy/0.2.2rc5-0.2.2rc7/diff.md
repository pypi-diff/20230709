# Comparing `tmp/sydeploy-0.2.2rc5-py3-none-any.whl.zip` & `tmp/sydeploy-0.2.2rc7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,20 @@
-Zip file size: 5995 bytes, number of entries: 14
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 17:27 sydeploy/__init__.py
--rw-r--r--  2.0 unx      149 b- defN 23-Jul-09 17:27 sydeploy/errors.py
--rw-r--r--  2.0 unx      132 b- defN 23-Jul-09 17:27 sydeploy/run.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 17:27 sydeploy/commands/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 17:27 sydeploy/commands/authenticate/__init__.py
--rw-r--r--  2.0 unx     2018 b- defN 23-Jul-09 17:27 sydeploy/commands/authenticate/codeartifact.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 17:27 sydeploy/commands/build/__init__.py
--rw-r--r--  2.0 unx     4370 b- defN 23-Jul-09 17:27 sydeploy/commands/build/python-package.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jul-09 17:27 sydeploy-0.2.2rc5.dist-info/LICENSE
--rw-r--r--  2.0 unx      297 b- defN 23-Jul-09 17:27 sydeploy-0.2.2rc5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 17:27 sydeploy-0.2.2rc5.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-09 17:27 sydeploy-0.2.2rc5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 17:27 sydeploy-0.2.2rc5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1191 b- defN 23-Jul-09 17:27 sydeploy-0.2.2rc5.dist-info/RECORD
-14 files, 9373 bytes uncompressed, 3971 bytes compressed:  57.6%
+Zip file size: 7298 bytes, number of entries: 18
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 17:37 sydeploy/__init__.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-09 17:37 sydeploy/errors.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Jul-09 17:37 sydeploy/run.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 17:37 sydeploy/commands/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 17:37 sydeploy/commands/authenticate/__init__.py
+-rw-r--r--  2.0 unx     2018 b- defN 23-Jul-09 17:37 sydeploy/commands/authenticate/codeartifact.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 17:37 sydeploy/commands/build/__init__.py
+-rw-r--r--  2.0 unx     4370 b- defN 23-Jul-09 17:37 sydeploy/commands/build/python-package.py
+-rw-r--r--  2.0 unx      388 b- defN 23-Jul-09 17:37 sydeploy/templates/meta.yaml.dist
+-rw-r--r--  2.0 unx      287 b- defN 23-Jul-09 17:37 sydeploy/templates/setup.py.dist
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 17:37 sydeploy/utils/__init__.py
+-rw-r--r--  2.0 unx      807 b- defN 23-Jul-09 17:37 sydeploy/utils/simple.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jul-09 17:38 sydeploy-0.2.2rc7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      297 b- defN 23-Jul-09 17:38 sydeploy-0.2.2rc7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 17:38 sydeploy-0.2.2rc7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-09 17:38 sydeploy-0.2.2rc7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 17:38 sydeploy-0.2.2rc7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1528 b- defN 23-Jul-09 17:38 sydeploy-0.2.2rc7.dist-info/RECORD
+18 files, 11192 bytes uncompressed, 4740 bytes compressed:  57.6%
```

## zipnote {}

```diff
@@ -18,26 +18,38 @@
 
 Filename: sydeploy/commands/build/__init__.py
 Comment: 
 
 Filename: sydeploy/commands/build/python-package.py
 Comment: 
 
-Filename: sydeploy-0.2.2rc5.dist-info/LICENSE
+Filename: sydeploy/templates/meta.yaml.dist
 Comment: 
 
-Filename: sydeploy-0.2.2rc5.dist-info/METADATA
+Filename: sydeploy/templates/setup.py.dist
 Comment: 
 
-Filename: sydeploy-0.2.2rc5.dist-info/WHEEL
+Filename: sydeploy/utils/__init__.py
 Comment: 
 
-Filename: sydeploy-0.2.2rc5.dist-info/entry_points.txt
+Filename: sydeploy/utils/simple.py
 Comment: 
 
-Filename: sydeploy-0.2.2rc5.dist-info/top_level.txt
+Filename: sydeploy-0.2.2rc7.dist-info/LICENSE
 Comment: 
 
-Filename: sydeploy-0.2.2rc5.dist-info/RECORD
+Filename: sydeploy-0.2.2rc7.dist-info/METADATA
+Comment: 
+
+Filename: sydeploy-0.2.2rc7.dist-info/WHEEL
+Comment: 
+
+Filename: sydeploy-0.2.2rc7.dist-info/entry_points.txt
+Comment: 
+
+Filename: sydeploy-0.2.2rc7.dist-info/top_level.txt
+Comment: 
+
+Filename: sydeploy-0.2.2rc7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sydeploy-0.2.2rc5.dist-info/LICENSE` & `sydeploy-0.2.2rc7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sydeploy-0.2.2rc5.dist-info/RECORD` & `sydeploy-0.2.2rc7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -2,13 +2,17 @@
 sydeploy/errors.py,sha256=BU5F1x81--SV7aVxynoUEHlu6b9LDFiQf2GnNazcs9c,149
 sydeploy/run.py,sha256=xBsWk4Qstmslp8XZGyEiZSd8_gMfPR8lCaX7BQ-hbWg,132
 sydeploy/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/codeartifact.py,sha256=cJ70VKV3DUe6jzNW5tcS7zYdk6h0r6sdinAusIF2q4M,2018
 sydeploy/commands/build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/build/python-package.py,sha256=6ti1iLGToUVivx_b0x7SIuilpwU0fPBS4aFH_NKXDWU,4370
-sydeploy-0.2.2rc5.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
-sydeploy-0.2.2rc5.dist-info/METADATA,sha256=A4K_QDV_CHpCJzc3lfAl1JgMAOHzjImphmt9AL3ZCg0,297
-sydeploy-0.2.2rc5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sydeploy-0.2.2rc5.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
-sydeploy-0.2.2rc5.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
-sydeploy-0.2.2rc5.dist-info/RECORD,,
+sydeploy/templates/meta.yaml.dist,sha256=XkJkfyrFwtMQqhrZaRNiCx_1TCbSMT1gz7TX0ngQcmc,388
+sydeploy/templates/setup.py.dist,sha256=kN0BaVS5hPiiASND6SXelU40c5JdDnJ8z2XXRJDxsE0,287
+sydeploy/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+sydeploy/utils/simple.py,sha256=fabtM0DAnb9iF28FPIBzAax7isR-aEfTzcWPWyLqBjM,807
+sydeploy-0.2.2rc7.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
+sydeploy-0.2.2rc7.dist-info/METADATA,sha256=Q4D8bXvaUCu6WM9R1l-v17UTYVA3BRpQR4PiIdysx3Q,297
+sydeploy-0.2.2rc7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sydeploy-0.2.2rc7.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
+sydeploy-0.2.2rc7.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
+sydeploy-0.2.2rc7.dist-info/RECORD,,
```

