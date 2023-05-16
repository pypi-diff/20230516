# Comparing `tmp/pypots-0.0.9.tar.gz` & `tmp/pypots-0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypots-0.0.9.tar", last modified: Tue Dec 20 14:04:38 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

