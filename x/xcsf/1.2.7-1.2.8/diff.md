# Comparing `tmp/xcsf-1.2.7.tar.gz` & `tmp/xcsf-1.2.8-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcsf-1.2.7.tar", last modified: Mon May  1 09:53:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

