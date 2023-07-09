# Comparing `tmp/calculator_MU-1.0.0.tar.gz` & `tmp/calculator_MU-1.0.1-py3.11.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculator_MU-1.0.0.tar", last modified: Sun Jul  9 13:48:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

