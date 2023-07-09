# Comparing `tmp/klujax-0.2.0.tar.gz` & `tmp/klujax-0.2.2-pp39-pypy39_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klujax-0.2.0.tar", last modified: Sun Jul  2 02:34:02 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

