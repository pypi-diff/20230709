# Comparing `tmp/fnum-1.2.1-py3-none-any.whl.zip` & `tmp/fnum-1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5747 bytes, number of entries: 11
--rw-r--r--  2.0 unx     4363 b- defN 23-Jul-07 21:09 fnum/__init__.py
--rw-r--r--  2.0 unx       29 b- defN 23-Jul-07 21:09 fnum/__main__.py
--rw-r--r--  2.0 unx     1969 b- defN 23-Jul-07 21:09 fnum/cli.py
--rw-r--r--  2.0 unx       41 b- defN 23-Jul-07 21:09 fnum/exceptions.py
--rw-r--r--  2.0 unx     2086 b- defN 23-Jul-07 21:09 fnum/metadata.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-07 21:10 fnum-1.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1038 b- defN 23-Jul-07 21:10 fnum-1.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 21:10 fnum-1.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-07 21:10 fnum-1.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-07 21:10 fnum-1.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      820 b- defN 23-Jul-07 21:10 fnum-1.2.1.dist-info/RECORD
-11 files, 11550 bytes uncompressed, 4373 bytes compressed:  62.1%
+Zip file size: 5777 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     4363 b- defN 23-Jul-09 06:10 fnum/__init__.py
+-rw-r--r--  2.0 unx       29 b- defN 23-Jul-09 06:10 fnum/__main__.py
+-rw-r--r--  2.0 unx     1969 b- defN 23-Jul-09 06:10 fnum/cli.py
+-rw-r--r--  2.0 unx       41 b- defN 23-Jul-09 06:10 fnum/exceptions.py
+-rw-r--r--  2.0 unx     2117 b- defN 23-Jul-09 06:10 fnum/metadata.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-09 06:10 fnum-1.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1038 b- defN 23-Jul-09 06:10 fnum-1.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 06:10 fnum-1.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-09 06:10 fnum-1.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-09 06:10 fnum-1.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jul-09 06:10 fnum-1.2.2.dist-info/RECORD
+11 files, 11581 bytes uncompressed, 4403 bytes compressed:  62.0%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: fnum/exceptions.py
 Comment: 
 
 Filename: fnum/metadata.py
 Comment: 
 
-Filename: fnum-1.2.1.dist-info/LICENSE
+Filename: fnum-1.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: fnum-1.2.1.dist-info/METADATA
+Filename: fnum-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: fnum-1.2.1.dist-info/WHEEL
+Filename: fnum-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: fnum-1.2.1.dist-info/entry_points.txt
+Filename: fnum-1.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: fnum-1.2.1.dist-info/top_level.txt
+Filename: fnum-1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: fnum-1.2.1.dist-info/RECORD
+Filename: fnum-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fnum/__init__.py

```diff
@@ -2,15 +2,15 @@
 from contextlib import contextmanager
 from imeta import ImageMetadata
 
 from .exceptions import FnumException
 from .metadata import FnumMetadata, FnumMax
 
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 
 def number_files(dirpath, suffixes, progressbar=None, include_imeta=False):
     dirpath = Path(dirpath)
 
     try:
         metadata = FnumMetadata.from_file(dirpath)
```

## fnum/metadata.py

```diff
@@ -15,15 +15,15 @@
     @classmethod
     def from_str(cls, data_str):
         data = yaml.safe_load(data_str)
         return cls(data)
 
     @classmethod
     def from_file(cls, dirpath):
-        data_str = (Path(dirpath) / cls._FILENAME).read_text()
+        data_str = (Path(dirpath) / cls._FILENAME).read_bytes()
         return cls.from_str(data_str)
 
     @classmethod
     def get_default(cls):
         return FnumMetadata(
             {
                 "order": [],
@@ -48,20 +48,20 @@
             data[field] = getattr(self, field)
         for key in self._raw_data.keys():
             if key not in data:
                 data[key] = self._raw_data[key]
         return data.items().__iter__()
 
     def __repr__(self):
-        data_str = yaml.safe_dump(dict(self))
+        data_str = yaml.safe_dump(dict(self), allow_unicode=True)
         return data_str
 
     def to_file(self, dirpath):
-        data_str = str(self)
-        (Path(dirpath) / self._FILENAME).write_text(data_str)
+        data_str = str(self).encode()
+        (Path(dirpath) / self._FILENAME).write_bytes(data_str)
 
 
 class FnumMax:
     _FILENAME = "fnum.max.yaml"
 
     def __init__(self, value):
         self.value = value
```

## Comparing `fnum-1.2.1.dist-info/LICENSE` & `fnum-1.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fnum-1.2.1.dist-info/METADATA` & `fnum-1.2.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnum
-Version: 1.2.1
+Version: 1.2.2
 Summary: Renames files in a directory using sequential integers
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/fnum
 Keywords: fnum,cli,utility,file,rename,sequential,order
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

