# Comparing `tmp/autoMLS-1.0.6-py3-none-any.whl.zip` & `tmp/autoMLS-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 49603 bytes, number of entries: 55
+Zip file size: 49705 bytes, number of entries: 55
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-24 13:34 autoML/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-01 12:14 autoML/AutoDetect/__init__.py
 -rw-r--r--  2.0 unx     8573 b- defN 23-Jul-09 07:53 autoML/AutoDetect/auto_detect.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 07:19 autoML/AutoDetect/vietnamese_nlp/__init__.py
 -rw-r--r--  2.0 unx     2571 b- defN 23-Jul-09 07:53 autoML/AutoDetect/vietnamese_nlp/nlp_onnx.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 07:19 autoML/AutoDetect/vietnamese_nlp/vietocr/__init__.py
 -rw-r--r--  2.0 unx      614 b- defN 23-Jul-09 05:25 autoML/AutoDetect/vietnamese_nlp/vietocr/predict.py
@@ -42,16 +42,16 @@
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 03:16 autoML/AutoTransform/__init__.py
 -rw-r--r--  2.0 unx    12177 b- defN 23-Jul-09 07:53 autoML/AutoTransform/auto_four_point_transform.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 15:03 autoML/AutoTransform/pyimagesearch/__init__.py
 -rw-r--r--  2.0 unx     1640 b- defN 23-Jun-07 08:38 autoML/AutoTransform/pyimagesearch/imutils.py
 -rw-r--r--  2.0 unx     3444 b- defN 23-Jun-07 08:09 autoML/AutoTransform/pyimagesearch/polygon_interacter.py
 -rw-r--r--  2.0 unx     2715 b- defN 23-Jul-09 07:53 autoML/AutoTransform/pyimagesearch/transform.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 15:02 autoML/CLI/__init__.py
--rw-r--r--  2.0 unx     5219 b- defN 23-Jul-09 07:53 autoML/CLI/automltoolkit.py
+-rw-r--r--  2.0 unx     5143 b- defN 23-Jul-09 07:58 autoML/CLI/automltoolkit.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 11:10 autoML/api_config/__init__.py
 -rw-r--r--  2.0 unx      633 b- defN 23-Jul-03 08:39 autoML/api_config/pydantic_model.py
--rw-r--r--  2.0 unx     2668 b- defN 23-Jul-09 07:55 autoMLS-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 07:55 autoMLS-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       74 b- defN 23-Jul-09 07:55 autoMLS-1.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-09 07:55 autoMLS-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5744 b- defN 23-Jul-09 07:55 autoMLS-1.0.6.dist-info/RECORD
-55 files, 138599 bytes uncompressed, 39959 bytes compressed:  71.2%
+-rw-r--r--  2.0 unx     3248 b- defN 23-Jul-09 08:00 autoMLS-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 08:00 autoMLS-1.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       74 b- defN 23-Jul-09 08:00 autoMLS-1.0.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-09 08:00 autoMLS-1.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5744 b- defN 23-Jul-09 08:00 autoMLS-1.0.7.dist-info/RECORD
+55 files, 139103 bytes uncompressed, 40061 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -144,23 +144,23 @@
 
 Filename: autoML/api_config/__init__.py
 Comment: 
 
 Filename: autoML/api_config/pydantic_model.py
 Comment: 
 
-Filename: autoMLS-1.0.6.dist-info/METADATA
+Filename: autoMLS-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: autoMLS-1.0.6.dist-info/WHEEL
+Filename: autoMLS-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: autoMLS-1.0.6.dist-info/entry_points.txt
+Filename: autoMLS-1.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: autoMLS-1.0.6.dist-info/top_level.txt
+Filename: autoMLS-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: autoMLS-1.0.6.dist-info/RECORD
+Filename: autoMLS-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## autoML/CLI/automltoolkit.py

