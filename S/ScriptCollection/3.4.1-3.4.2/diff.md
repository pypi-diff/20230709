# Comparing `tmp/ScriptCollection-3.4.1-py3-none-any.whl.zip` & `tmp/ScriptCollection-3.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 62303 bytes, number of entries: 14
+Zip file size: 62325 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat    19068 b- defN 23-Jul-09 10:07 ScriptCollection/Executables.py
 -rw-rw-rw-  2.0 fat    34378 b- defN 23-Jun-27 21:57 ScriptCollection/GeneralUtilities.py
 -rw-rw-rw-  2.0 fat     1937 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerBase.py
 -rw-rw-rw-  2.0 fat     6275 b- defN 23-May-26 16:46 ScriptCollection/ProgramRunnerEpew.py
 -rw-rw-rw-  2.0 fat     3023 b- defN 22-Aug-30 21:59 ScriptCollection/ProgramRunnerPopen.py
--rw-rw-rw-  2.0 fat    96083 b- defN 23-Jul-09 10:08 ScriptCollection/ScriptCollectionCore.py
--rw-rw-rw-  2.0 fat   144026 b- defN 23-Jul-09 10:07 ScriptCollection/TasksForCommonProjectStructure.py
+-rw-rw-rw-  2.0 fat    96083 b- defN 23-Jul-09 20:14 ScriptCollection/ScriptCollectionCore.py
+-rw-rw-rw-  2.0 fat   144098 b- defN 23-Jul-09 20:14 ScriptCollection/TasksForCommonProjectStructure.py
 -rw-rw-rw-  2.0 fat     7918 b- defN 22-Aug-30 21:59 ScriptCollection/UpdateCertificates.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Aug-29 05:45 ScriptCollection/__init__.py
--rw-rw-rw-  2.0 fat     7649 b- defN 23-Jul-09 10:08 ScriptCollection-3.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-09 10:08 ScriptCollection-3.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     2088 b- defN 23-Jul-09 10:08 ScriptCollection-3.4.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-09 10:08 ScriptCollection-3.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1290 b- defN 23-Jul-09 10:08 ScriptCollection-3.4.1.dist-info/RECORD
-14 files, 323844 bytes uncompressed, 60121 bytes compressed:  81.4%
+-rw-rw-rw-  2.0 fat     7649 b- defN 23-Jul-09 20:14 ScriptCollection-3.4.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-09 20:14 ScriptCollection-3.4.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     2088 b- defN 23-Jul-09 20:14 ScriptCollection-3.4.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-09 20:14 ScriptCollection-3.4.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1290 b- defN 23-Jul-09 20:14 ScriptCollection-3.4.2.dist-info/RECORD
+14 files, 323916 bytes uncompressed, 60143 bytes compressed:  81.4%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: ScriptCollection/UpdateCertificates.py
 Comment: 
 
 Filename: ScriptCollection/__init__.py
 Comment: 
 
-Filename: ScriptCollection-3.4.1.dist-info/METADATA
+Filename: ScriptCollection-3.4.2.dist-info/METADATA
 Comment: 
 
-Filename: ScriptCollection-3.4.1.dist-info/WHEEL
+Filename: ScriptCollection-3.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: ScriptCollection-3.4.1.dist-info/entry_points.txt
+Filename: ScriptCollection-3.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ScriptCollection-3.4.1.dist-info/top_level.txt
+Filename: ScriptCollection-3.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ScriptCollection-3.4.1.dist-info/RECORD
+Filename: ScriptCollection-3.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ScriptCollection/ScriptCollectionCore.py

```diff
@@ -25,15 +25,15 @@
 import PyPDF2
 from .GeneralUtilities import GeneralUtilities
 from .ProgramRunnerBase import ProgramRunnerBase
 from .ProgramRunnerPopen import ProgramRunnerPopen
 from .ProgramRunnerEpew import ProgramRunnerEpew, CustomEpewArgument
 
 
-version = "3.4.1"
+version = "3.4.2"
 __version__ = version
 
 
 class ScriptCollectionCore:
 
     # The purpose of this property is to use it when testing your code which uses scriptcollection for external program-calls.
     # Do not change this value for productive environments.
```

## ScriptCollection/TasksForCommonProjectStructure.py

