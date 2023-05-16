# Comparing `tmp/TuoTuo-0.2.6.tar.gz` & `tmp/TuoTuo-0.2.7-cp38-cp38-macosx_10_14_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TuoTuo-0.2.6.tar", last modified: Wed May  3 20:49:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

