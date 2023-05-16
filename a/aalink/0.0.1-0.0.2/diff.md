# Comparing `tmp/aalink-0.0.1.tar.gz` & `tmp/aalink-0.0.2-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aalink-0.0.1.tar", last modified: Mon May 15 18:45:21 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

