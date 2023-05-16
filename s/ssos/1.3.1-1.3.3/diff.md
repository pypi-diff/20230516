# Comparing `tmp/ssos-1.3.1.tar.gz` & `tmp/ssos-1.3.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssos-1.3.1.tar", last modified: Wed Dec  1 17:21:54 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

