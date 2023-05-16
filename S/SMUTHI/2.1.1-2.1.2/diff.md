# Comparing `tmp/SMUTHI-2.1.1.tar.gz` & `tmp/SMUTHI-2.1.2-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SMUTHI-2.1.1.tar", last modified: Thu May  4 10:52:50 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

