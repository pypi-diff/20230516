# Comparing `tmp/apache-airflow-providers-sqlite-3.3.2rc1.tar.gz` & `tmp/apache_airflow_providers_sqlite-3.4.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-sqlite-3.3.2rc1.tar", last modified: Fri Apr 21 19:50:07 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

