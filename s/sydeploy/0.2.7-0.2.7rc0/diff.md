# Comparing `tmp/sydeploy-0.2.7-py3-none-any.whl.zip` & `tmp/sydeploy-0.2.7rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 7257 bytes, number of entries: 18
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 21:16 sydeploy/__init__.py
--rw-r--r--  2.0 unx      149 b- defN 23-Jul-09 21:16 sydeploy/errors.py
--rw-r--r--  2.0 unx      132 b- defN 23-Jul-09 21:16 sydeploy/run.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 21:16 sydeploy/commands/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 21:16 sydeploy/commands/authenticate/__init__.py
--rw-r--r--  2.0 unx     2008 b- defN 23-Jul-09 21:16 sydeploy/commands/authenticate/codeartifact.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 21:16 sydeploy/commands/build/__init__.py
--rw-r--r--  2.0 unx     4370 b- defN 23-Jul-09 21:16 sydeploy/commands/build/python-package.py
--rw-r--r--  2.0 unx      388 b- defN 23-Jul-09 21:16 sydeploy/templates/meta.yaml.dist
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-09 21:16 sydeploy/templates/setup.py.dist
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 21:16 sydeploy/utils/__init__.py
--rw-r--r--  2.0 unx      807 b- defN 23-Jul-09 21:16 sydeploy/utils/simple.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jul-09 21:16 sydeploy-0.2.7.dist-info/LICENSE
--rw-r--r--  2.0 unx      316 b- defN 23-Jul-09 21:16 sydeploy-0.2.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 21:16 sydeploy-0.2.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-09 21:16 sydeploy-0.2.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 21:16 sydeploy-0.2.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1510 b- defN 23-Jul-09 21:16 sydeploy-0.2.7.dist-info/RECORD
-18 files, 11183 bytes uncompressed, 4735 bytes compressed:  57.7%
+Zip file size: 7352 bytes, number of entries: 18
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 21:22 sydeploy/__init__.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-09 21:22 sydeploy/errors.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Jul-09 21:22 sydeploy/run.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 21:22 sydeploy/commands/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 21:22 sydeploy/commands/authenticate/__init__.py
+-rw-r--r--  2.0 unx     2156 b- defN 23-Jul-09 21:22 sydeploy/commands/authenticate/codeartifact.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 21:22 sydeploy/commands/build/__init__.py
+-rw-r--r--  2.0 unx     4370 b- defN 23-Jul-09 21:22 sydeploy/commands/build/python-package.py
+-rw-r--r--  2.0 unx      388 b- defN 23-Jul-09 21:22 sydeploy/templates/meta.yaml.dist
+-rw-r--r--  2.0 unx      287 b- defN 23-Jul-09 21:22 sydeploy/templates/setup.py.dist
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 21:22 sydeploy/utils/__init__.py
+-rw-r--r--  2.0 unx      807 b- defN 23-Jul-09 21:22 sydeploy/utils/simple.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jul-09 21:23 sydeploy-0.2.7rc0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      319 b- defN 23-Jul-09 21:23 sydeploy-0.2.7rc0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 21:23 sydeploy-0.2.7rc0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-09 21:23 sydeploy-0.2.7rc0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 21:23 sydeploy-0.2.7rc0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1528 b- defN 23-Jul-09 21:23 sydeploy-0.2.7rc0.dist-info/RECORD
+18 files, 11352 bytes uncompressed, 4794 bytes compressed:  57.8%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: sydeploy/utils/__init__.py
 Comment: 
 
 Filename: sydeploy/utils/simple.py
 Comment: 
 
-Filename: sydeploy-0.2.7.dist-info/LICENSE
+Filename: sydeploy-0.2.7rc0.dist-info/LICENSE
 Comment: 
 
-Filename: sydeploy-0.2.7.dist-info/METADATA
+Filename: sydeploy-0.2.7rc0.dist-info/METADATA
 Comment: 
 
