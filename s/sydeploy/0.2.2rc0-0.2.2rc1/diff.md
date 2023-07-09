# Comparing `tmp/sydeploy-0.2.2rc0.tar.gz` & `tmp/sydeploy-0.2.2rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sydeploy-0.2.2rc0.tar", last modified: Sun Jul  9 17:06:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

