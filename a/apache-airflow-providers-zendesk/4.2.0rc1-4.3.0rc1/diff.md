# Comparing `tmp/apache-airflow-providers-zendesk-4.2.0rc1.tar.gz` & `tmp/apache_airflow_providers_zendesk-4.3.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-zendesk-4.2.0rc1.tar", last modified: Thu Dec  1 14:33:12 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