```diff
@@ -1526,19 +1526,21 @@
         certificate_file = os.path.join(codeunit_folder, "Other", "Resources", source_constant_name, f"{domain}.crt")
         with open(certificate_file, encoding="utf-8") as text_wrapper:
             certificate = crypto.load_certificate(crypto.FILETYPE_PEM, text_wrapper.read())
         certificate_publickey = crypto.dump_publickey(crypto.FILETYPE_PEM, certificate.get_pubkey()).decode("utf-8")
         self.set_constant(codeunit_folder, source_constant_name+"PublicKey", certificate_publickey)
 
     @GeneralUtilities.check_arguments
-    def set_constants_for_certificate_private_information(self, codeunit_folder: str, certificate_resource_name: str = "DevelopmentCertificate"):
+    def set_constants_for_certificate_private_information(self, codeunit_folder: str, certificate_resource_name: str = "DevelopmentCertificate", domain: str = None):
         """Expects a certificate-resource and generates a constant for its sensitive information in hex-format"""
-        codeunit_name = os.path.basename(codeunit_folder)
-        self.generate_constant_from_resource_by_filename(codeunit_folder, certificate_resource_name, f"{codeunit_name}.test.local.pfx", "PFX")
-        self.generate_constant_from_resource_by_filename(codeunit_folder, certificate_resource_name, f"{codeunit_name}.test.local.password", "Password")
+        if domain is None:
+            codeunit_name = os.path.basename(codeunit_folder)
+            domain=codeunit_name
+        self.generate_constant_from_resource_by_filename(codeunit_folder, certificate_resource_name, f"{domain}.test.local.pfx", "PFX")
+        self.generate_constant_from_resource_by_filename(codeunit_folder, certificate_resource_name, f"{domain}.test.local.password", "Password")
 
     @GeneralUtilities.check_arguments
     def generate_constant_from_resource_by_filename(self, codeunit_folder: str, resource_name: str, filename: str, constant_name: str):
         certificate_resource_folder = GeneralUtilities.resolve_relative_path(f"Other/Resources/{resource_name}", codeunit_folder)
         resource_file = os.path.join(certificate_resource_folder, filename)
         resource_file_content = GeneralUtilities.read_binary_from_file(resource_file)
         resource_file_as_hex = resource_file_content.hex()
```

## Comparing `ScriptCollection-3.4.1.dist-info/METADATA` & `ScriptCollection-3.4.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScriptCollection
-Version: 3.4.1
+Version: 3.4.2
 Summary: The ScriptCollection is the place for reusable scripts.
 Home-page: https://github.com/anionDev/ScriptCollection
 Author: Marius Göcke
 Author-email: marius.goecke@gmail.com
 Project-URL: Documentation, https://aniondev.github.io/ScriptCollectionReference/index.html
 Project-URL: Changelog, https://github.com/anionDev/ScriptCollection/tree/main/Other/Resources/Changelog
 Keywords: package release build management
```

## Comparing `ScriptCollection-3.4.1.dist-info/entry_points.txt` & `ScriptCollection-3.4.2.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `ScriptCollection-3.4.1.dist-info/RECORD` & `ScriptCollection-3.4.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ScriptCollection/Executables.py,sha256=BanfD3ls0ov3ECnsbuyzNstdYjqz_HplreQYJxrB8Ag,19068
 ScriptCollection/GeneralUtilities.py,sha256=vZDiW5lWJRCrIZVs1bTCZ-O5slQnM5dv4GcJ-RTMowY,34378
 ScriptCollection/ProgramRunnerBase.py,sha256=2kyOuoM3oFjBfLc9Q5t5RTz7Ya2CjUxFtB1rBBDmnjU,1937
 ScriptCollection/ProgramRunnerEpew.py,sha256=nIzY4dG6W-xEpkeoTbozwNZtFSIo-bU_W6t6u1AZKtE,6275
 ScriptCollection/ProgramRunnerPopen.py,sha256=HOs1QVnXiQtwXy1_xvH79bWBdd0i-2tUyyLloQBvMto,3023
-ScriptCollection/ScriptCollectionCore.py,sha256=fGgSe24439rYvBd1iDNq3QniX3pzI319Jxy9K9FAGuo,96083
-ScriptCollection/TasksForCommonProjectStructure.py,sha256=b_QoN7vu_F6IxVy6RzzObjhs5mu9EE3VEKRG6NeLu-0,144026
+ScriptCollection/ScriptCollectionCore.py,sha256=6qa2zBQSbxkIBwMZ4heulf6dDhtrMN7gkanutNxeHhk,96083
+ScriptCollection/TasksForCommonProjectStructure.py,sha256=aDhyppnfEgaiLxo4H04fZVJfAjsGisUeexCkq6LyEHo,144098
 ScriptCollection/UpdateCertificates.py,sha256=Go-JJK-YTi7aBB1phlLxypa8GHkmFHBEPB0_TT9G-bw,7918
 ScriptCollection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ScriptCollection-3.4.1.dist-info/METADATA,sha256=XkqpMqaZjnWku2gkdcPlwesxWShk9aNNgbPXJo5L2zc,7649
-ScriptCollection-3.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ScriptCollection-3.4.1.dist-info/entry_points.txt,sha256=dJKdWcH41owxlKx_khj4P7DItr9lhxWP9JU2Dq8GSsQ,2088
-ScriptCollection-3.4.1.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
-ScriptCollection-3.4.1.dist-info/RECORD,,
+ScriptCollection-3.4.2.dist-info/METADATA,sha256=evfc3SpJ8Vv-CaWAdN61NruiT4me5XscExweMZkxWUw,7649
+ScriptCollection-3.4.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ScriptCollection-3.4.2.dist-info/entry_points.txt,sha256=dJKdWcH41owxlKx_khj4P7DItr9lhxWP9JU2Dq8GSsQ,2088
+ScriptCollection-3.4.2.dist-info/top_level.txt,sha256=hY2hOVH0V0Ce51WB76zKkIWTUNwMUdHo4XDkR2vYVwg,17
+ScriptCollection-3.4.2.dist-info/RECORD,,
```

