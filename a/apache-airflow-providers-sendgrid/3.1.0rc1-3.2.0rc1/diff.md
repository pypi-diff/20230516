# Comparing `tmp/apache-airflow-providers-sendgrid-3.1.0rc1.tar.gz` & `tmp/apache_airflow_providers_sendgrid-3.2.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-sendgrid-3.1.0rc1.tar", last modified: Tue Nov 15 00:15:37 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
