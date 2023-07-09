# Comparing `tmp/poissonate-1.0.tar.gz` & `tmp/poissonate-1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poissonate-1.0.tar", last modified: Sun Jul  9 01:58:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

