# Comparing `tmp/pyBPPIBridge-0.4.4-py3-none-any.whl.zip` & `tmp/pyBPPIBridge-0.4.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 51120 bytes, number of entries: 39
+Zip file size: 51575 bytes, number of entries: 39
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-05 07:02 bppiapi/__init__.py
 -rw-rw-r--  2.0 unx     9566 b- defN 23-Jul-07 16:35 bppiapi/bppiPipeline.py
 -rw-rw-r--  2.0 unx     1188 b- defN 23-May-05 16:17 bppiapi/uploadConfig.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-07 16:35 bppiapi/project/__init__.py
 -rw-rw-r--  2.0 unx      930 b- defN 23-Jul-07 16:35 bppiapi/project/bppiApiProjectWrapper.py
 -rw-rw-r--  2.0 unx      514 b- defN 23-Jul-07 16:35 bppiapi/project/bppiProject.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-07 16:35 bppiapi/repository/__init__.py
@@ -23,19 +23,19 @@
 -rw-rw-r--  2.0 unx    11525 b- defN 23-Jul-07 16:35 pipelines/repository/bppiPLRBluePrismRepo.py
 -rw-rw-r--  2.0 unx     1423 b- defN 23-Jul-07 16:35 pipelines/repository/bppiPLRCSVFile.py
 -rw-rw-r--  2.0 unx     1068 b- defN 23-Jul-07 16:35 pipelines/repository/bppiPLRChorusExtract.py
 -rw-rw-r--  2.0 unx     1606 b- defN 23-Jul-07 16:35 pipelines/repository/bppiPLRExcelFile.py
 -rw-rw-r--  2.0 unx     2437 b- defN 23-Jul-07 16:35 pipelines/repository/bppiPLRODBC.py
 -rw-rw-r--  2.0 unx     5067 b- defN 23-Jul-07 16:35 pipelines/repository/bppiPLRSAPRfcTable.py
 -rw-rw-r--  2.0 unx     1331 b- defN 23-Jul-07 16:35 pipelines/repository/bppiPLRXESFile.py
--rw-rw-r--  2.0 unx      633 b- defN 23-Jul-07 16:35 pyBPPIBridge-0.4.4.data/data/dossier_config/bplogs.sql
--rw-rw-r--  2.0 unx     7128 b- defN 23-Jul-07 16:35 pyBPPIBridge-0.4.4.data/data/dossier_config/config.ddl
--rw-rw-r--  2.0 unx     3458 b- defN 23-Jul-07 16:35 pyBPPIBridge-0.4.4.data/data/dossier_config/config.ini-template
+-rw-rw-r--  2.0 unx      633 b- defN 23-Jul-07 16:35 pyBPPIBridge-0.4.5.data/data/dossier_config/bplogs.sql
+-rw-rw-r--  2.0 unx     7128 b- defN 23-Jul-07 16:35 pyBPPIBridge-0.4.5.data/data/dossier_config/config.ddl
+-rw-rw-r--  2.0 unx     3458 b- defN 23-Jul-07 16:35 pyBPPIBridge-0.4.5.data/data/dossier_config/config.ini-template
 -rw-rw-r--  2.0 unx      537 b- defN 23-Jul-07 16:35 utils/__init__.py
 -rw-rw-r--  2.0 unx     8847 b- defN 23-Jul-07 16:35 utils/constants.py
 -rw-rw-r--  2.0 unx     2016 b- defN 23-Jul-07 16:35 utils/log.py
--rw-rw-r--  2.0 unx    35149 b- defN 23-Jul-09 14:58 pyBPPIBridge-0.4.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1778 b- defN 23-Jul-09 14:58 pyBPPIBridge-0.4.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-09 14:58 pyBPPIBridge-0.4.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       31 b- defN 23-Jul-09 14:58 pyBPPIBridge-0.4.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3444 b- defN 23-Jul-09 14:58 pyBPPIBridge-0.4.4.dist-info/RECORD
-39 files, 144013 bytes uncompressed, 45526 bytes compressed:  68.4%
+-rw-rw-r--  2.0 unx    35149 b- defN 23-Jul-09 16:09 pyBPPIBridge-0.4.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3174 b- defN 23-Jul-09 16:09 pyBPPIBridge-0.4.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-09 16:09 pyBPPIBridge-0.4.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       31 b- defN 23-Jul-09 16:09 pyBPPIBridge-0.4.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3444 b- defN 23-Jul-09 16:09 pyBPPIBridge-0.4.5.dist-info/RECORD
+39 files, 145409 bytes uncompressed, 45981 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -78,41 +78,41 @@
 
 Filename: pipelines/repository/bppiPLRSAPRfcTable.py
 Comment: 
 
 Filename: pipelines/repository/bppiPLRXESFile.py
 Comment: 
 
-Filename: pyBPPIBridge-0.4.4.data/data/dossier_config/bplogs.sql
+Filename: pyBPPIBridge-0.4.5.data/data/dossier_config/bplogs.sql
 Comment: 
 
-Filename: pyBPPIBridge-0.4.4.data/data/dossier_config/config.ddl
+Filename: pyBPPIBridge-0.4.5.data/data/dossier_config/config.ddl
 Comment: 
 
-Filename: pyBPPIBridge-0.4.4.data/data/dossier_config/config.ini-template
+Filename: pyBPPIBridge-0.4.5.data/data/dossier_config/config.ini-template
 Comment: 
 
 Filename: utils/__init__.py
 Comment: 
 
 Filename: utils/constants.py
 Comment: 
 
 Filename: utils/log.py
 Comment: 
 
