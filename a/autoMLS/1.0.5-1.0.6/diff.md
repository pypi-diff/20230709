# Comparing `tmp/autoMLS-1.0.5-py3-none-any.whl.zip` & `tmp/autoMLS-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -45,13 +45,13 @@
 -rw-r--r--  2.0 unx     1640 b- defN 23-Jun-07 08:38 autoML/AutoTransform/pyimagesearch/imutils.py
 -rw-r--r--  2.0 unx     3444 b- defN 23-Jun-07 08:09 autoML/AutoTransform/pyimagesearch/polygon_interacter.py
 -rw-r--r--  2.0 unx     2715 b- defN 23-Jul-09 07:53 autoML/AutoTransform/pyimagesearch/transform.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 15:02 autoML/CLI/__init__.py
 -rw-r--r--  2.0 unx     5219 b- defN 23-Jul-09 07:53 autoML/CLI/automltoolkit.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 11:10 autoML/api_config/__init__.py
 -rw-r--r--  2.0 unx      633 b- defN 23-Jul-03 08:39 autoML/api_config/pydantic_model.py
--rw-r--r--  2.0 unx     2668 b- defN 23-Jul-09 07:53 autoMLS-1.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 07:53 autoMLS-1.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       74 b- defN 23-Jul-09 07:53 autoMLS-1.0.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-09 07:53 autoMLS-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5744 b- defN 23-Jul-09 07:53 autoMLS-1.0.5.dist-info/RECORD
+-rw-r--r--  2.0 unx     2668 b- defN 23-Jul-09 07:55 autoMLS-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 07:55 autoMLS-1.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       74 b- defN 23-Jul-09 07:55 autoMLS-1.0.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-09 07:55 autoMLS-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5744 b- defN 23-Jul-09 07:55 autoMLS-1.0.6.dist-info/RECORD
 55 files, 138599 bytes uncompressed, 39959 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -144,23 +144,23 @@
 
 Filename: autoML/api_config/__init__.py
 Comment: 
 
 Filename: autoML/api_config/pydantic_model.py
 Comment: 
 
-Filename: autoMLS-1.0.5.dist-info/METADATA
+Filename: autoMLS-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: autoMLS-1.0.5.dist-info/WHEEL
+Filename: autoMLS-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: autoMLS-1.0.5.dist-info/entry_points.txt
+Filename: autoMLS-1.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: autoMLS-1.0.5.dist-info/top_level.txt
+Filename: autoMLS-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: autoMLS-1.0.5.dist-info/RECORD
+Filename: autoMLS-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `autoMLS-1.0.5.dist-info/METADATA` & `autoMLS-1.0.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoMLS
-Version: 1.0.5
+Version: 1.0.6
 Summary: E-kyc for Industries application
 Home-page: https://github.com/aihackervn
 Author: TinVo
 Author-email: tinprocoder0908@gmail.com
 License: MIT
 Keywords: AI HACKER VNESE,AI,autoML,Deep Learning,Computer Vision,Interface
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `autoMLS-1.0.5.dist-info/RECORD` & `autoMLS-1.0.6.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -44,12 +44,12 @@
 autoML/AutoTransform/pyimagesearch/imutils.py,sha256=K7xy2B33G-07s2BVqtYrQSdmT3d-xqEwr1BmsoKDfCE,1640
 autoML/AutoTransform/pyimagesearch/polygon_interacter.py,sha256=lfVkLmwBrnY0GbrbMIqLk-oIrL4qFMzsCDM2OEA2uyA,3444
 autoML/AutoTransform/pyimagesearch/transform.py,sha256=PUGkLUaZuzXhMgWsj2ObkpHztNzuNon51F8G-hoDC0c,2715
 autoML/CLI/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autoML/CLI/automltoolkit.py,sha256=Ot10vozHsYuwPb2cQnQpkN0FA_8stm02TbA-YpH6_Xk,5219
 autoML/api_config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autoML/api_config/pydantic_model.py,sha256=UBu3BmHHw4m68yd44WIXTc1azN54fxNZS8ui3hRZN0E,633
-autoMLS-1.0.5.dist-info/METADATA,sha256=hStiOiqJVMSZFOhwEEQMH45uIz-4EhVpY54SMuNoFog,2668
-autoMLS-1.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-autoMLS-1.0.5.dist-info/entry_points.txt,sha256=NJCA-rvjIUHeUb6HvTdu6GAertrwjlLYmwv55TquBcA,74
-autoMLS-1.0.5.dist-info/top_level.txt,sha256=AT_zKwGhtTY5CMtZai5z7cPq3hBBJtTb88ixK-zyJm0,7
-autoMLS-1.0.5.dist-info/RECORD,,
+autoMLS-1.0.6.dist-info/METADATA,sha256=ZlHqJSsClo3kcw2aditMIcDwwgGgVZMWp5MU02LezPI,2668
+autoMLS-1.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+autoMLS-1.0.6.dist-info/entry_points.txt,sha256=NJCA-rvjIUHeUb6HvTdu6GAertrwjlLYmwv55TquBcA,74
+autoMLS-1.0.6.dist-info/top_level.txt,sha256=AT_zKwGhtTY5CMtZai5z7cPq3hBBJtTb88ixK-zyJm0,7
+autoMLS-1.0.6.dist-info/RECORD,,
```

