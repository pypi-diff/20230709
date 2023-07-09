# Comparing `tmp/GoldyBot-5.0.dev5.tar.gz` & `tmp/GoldyBot-5.0.dev6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoldyBot-5.0.dev5.tar", last modified: Sat Jul  8 23:43:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

