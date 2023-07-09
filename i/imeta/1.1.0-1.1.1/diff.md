# Comparing `tmp/imeta-1.1.0-py3-none-any.whl.zip` & `tmp/imeta-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4196 bytes, number of entries: 9
--rw-r--r--  2.0 unx     2125 b- defN 23-Jul-07 19:16 imeta/__init__.py
--rw-r--r--  2.0 unx      152 b- defN 23-Jul-07 19:16 imeta/exceptions.py
--rw-r--r--  2.0 unx      849 b- defN 23-Jul-07 19:16 imeta/schema.py
--rw-r--r--  2.0 unx      891 b- defN 23-Jul-07 19:16 imeta/serializer.py
--rw-r--r--  2.0 unx     1881 b- defN 23-Jul-07 19:16 imeta/schema/1.0.json
--rw-r--r--  2.0 unx      931 b- defN 23-Jul-07 19:16 imeta-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 19:16 imeta-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-07 19:16 imeta-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      661 b- defN 23-Jul-07 19:16 imeta-1.1.0.dist-info/RECORD
-9 files, 7588 bytes uncompressed, 3068 bytes compressed:  59.6%
+Zip file size: 4217 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     2156 b- defN 23-Jul-09 05:54 imeta/__init__.py
+-rw-r--r--  2.0 unx      152 b- defN 23-Jul-09 05:54 imeta/exceptions.py
+-rw-r--r--  2.0 unx      849 b- defN 23-Jul-09 05:54 imeta/schema.py
+-rw-r--r--  2.0 unx      891 b- defN 23-Jul-09 05:54 imeta/serializer.py
+-rw-r--r--  2.0 unx     1881 b- defN 23-Jul-09 05:54 imeta/schema/1.0.json
+-rw-r--r--  2.0 unx      931 b- defN 23-Jul-09 05:54 imeta-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 05:54 imeta-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-09 05:54 imeta-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      661 b- defN 23-Jul-09 05:54 imeta-1.1.1.dist-info/RECORD
+9 files, 7619 bytes uncompressed, 3089 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: imeta/serializer.py
 Comment: 
 
 Filename: imeta/schema/1.0.json
 Comment: 
 
-Filename: imeta-1.1.0.dist-info/METADATA
+Filename: imeta-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: imeta-1.1.0.dist-info/WHEEL
+Filename: imeta-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: imeta-1.1.0.dist-info/top_level.txt
+Filename: imeta-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: imeta-1.1.0.dist-info/RECORD
+Filename: imeta-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## imeta/__init__.py

```diff
@@ -3,15 +3,15 @@
 from jsonschema.validators import validator_for
 
 from .schema import Schema
 from .serializer import Serializer
 from .exceptions import ValidationError
 
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 
 class ImageMetadata:
     def __init__(self, data):
         if not isinstance(data, dict) or "$version" not in data:
             raise ValidationError(
                 "Image metadata must contain a top-level $version key"
@@ -33,15 +33,15 @@
     @classmethod
     def from_str(cls, data_str):
         data = json.loads(data_str)
         return cls(data)
 
     @classmethod
     def from_file(cls, filename):
-        data_str = Path(filename).read_text()
+        data_str = Path(filename).read_bytes()
         return cls.from_str(data_str)
 
     @classmethod
     def for_image(cls, filename):
         filepath = Path(filename)
         metapath = filepath.parents[0] / f"{filepath.stem}.json"
         return str(metapath)
@@ -56,16 +56,16 @@
         data.move_to_end("$version", last=False)
         for key in self._raw_data.keys():
             if key not in data:
                 data[key] = self._raw_data[key]
         return data.items().__iter__()
 
     def __repr__(self):
-        data_str = json.dumps(dict(self))
+        data_str = json.dumps(dict(self), ensure_ascii=False)
         return data_str
 
     def to_file(self, filename):
-        data_str = str(self)
-        Path(filename).write_text(data_str)
+        data_str = str(self).encode()
+        Path(filename).write_bytes(data_str)
 
     def to_image(self, filename):
         self.to_file(self.for_image(filename))
```

## Comparing `imeta-1.1.0.dist-info/METADATA` & `imeta-1.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imeta
-Version: 1.1.0
+Version: 1.1.1
 Summary: Standard for capturing metadata about an image on the web
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/imeta
 Keywords: imeta,utility,image,metadata
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `imeta-1.1.0.dist-info/RECORD` & `imeta-1.1.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-imeta/__init__.py,sha256=B95mY22kW_9lRn5hE4BHxrRiay3GmKjlBY3Z9rfxTcQ,2125
+imeta/__init__.py,sha256=DuZWbtBbo8TP2ghTrSWCW7TSQuEt3Tl0Us5qB8op5Ug,2156
 imeta/exceptions.py,sha256=LsmGqVLqWROo3n_s3y7ktJJvra2SoCYuHIOpsakW5aw,152
 imeta/schema.py,sha256=MQa2yHJoo7mHw77DlQR_G-H2dLGMizkrADT4SUbes8o,849
 imeta/serializer.py,sha256=AjIfx7nCKIDiDbwsjhukH6GLTJcQ60hNkwZcZmDlmPU,891
 imeta/schema/1.0.json,sha256=h199lN1CXr8fDq1n8s_mpmv_kjWBcCKVDKrTVrVIshg,1881
-imeta-1.1.0.dist-info/METADATA,sha256=9KshWfpUyX02ab2kN-zA7Qd7kRHPeIvfL25JSyxxugU,931
-imeta-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-imeta-1.1.0.dist-info/top_level.txt,sha256=FBV8zF4u9Jdo2epLMcKy2JDK2csjrdQLIAGvi3alf9Y,6
-imeta-1.1.0.dist-info/RECORD,,
+imeta-1.1.1.dist-info/METADATA,sha256=slyv-xG4TFXorHunsugG1ctsE_5pA6LJALzILy4ee1Q,931
+imeta-1.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+imeta-1.1.1.dist-info/top_level.txt,sha256=FBV8zF4u9Jdo2epLMcKy2JDK2csjrdQLIAGvi3alf9Y,6
+imeta-1.1.1.dist-info/RECORD,,
```

