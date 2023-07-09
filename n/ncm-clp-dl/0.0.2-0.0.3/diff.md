# Comparing `tmp/ncm-clp-dl-0.0.2.tar.gz` & `tmp/ncm_clp_dl-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ncm-clp-dl-0.0.2.tar", last modified: Sun Jul  9 03:41:00 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

