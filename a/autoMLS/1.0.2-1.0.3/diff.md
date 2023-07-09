# Comparing `tmp/autoMLS-1.0.2-py3-none-any.whl.zip` & `tmp/autoMLS-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 49607 bytes, number of entries: 55
+Zip file size: 49629 bytes, number of entries: 55
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-24 13:34 autoML/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-01 12:14 autoML/AutoDetect/__init__.py
 -rw-r--r--  2.0 unx     8588 b- defN 23-Jul-09 05:25 autoML/AutoDetect/auto_detect.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 07:19 autoML/AutoDetect/vietnamese_nlp/__init__.py
 -rw-r--r--  2.0 unx     2581 b- defN 23-Jul-09 05:25 autoML/AutoDetect/vietnamese_nlp/nlp_onnx.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 07:19 autoML/AutoDetect/vietnamese_nlp/vietocr/__init__.py
 -rw-r--r--  2.0 unx      614 b- defN 23-Jul-09 05:25 autoML/AutoDetect/vietnamese_nlp/vietocr/predict.py
@@ -42,16 +42,16 @@
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 03:16 autoML/AutoTransform/__init__.py
 -rw-r--r--  2.0 unx    12182 b- defN 23-Jul-09 05:25 autoML/AutoTransform/auto_four_point_transform.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 15:03 autoML/AutoTransform/pyimagesearch/__init__.py
 -rw-r--r--  2.0 unx     1640 b- defN 23-Jun-07 08:38 autoML/AutoTransform/pyimagesearch/imutils.py
 -rw-r--r--  2.0 unx     3444 b- defN 23-Jun-07 08:09 autoML/AutoTransform/pyimagesearch/polygon_interacter.py
 -rw-r--r--  2.0 unx     2720 b- defN 23-Jun-07 08:09 autoML/AutoTransform/pyimagesearch/transform.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 15:02 autoML/CLI/__init__.py
--rw-r--r--  2.0 unx     5234 b- defN 23-Jul-09 05:33 autoML/CLI/main.py
+-rw-r--r--  2.0 unx     5234 b- defN 23-Jul-09 05:33 autoML/CLI/automltoolkit.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 11:10 autoML/api_config/__init__.py
 -rw-r--r--  2.0 unx      633 b- defN 23-Jul-03 08:39 autoML/api_config/pydantic_model.py
--rw-r--r--  2.0 unx     2652 b- defN 23-Jul-09 05:41 autoMLS-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 05:41 autoMLS-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-Jul-09 05:41 autoMLS-1.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-09 05:41 autoMLS-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5735 b- defN 23-Jul-09 05:41 autoMLS-1.0.2.dist-info/RECORD
-55 files, 138856 bytes uncompressed, 39981 bytes compressed:  71.2%
+-rw-r--r--  2.0 unx     2652 b- defN 23-Jul-09 07:43 autoMLS-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 07:43 autoMLS-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Jul-09 07:43 autoMLS-1.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-09 07:43 autoMLS-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5744 b- defN 23-Jul-09 07:43 autoMLS-1.0.3.dist-info/RECORD
+55 files, 138869 bytes uncompressed, 39985 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -135,32 +135,32 @@
 
 Filename: autoML/AutoTransform/pyimagesearch/transform.py
 Comment: 
 
 Filename: autoML/CLI/__init__.py
 Comment: 
 
-Filename: autoML/CLI/main.py
+Filename: autoML/CLI/automltoolkit.py
 Comment: 
 
 Filename: autoML/api_config/__init__.py
 Comment: 
 
 Filename: autoML/api_config/pydantic_model.py
 Comment: 
 
-Filename: autoMLS-1.0.2.dist-info/METADATA
+Filename: autoMLS-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: autoMLS-1.0.2.dist-info/WHEEL
+Filename: autoMLS-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: autoMLS-1.0.2.dist-info/entry_points.txt
+Filename: autoMLS-1.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: autoMLS-1.0.2.dist-info/top_level.txt
+Filename: autoMLS-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: autoMLS-1.0.2.dist-info/RECORD
+Filename: autoMLS-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `autoML/CLI/main.py` & `autoML/CLI/automltoolkit.py`

 * *Files identical despite different names*

## Comparing `autoMLS-1.0.2.dist-info/METADATA` & `autoMLS-1.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoMLS
-Version: 1.0.2
+Version: 1.0.3
 Summary: E-kyc for Industries application
 Home-page: https://github.com/aihackervn
 Author: TinVo
 Author-email: tinprocoder0908@gmail.com
 License: MIT
 Keywords: AI,autoML,Deep Learning,Computer Vision,Interface
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `autoMLS-1.0.2.dist-info/RECORD` & `autoMLS-1.0.3.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 autoML/AutoTransform/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autoML/AutoTransform/auto_four_point_transform.py,sha256=sCFfkaMGFWb7UuHFL9pBnVdAE_2WdaghN1KsE4i9-ks,12182
 autoML/AutoTransform/pyimagesearch/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autoML/AutoTransform/pyimagesearch/imutils.py,sha256=K7xy2B33G-07s2BVqtYrQSdmT3d-xqEwr1BmsoKDfCE,1640
 autoML/AutoTransform/pyimagesearch/polygon_interacter.py,sha256=lfVkLmwBrnY0GbrbMIqLk-oIrL4qFMzsCDM2OEA2uyA,3444
 autoML/AutoTransform/pyimagesearch/transform.py,sha256=hFPQ0PLTfo3Zewgshy_sGb4PyqxU2g_v0MckT2R6jfE,2720
 autoML/CLI/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-autoML/CLI/main.py,sha256=dEYjPljfVQPHyPHxSLp8hRfdi6wtajtRP2-XSGx3If0,5234
+autoML/CLI/automltoolkit.py,sha256=dEYjPljfVQPHyPHxSLp8hRfdi6wtajtRP2-XSGx3If0,5234
 autoML/api_config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autoML/api_config/pydantic_model.py,sha256=UBu3BmHHw4m68yd44WIXTc1azN54fxNZS8ui3hRZN0E,633
-autoMLS-1.0.2.dist-info/METADATA,sha256=k8AkxFtsS9QeakJw5bQ9piKrNU__f9ULIFkKuH9HiFc,2652
-autoMLS-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-autoMLS-1.0.2.dist-info/entry_points.txt,sha256=nyKWMvimeYFV79TcUr5zt9V06vFFOGv21EE_WuNgag8,55
-autoMLS-1.0.2.dist-info/top_level.txt,sha256=AT_zKwGhtTY5CMtZai5z7cPq3hBBJtTb88ixK-zyJm0,7
-autoMLS-1.0.2.dist-info/RECORD,,
+autoMLS-1.0.3.dist-info/METADATA,sha256=RRkhICoICzCSJ4oPlALxvJx8viL4gaMnwk0hYeOETbk,2652
+autoMLS-1.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+autoMLS-1.0.3.dist-info/entry_points.txt,sha256=0DGXveGU_LCNF3oLucdc-2QlshgdiQGXJpt_ViRKEv0,59
+autoMLS-1.0.3.dist-info/top_level.txt,sha256=AT_zKwGhtTY5CMtZai5z7cPq3hBBJtTb88ixK-zyJm0,7
+autoMLS-1.0.3.dist-info/RECORD,,
```

