# Comparing `tmp/impose-cli-0.1.41rc8.tar.gz` & `tmp/impose_cli-0.1.41rc9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-cli-0.1.41rc8.tar", last modified: Sun Jul  9 08:19:54 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

