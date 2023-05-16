# Comparing `tmp/tensor_processor_learning-1.6.tar.gz` & `tmp/tensor_processor_learning-1.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor_processor_learning-1.6.tar", last modified: Tue May 16 03:57:39 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

