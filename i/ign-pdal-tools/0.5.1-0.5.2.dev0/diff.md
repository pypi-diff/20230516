# Comparing `tmp/ign-pdal-tools-0.5.1.tar.gz` & `tmp/ign_pdal_tools-0.5.2.dev0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ign-pdal-tools-0.5.1.tar", last modified: Mon Apr 17 16:03:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