-Filename: sydeploy-0.2.7.dist-info/WHEEL
+Filename: sydeploy-0.2.7rc0.dist-info/WHEEL
 Comment: 
 
-Filename: sydeploy-0.2.7.dist-info/entry_points.txt
+Filename: sydeploy-0.2.7rc0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sydeploy-0.2.7.dist-info/top_level.txt
+Filename: sydeploy-0.2.7rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: sydeploy-0.2.7.dist-info/RECORD
+Filename: sydeploy-0.2.7rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sydeploy/commands/authenticate/codeartifact.py

```diff
@@ -1,22 +1,26 @@
 import sys
 import os
-from subprocess import run, check_call
+from subprocess import run, Popen, PIPE
 from impose_cli.decorators import impose
 
 
 def get_index_url():
     pip = "pip" + str(sys.version_info[0])
     return run(args=f"{pip} config get global.index-url", shell=True, capture_output=True).stdout.decode("utf-8").strip()
 
 
 def set_index_url(body, extra: bool = False):
+    print(body)
     pip = "pip" + str(sys.version_info[0])
     index_url = "extra-index-url" if extra else "index-url"
-    os.system(f'{pip} config set globals.{index_url} "{body}"')
+    process = Popen([pip, "config", "set", f"globals.{index_url}", f'"{body}"'], stdout=PIPE, stderr=PIPE, text=True)
+    output, error = process.communicate()
+    print(output)
+    print(error)
 
 
 @impose
 def pip(domain: str = None, repo: str = None, region: str = None):
     if domain is None or repo is None:
         raise Exception("A domain and a repo must be defined for CodeArtifact.")
     region = "" if region is None else f"--region {region}"
```

## Comparing `sydeploy-0.2.7.dist-info/LICENSE` & `sydeploy-0.2.7rc0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sydeploy-0.2.7.dist-info/RECORD` & `sydeploy-0.2.7rc0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 sydeploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/errors.py,sha256=BU5F1x81--SV7aVxynoUEHlu6b9LDFiQf2GnNazcs9c,149
 sydeploy/run.py,sha256=xBsWk4Qstmslp8XZGyEiZSd8_gMfPR8lCaX7BQ-hbWg,132
 sydeploy/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sydeploy/commands/authenticate/codeartifact.py,sha256=ciH41hS00EuhMGCfe0gVKBSvNQDT9jov6sgjefzjlJ8,2008
+sydeploy/commands/authenticate/codeartifact.py,sha256=7reyUtOJN8NROBJQSJc89k5I3C_9OdzeDcWMztqz7WA,2156
 sydeploy/commands/build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/build/python-package.py,sha256=6ti1iLGToUVivx_b0x7SIuilpwU0fPBS4aFH_NKXDWU,4370
 sydeploy/templates/meta.yaml.dist,sha256=XkJkfyrFwtMQqhrZaRNiCx_1TCbSMT1gz7TX0ngQcmc,388
 sydeploy/templates/setup.py.dist,sha256=kN0BaVS5hPiiASND6SXelU40c5JdDnJ8z2XXRJDxsE0,287
 sydeploy/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/utils/simple.py,sha256=fabtM0DAnb9iF28FPIBzAax7isR-aEfTzcWPWyLqBjM,807
-sydeploy-0.2.7.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
-sydeploy-0.2.7.dist-info/METADATA,sha256=Kn-G_fnRqChUj3sGnBeUnMuzPCFshBcR8vbeFurTafs,316
-sydeploy-0.2.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sydeploy-0.2.7.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
-sydeploy-0.2.7.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
-sydeploy-0.2.7.dist-info/RECORD,,
+sydeploy-0.2.7rc0.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
+sydeploy-0.2.7rc0.dist-info/METADATA,sha256=ilkXdflJNQWzPduN6Ed0Q5JgEmqLWBPS2GE_FPO3GVU,319
+sydeploy-0.2.7rc0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sydeploy-0.2.7rc0.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
+sydeploy-0.2.7rc0.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
+sydeploy-0.2.7rc0.dist-info/RECORD,,
```