```diff
@@ -124,8 +124,7 @@
 
         input("Press Enter to continue...")
         print()
 
 
 if __name__ == '__main__':
     start_terminal_loop()
-# qr, id , name, birth, gender, country, home, add, valid, p, c, po, l, r,m
```

## Comparing `autoMLS-1.0.6.dist-info/METADATA` & `autoMLS-1.0.7.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,93 @@
 Metadata-Version: 2.1
 Name: autoMLS
-Version: 1.0.6
+Version: 1.0.7
 Summary: E-kyc for Industries application
 Home-page: https://github.com/aihackervn
 Author: TinVo
 Author-email: tinprocoder0908@gmail.com
 License: MIT
 Keywords: AI HACKER VNESE,AI,autoML,Deep Learning,Computer Vision,Interface
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: annotated-types (==0.5.0)
 Requires-Dist: anyio (==3.7.1)
 Requires-Dist: beautifulsoup4 (==4.12.2)
+Requires-Dist: bleach (==6.0.0)
 Requires-Dist: certifi (==2023.5.7)
 Requires-Dist: charset-normalizer (==3.2.0)
 Requires-Dist: coloredlogs (==15.0.1)
 Requires-Dist: contourpy (==1.1.0)
 Requires-Dist: cycler (==0.11.0)
+Requires-Dist: docutils (==0.20.1)
 Requires-Dist: einops (==0.6.1)
 Requires-Dist: exceptiongroup (==1.1.2)
 Requires-Dist: fastapi (==0.100.0)
 Requires-Dist: filelock (==3.12.2)
 Requires-Dist: flatbuffers (==23.5.26)
 Requires-Dist: fonttools (==4.40.0)
 Requires-Dist: gdown (==4.7.1)
 Requires-Dist: humanfriendly (==10.0)
 Requires-Dist: idna (==3.4)
+Requires-Dist: importlib-metadata (==6.8.0)
 Requires-Dist: importlib-resources (==6.0.0)
+Requires-Dist: jaraco.classes (==3.3.0)
 Requires-Dist: Jinja2 (==3.1.2)
 Requires-Dist: joblib (==1.3.1)
+Requires-Dist: keyring (==24.2.0)
 Requires-Dist: kiwisolver (==1.4.4)
+Requires-Dist: markdown-it-py (==3.0.0)
 Requires-Dist: MarkupSafe (==2.1.3)
 Requires-Dist: matplotlib (==3.7.2)
+Requires-Dist: mdurl (==0.1.2)
+Requires-Dist: more-itertools (==9.1.0)
 Requires-Dist: mpmath (==1.3.0)
 Requires-Dist: networkx (==3.1)
-Requires-Dist: numpy (==1.24.4)
+Requires-Dist: numpy (==1.25.0)
 Requires-Dist: onnxruntime (==1.15.1)
 Requires-Dist: opencv-python (==4.8.0.74)
 Requires-Dist: packaging (==23.1)
 Requires-Dist: pandas (==2.0.3)
 Requires-Dist: Pillow (==10.0.0)
+Requires-Dist: pkginfo (==1.9.6)
 Requires-Dist: protobuf (==4.23.4)
 Requires-Dist: psutil (==5.9.5)
 Requires-Dist: pydantic (==2.0.2)
 Requires-Dist: pydantic-core (==2.1.2)
+Requires-Dist: Pygments (==2.15.1)
 Requires-Dist: pyparsing (==3.0.9)
 Requires-Dist: PySocks (==1.7.1)
 Requires-Dist: python-dateutil (==2.8.2)
 Requires-Dist: pytz (==2023.3)
 Requires-Dist: PyYAML (==6.0)
+Requires-Dist: readme-renderer (==40.0)
 Requires-Dist: requests (==2.31.0)
