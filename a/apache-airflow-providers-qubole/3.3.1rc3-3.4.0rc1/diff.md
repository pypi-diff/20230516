# Comparing `tmp/apache-airflow-providers-qubole-3.3.1rc3.tar.gz` & `tmp/apache_airflow_providers_qubole-3.4.0rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-qubole-3.3.1rc3.tar", last modified: Sat Nov 26 10:30:02 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

