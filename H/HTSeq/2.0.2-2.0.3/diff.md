# Comparing `tmp/HTSeq-2.0.2.tar.gz` & `tmp/HTSeq-2.0.3-cp39-cp39-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/io/wheelhouse/HTSeq-2.0.2.tar", last modified: Sat Jul  2 06:32:49 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