+Requires-Dist: requests-toolbelt (==1.0.0)
+Requires-Dist: rfc3986 (==2.0.0)
+Requires-Dist: rich (==13.4.2)
 Requires-Dist: scikit-learn (==1.3.0)
 Requires-Dist: scipy (==1.11.1)
 Requires-Dist: seaborn (==0.12.2)
 Requires-Dist: six (==1.16.0)
 Requires-Dist: sniffio (==1.3.0)
 Requires-Dist: soupsieve (==2.4.1)
 Requires-Dist: starlette (==0.27.0)
 Requires-Dist: sympy (==1.12)
 Requires-Dist: threadpoolctl (==3.1.0)
 Requires-Dist: torch (==2.0.1)
 Requires-Dist: torchvision (==0.15.2)
 Requires-Dist: tqdm (==4.65.0)
+Requires-Dist: twine (==4.0.2)
 Requires-Dist: typing-extensions (==4.7.1)
 Requires-Dist: tzdata (==2023.3)
 Requires-Dist: ultralytics (==8.0.131)
 Requires-Dist: urllib3 (==2.0.3)
+Requires-Dist: webencodings (==0.5.1)
 Requires-Dist: wget (==3.2)
 Requires-Dist: zipp (==3.15.0)
 Provides-Extra: dev
 Requires-Dist: pytest (>=7.0) ; extra == 'dev'
 Requires-Dist: twine (>=4.0.2) ; extra == 'dev'
```

## Comparing `autoMLS-1.0.6.dist-info/RECORD` & `autoMLS-1.0.7.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 autoML/AutoTransform/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autoML/AutoTransform/auto_four_point_transform.py,sha256=FqZHB4G8z7Zco_6292NnsvJ25FJn1k_4fKL1Jg9A744,12177
 autoML/AutoTransform/pyimagesearch/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autoML/AutoTransform/pyimagesearch/imutils.py,sha256=K7xy2B33G-07s2BVqtYrQSdmT3d-xqEwr1BmsoKDfCE,1640
 autoML/AutoTransform/pyimagesearch/polygon_interacter.py,sha256=lfVkLmwBrnY0GbrbMIqLk-oIrL4qFMzsCDM2OEA2uyA,3444
 autoML/AutoTransform/pyimagesearch/transform.py,sha256=PUGkLUaZuzXhMgWsj2ObkpHztNzuNon51F8G-hoDC0c,2715
 autoML/CLI/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-autoML/CLI/automltoolkit.py,sha256=Ot10vozHsYuwPb2cQnQpkN0FA_8stm02TbA-YpH6_Xk,5219
+autoML/CLI/automltoolkit.py,sha256=oJaUQKYdA6rqMwfPizkwSN42yRx7YA2pYAII8gr99KE,5143
 autoML/api_config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autoML/api_config/pydantic_model.py,sha256=UBu3BmHHw4m68yd44WIXTc1azN54fxNZS8ui3hRZN0E,633
-autoMLS-1.0.6.dist-info/METADATA,sha256=ZlHqJSsClo3kcw2aditMIcDwwgGgVZMWp5MU02LezPI,2668
-autoMLS-1.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-autoMLS-1.0.6.dist-info/entry_points.txt,sha256=NJCA-rvjIUHeUb6HvTdu6GAertrwjlLYmwv55TquBcA,74
-autoMLS-1.0.6.dist-info/top_level.txt,sha256=AT_zKwGhtTY5CMtZai5z7cPq3hBBJtTb88ixK-zyJm0,7
-autoMLS-1.0.6.dist-info/RECORD,,
+autoMLS-1.0.7.dist-info/METADATA,sha256=90DuGJUIdZuW7EueMoy40Y24yA-dJUoNvWTAOA5iZD0,3248
+autoMLS-1.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+autoMLS-1.0.7.dist-info/entry_points.txt,sha256=NJCA-rvjIUHeUb6HvTdu6GAertrwjlLYmwv55TquBcA,74
+autoMLS-1.0.7.dist-info/top_level.txt,sha256=AT_zKwGhtTY5CMtZai5z7cPq3hBBJtTb88ixK-zyJm0,7
+autoMLS-1.0.7.dist-info/RECORD,,
```

