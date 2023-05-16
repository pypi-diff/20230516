# Comparing `tmp/getCalspec-2.0.0.tar.gz` & `tmp/getCalspec-2.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jneveu/Documents/LSST/Calibration/getCalspec/dist/.tmp-1pt_0_15/getCalspec-2.0.0.tar", last modified: Wed Mar  8 13:41:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

