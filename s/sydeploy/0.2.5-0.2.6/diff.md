# Comparing `tmp/sydeploy-0.2.5-py3-none-any.whl.zip` & `tmp/sydeploy-0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 7256 bytes, number of entries: 18
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 18:56 sydeploy/__init__.py
--rw-r--r--  2.0 unx      149 b- defN 23-Jul-09 18:56 sydeploy/errors.py
--rw-r--r--  2.0 unx      132 b- defN 23-Jul-09 18:56 sydeploy/run.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 18:56 sydeploy/commands/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 18:56 sydeploy/commands/authenticate/__init__.py
--rw-r--r--  2.0 unx     2012 b- defN 23-Jul-09 18:56 sydeploy/commands/authenticate/codeartifact.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 18:56 sydeploy/commands/build/__init__.py
--rw-r--r--  2.0 unx     4370 b- defN 23-Jul-09 18:56 sydeploy/commands/build/python-package.py
--rw-r--r--  2.0 unx      388 b- defN 23-Jul-09 18:56 sydeploy/templates/meta.yaml.dist
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-09 18:56 sydeploy/templates/setup.py.dist
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 18:56 sydeploy/utils/__init__.py
--rw-r--r--  2.0 unx      807 b- defN 23-Jul-09 18:56 sydeploy/utils/simple.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jul-09 18:56 sydeploy-0.2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      316 b- defN 23-Jul-09 18:56 sydeploy-0.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 18:56 sydeploy-0.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-09 18:56 sydeploy-0.2.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 18:56 sydeploy-0.2.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1510 b- defN 23-Jul-09 18:56 sydeploy-0.2.5.dist-info/RECORD
-18 files, 11187 bytes uncompressed, 4734 bytes compressed:  57.7%
+Zip file size: 7260 bytes, number of entries: 18
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 20:27 sydeploy/__init__.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-09 20:27 sydeploy/errors.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Jul-09 20:27 sydeploy/run.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 20:27 sydeploy/commands/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 20:27 sydeploy/commands/authenticate/__init__.py
+-rw-r--r--  2.0 unx     2013 b- defN 23-Jul-09 20:27 sydeploy/commands/authenticate/codeartifact.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 20:27 sydeploy/commands/build/__init__.py
+-rw-r--r--  2.0 unx     4370 b- defN 23-Jul-09 20:27 sydeploy/commands/build/python-package.py
+-rw-r--r--  2.0 unx      388 b- defN 23-Jul-09 20:27 sydeploy/templates/meta.yaml.dist
+-rw-r--r--  2.0 unx      287 b- defN 23-Jul-09 20:27 sydeploy/templates/setup.py.dist
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 20:27 sydeploy/utils/__init__.py
+-rw-r--r--  2.0 unx      807 b- defN 23-Jul-09 20:27 sydeploy/utils/simple.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jul-09 20:27 sydeploy-0.2.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      316 b- defN 23-Jul-09 20:27 sydeploy-0.2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 20:27 sydeploy-0.2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-09 20:27 sydeploy-0.2.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 20:27 sydeploy-0.2.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1510 b- defN 23-Jul-09 20:27 sydeploy-0.2.6.dist-info/RECORD
+18 files, 11188 bytes uncompressed, 4738 bytes compressed:  57.7%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: sydeploy/utils/__init__.py
 Comment: 
 
 Filename: sydeploy/utils/simple.py
 Comment: 
 
-Filename: sydeploy-0.2.5.dist-info/LICENSE
+Filename: sydeploy-0.2.6.dist-info/LICENSE
 Comment: 
 
-Filename: sydeploy-0.2.5.dist-info/METADATA
+Filename: sydeploy-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: sydeploy-0.2.5.dist-info/WHEEL
+Filename: sydeploy-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: sydeploy-0.2.5.dist-info/entry_points.txt
+Filename: sydeploy-0.2.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: sydeploy-0.2.5.dist-info/top_level.txt
+Filename: sydeploy-0.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: sydeploy-0.2.5.dist-info/RECORD
+Filename: sydeploy-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sydeploy/commands/authenticate/codeartifact.py

```diff
@@ -8,15 +8,15 @@
     pip = "pip" + str(sys.version_info[0])
     return run(args=f"{pip} config get global.index-url", shell=True, capture_output=True).stdout.decode("utf-8").strip()
 
 
 def set_index_url(body, extra: bool = False):
     pip = "pip" + str(sys.version_info[0])
     index_url = "extra-index-url" if extra else "index-url"
-    check_call([pip, "config", "set", f"global.{index_url}", body])
+    check_call([pip, "config", "set", f"globals.{index_url}", body])
 
 
 @impose
 def pip(domain: str = None, repo: str = None, region: str = None):
     if domain is None or repo is None:
         raise Exception("A domain and a repo must be defined for CodeArtifact.")
     region = "" if region is None else f"--region {region}"
```

## Comparing `sydeploy-0.2.5.dist-info/LICENSE` & `sydeploy-0.2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sydeploy-0.2.5.dist-info/RECORD` & `sydeploy-0.2.6.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 sydeploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/errors.py,sha256=BU5F1x81--SV7aVxynoUEHlu6b9LDFiQf2GnNazcs9c,149
 sydeploy/run.py,sha256=xBsWk4Qstmslp8XZGyEiZSd8_gMfPR8lCaX7BQ-hbWg,132
 sydeploy/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sydeploy/commands/authenticate/codeartifact.py,sha256=Dnon0tJf5_YsbuLbRCdInPqcgmIb6GkGa40UOdqNq_0,2012
+sydeploy/commands/authenticate/codeartifact.py,sha256=CGZan0-fcP-sxlzi12Q6jRT4inN31t6AObZVW7-Felk,2013
 sydeploy/commands/build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/build/python-package.py,sha256=6ti1iLGToUVivx_b0x7SIuilpwU0fPBS4aFH_NKXDWU,4370
 sydeploy/templates/meta.yaml.dist,sha256=XkJkfyrFwtMQqhrZaRNiCx_1TCbSMT1gz7TX0ngQcmc,388
 sydeploy/templates/setup.py.dist,sha256=kN0BaVS5hPiiASND6SXelU40c5JdDnJ8z2XXRJDxsE0,287
 sydeploy/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/utils/simple.py,sha256=fabtM0DAnb9iF28FPIBzAax7isR-aEfTzcWPWyLqBjM,807
-sydeploy-0.2.5.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
-sydeploy-0.2.5.dist-info/METADATA,sha256=R2W4FSs1PYsJIEBtjBQJTIG9Jh_2IdyGSYa_GAv5F8s,316
-sydeploy-0.2.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sydeploy-0.2.5.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
-sydeploy-0.2.5.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
-sydeploy-0.2.5.dist-info/RECORD,,
+sydeploy-0.2.6.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
+sydeploy-0.2.6.dist-info/METADATA,sha256=NtWlUttkLcQlmiOwtLVWG-9uSPPC120AdDDz84jEyDA,316
+sydeploy-0.2.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sydeploy-0.2.6.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
+sydeploy-0.2.6.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
+sydeploy-0.2.6.dist-info/RECORD,,
```

