# Comparing `tmp/apache-airflow-providers-ssh-3.6.0rc1.tar.gz` & `tmp/apache_airflow_providers_ssh-3.7.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-ssh-3.6.0rc1.tar", last modified: Sun Apr  2 05:49:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

