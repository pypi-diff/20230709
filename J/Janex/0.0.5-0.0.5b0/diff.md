# Comparing `tmp/Janex-0.0.5.tar.gz` & `tmp/Janex-0.0.5b0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Janex-0.0.5.tar", last modified: Sun Jul  9 16:35:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