-Filename: pyBPPIBridge-0.4.4.dist-info/LICENSE
+Filename: pyBPPIBridge-0.4.5.dist-info/LICENSE
 Comment: 
 
-Filename: pyBPPIBridge-0.4.4.dist-info/METADATA
+Filename: pyBPPIBridge-0.4.5.dist-info/METADATA
 Comment: 
 
-Filename: pyBPPIBridge-0.4.4.dist-info/WHEEL
+Filename: pyBPPIBridge-0.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: pyBPPIBridge-0.4.4.dist-info/top_level.txt
+Filename: pyBPPIBridge-0.4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pyBPPIBridge-0.4.4.dist-info/RECORD
+Filename: pyBPPIBridge-0.4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyBPPIBridge-0.4.4.data/data/dossier_config/bplogs.sql` & `pyBPPIBridge-0.4.5.data/data/dossier_config/bplogs.sql`

 * *Files identical despite different names*

## Comparing `pyBPPIBridge-0.4.4.data/data/dossier_config/config.ddl` & `pyBPPIBridge-0.4.5.data/data/dossier_config/config.ddl`

 * *Files identical despite different names*

## Comparing `pyBPPIBridge-0.4.4.data/data/dossier_config/config.ini-template` & `pyBPPIBridge-0.4.5.data/data/dossier_config/config.ini-template`

 * *Files identical despite different names*

## Comparing `pyBPPIBridge-0.4.4.dist-info/LICENSE` & `pyBPPIBridge-0.4.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyBPPIBridge-0.4.4.dist-info/RECORD` & `pyBPPIBridge-0.4.5.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 pipelines/repository/bppiPLRBluePrismRepo.py,sha256=yolHTmTSkMohI9HWMQ_oMiwTveNcCcOV8xJKMacnuuk,11525
 pipelines/repository/bppiPLRCSVFile.py,sha256=8k8gI1w-P4UO3gStETVDtI2heGOdpOq2cb7qZo3Ddtg,1423
 pipelines/repository/bppiPLRChorusExtract.py,sha256=KpfNo1BptSOjP2VlnNPqtlxykVHz-WbWGHJZO7hxoMY,1068
 pipelines/repository/bppiPLRExcelFile.py,sha256=A_neAsONhb43hMwi6ThE5ZsAPhYS35ekgatcIpDfMPE,1606
 pipelines/repository/bppiPLRODBC.py,sha256=-eDrXOt3TvCKPbqGz6sigflSzztaIgWUdOBJ-eIuCBU,2437
 pipelines/repository/bppiPLRSAPRfcTable.py,sha256=oIgi9DY9w_22bHZja_Mq_wnJhAjos191y9_JUWRtoeE,5067
 pipelines/repository/bppiPLRXESFile.py,sha256=d-3EqwE57ve4Ky0yM9tb-SkeFnD8fODO9c-c0MO7FYg,1331
-pyBPPIBridge-0.4.4.data/data/dossier_config/bplogs.sql,sha256=63zhkNkancN97iN6lLKXoWxxndEWEDfbojiwJlYe4xI,633
-pyBPPIBridge-0.4.4.data/data/dossier_config/config.ddl,sha256=Z85hD3CwbLUzjIHXUldQx0sAT3chmHtSxarVSdbMPGY,7128
-pyBPPIBridge-0.4.4.data/data/dossier_config/config.ini-template,sha256=1U1q8lJXifFs1iwP3d4fefJ8kogvgM1YzZde8lxxvD8,3458
+pyBPPIBridge-0.4.5.data/data/dossier_config/bplogs.sql,sha256=63zhkNkancN97iN6lLKXoWxxndEWEDfbojiwJlYe4xI,633
+pyBPPIBridge-0.4.5.data/data/dossier_config/config.ddl,sha256=Z85hD3CwbLUzjIHXUldQx0sAT3chmHtSxarVSdbMPGY,7128
+pyBPPIBridge-0.4.5.data/data/dossier_config/config.ini-template,sha256=1U1q8lJXifFs1iwP3d4fefJ8kogvgM1YzZde8lxxvD8,3458
 utils/__init__.py,sha256=nGIxdrhitBu5XgEjM5Q0sBnWby1TIwhpGU22MCyoKE0,537
 utils/constants.py,sha256=b-q0yJp2LP_31tnno2P1FolBHqk9Ei1pTULK-hB_PzI,8847
 utils/log.py,sha256=i1bNdQV9wOlNjjUFlT5iTxKxgI-li26DI4-IGhU0cI8,2016
-pyBPPIBridge-0.4.4.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-pyBPPIBridge-0.4.4.dist-info/METADATA,sha256=Ek7j4jZBY6OUYbiQyGZXTxhmLPjgoRDfAnX_beIFSU8,1778
-pyBPPIBridge-0.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyBPPIBridge-0.4.4.dist-info/top_level.txt,sha256=Qc9uXZrETiwh2KzNzaKdvRSpdvbtLaWFbKpCG1Et66s,31
-pyBPPIBridge-0.4.4.dist-info/RECORD,,
+pyBPPIBridge-0.4.5.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+pyBPPIBridge-0.4.5.dist-info/METADATA,sha256=iEueDgy_v6jRor57wnK_pJnISbbfQXdVrsy_WWALZXA,3174
+pyBPPIBridge-0.4.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyBPPIBridge-0.4.5.dist-info/top_level.txt,sha256=Qc9uXZrETiwh2KzNzaKdvRSpdvbtLaWFbKpCG1Et66s,31
+pyBPPIBridge-0.4.5.dist-info/RECORD,,
```

