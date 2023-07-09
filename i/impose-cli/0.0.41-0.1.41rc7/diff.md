# Comparing `tmp/impose-cli-0.0.41.tar.gz` & `tmp/impose_cli-0.1.41rc7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-cli-0.0.41.tar", last modified: Tue May  9 07:23:08 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

