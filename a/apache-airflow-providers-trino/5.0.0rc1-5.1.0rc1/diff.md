# Comparing `tmp/apache-airflow-providers-trino-5.0.0rc1.tar.gz` & `tmp/apache_airflow_providers_trino-5.1.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-trino-5.0.0rc1.tar", last modified: Fri Apr 21 19:50:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

