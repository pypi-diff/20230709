# Comparing `tmp/xfem-2.1.2303.tar.gz` & `tmp/xfem-2.1.2303.post6.dev0-cp39-cp39-macosx_11_0_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfem-2.1.2303.tar", last modified: Thu Jul  6 10:23:08 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

