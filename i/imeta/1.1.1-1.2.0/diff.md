# Comparing `tmp/imeta-1.1.1-py3-none-any.whl.zip` & `tmp/imeta-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 4217 bytes, number of entries: 9
--rw-r--r--  2.0 unx     2156 b- defN 23-Jul-09 05:54 imeta/__init__.py
--rw-r--r--  2.0 unx      152 b- defN 23-Jul-09 05:54 imeta/exceptions.py
--rw-r--r--  2.0 unx      849 b- defN 23-Jul-09 05:54 imeta/schema.py
--rw-r--r--  2.0 unx      891 b- defN 23-Jul-09 05:54 imeta/serializer.py
--rw-r--r--  2.0 unx     1881 b- defN 23-Jul-09 05:54 imeta/schema/1.0.json
--rw-r--r--  2.0 unx      931 b- defN 23-Jul-09 05:54 imeta-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 05:54 imeta-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-09 05:54 imeta-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      661 b- defN 23-Jul-09 05:54 imeta-1.1.1.dist-info/RECORD
-9 files, 7619 bytes uncompressed, 3089 bytes compressed:  59.5%
+Zip file size: 5220 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     2996 b- defN 23-Jul-09 19:04 imeta/__init__.py
+-rw-r--r--  2.0 unx      152 b- defN 23-Jul-09 19:04 imeta/exceptions.py
+-rw-r--r--  2.0 unx      849 b- defN 23-Jul-09 19:04 imeta/schema.py
+-rw-r--r--  2.0 unx     1096 b- defN 23-Jul-09 19:04 imeta/serializer.py
+-rw-r--r--  2.0 unx     1893 b- defN 23-Jul-09 19:04 imeta/schema/1.0.json
+-rw-r--r--  2.0 unx     2094 b- defN 23-Jul-09 19:04 imeta/schema/1.1.json
+-rw-r--r--  2.0 unx      931 b- defN 23-Jul-09 19:04 imeta-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 19:04 imeta-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-09 19:04 imeta-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      740 b- defN 23-Jul-09 19:04 imeta-1.2.0.dist-info/RECORD
+10 files, 10849 bytes uncompressed, 3974 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -9,20 +9,23 @@
 
 Filename: imeta/serializer.py
 Comment: 
 
 Filename: imeta/schema/1.0.json
 Comment: 
 
-Filename: imeta-1.1.1.dist-info/METADATA
+Filename: imeta/schema/1.1.json
 Comment: 
 
-Filename: imeta-1.1.1.dist-info/WHEEL
+Filename: imeta-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: imeta-1.1.1.dist-info/top_level.txt
+Filename: imeta-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: imeta-1.1.1.dist-info/RECORD
+Filename: imeta-1.2.0.dist-info/top_level.txt
+Comment: 
+
+Filename: imeta-1.2.0.dist-info/RECORD
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
 
 
-__version__ = "1.1.1"
+__version__ = "1.2.0"
 
 
 class ImageMetadata:
     def __init__(self, data):
         if not isinstance(data, dict) or "$version" not in data:
             raise ValidationError(
                 "Image metadata must contain a top-level $version key"
@@ -44,28 +44,52 @@
     def for_image(cls, filename):
         filepath = Path(filename)
         metapath = filepath.parents[0] / f"{filepath.stem}.json"
         return str(metapath)
 
     @classmethod
     def from_image(cls, filename):
-        return cls.from_file(cls.for_image(filename))
+        filepath = Path(filename)
+        if not filepath.exists() or not filepath.is_file():
+            raise ValidationError(f"Image filename is not a file: {filename}")
+
+        metadata = cls.from_file(cls.for_image(filename))
+
+        if (
+            metadata._serializer._VERSION != "1.0"
+            and filepath.suffix[1:] != metadata.extension
+        ):
+            raise ValidationError(
+                f"Image filename does not have extension {metadata.extension}: {filename}"
+            )
+
+        return metadata
 
     def __iter__(self):
         data = self._serializer.serialize(self)
         data["$version"] = self._serializer._VERSION
+        if self._serializer._VERSION != "1.0":
+            data.move_to_end("extension", last=False)
         data.move_to_end("$version", last=False)
+
         for key in self._raw_data.keys():
             if key not in data:
                 data[key] = self._raw_data[key]
+
         return data.items().__iter__()
 
     def __repr__(self):
         data_str = json.dumps(dict(self), ensure_ascii=False)
         return data_str
 
     def to_file(self, filename):
         data_str = str(self).encode()
         Path(filename).write_bytes(data_str)
 
     def to_image(self, filename):
+        filepath = Path(filename)
+        if self._serializer._VERSION != "1.0" and filepath.suffix[1:] != self.extension:
+            raise ValidationError(
+                f"Image filename does not have extension {self.extension}: {filename}"
+            )
+
         self.to_file(self.for_image(filename))
```

## imeta/serializer.py

```diff
@@ -27,7 +27,19 @@
         data = OrderedDict((field, getattr(metadata, field)) for field in cls._FIELDS)
         return data
 
 
 class V1Serializer(Serializer):
     _VERSION = "1.0"
     _FIELDS = ["source_url", "source_id", "source_name", "access_date", "tags"]
+
+
+class V1_1Serializer(Serializer):
+    _VERSION = "1.1"
+    _FIELDS = [
+        "extension",
+        "source_url",
+        "source_id",
+        "source_name",
+        "access_date",
+        "tags",
+    ]
```

## imeta/schema/1.0.json

### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'description'": "'Describes an image found on the web.'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "$id": "https://raw.githubusercontent.com/healthycrowd/imeta/main/schema/1.0.json",
     "$schema": "https://json-schema.org/draft/2020-12/schema",
-    "description": "Audio rendition resource",
+    "description": "Describes an image found on the web.",
     "properties": {
         "$version": {
             "description": "Version of this schema that should be used for validation.",
             "enum": [
                 "1.0"
             ],
             "type": [
```

## Comparing `imeta-1.1.1.dist-info/METADATA` & `imeta-1.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imeta
-Version: 1.1.1
+Version: 1.2.0
 Summary: Standard for capturing metadata about an image on the web
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/imeta
 Keywords: imeta,utility,image,metadata
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

