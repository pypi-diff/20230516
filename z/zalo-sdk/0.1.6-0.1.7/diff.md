# Comparing `tmp/zalo_sdk-0.1.6.tar.gz` & `tmp/zalo_sdk-0.1.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zalo_sdk-0.1.6.tar", last modified: Mon May  1 12:04:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

