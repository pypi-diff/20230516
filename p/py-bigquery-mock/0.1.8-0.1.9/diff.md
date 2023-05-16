# Comparing `tmp/py-bigquery-mock-0.1.8.tar.gz` & `tmp/py-bigquery-mock-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-bigquery-mock-0.1.8.tar", last modified: Tue May 16 17:14:51 2023, max compression
+gzip compressed data, was "py-bigquery-mock-0.1.9.tar", last modified: Tue May 16 19:51:55 2023, max compression
```

## Comparing `py-bigquery-mock-0.1.8.tar` & `py-bigquery-mock-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-16 17:14:51.857996 py-bigquery-mock-0.1.8/
--rw-r--r--   0 phtremblay (2028354092) 932231305    35149 2023-05-16 15:50:35.000000 py-bigquery-mock-0.1.8/LICENSE
--rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-16 17:14:51.857822 py-bigquery-mock-0.1.8/PKG-INFO
--rw-r--r--   0 phtremblay (2028354092) 932231305       18 2023-05-16 15:50:35.000000 py-bigquery-mock-0.1.8/README.md
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-16 17:14:51.856855 py-bigquery-mock-0.1.8/bigquery_mock/
--rw-r--r--   0 phtremblay (2028354092) 932231305       52 2023-05-16 16:48:27.000000 py-bigquery-mock-0.1.8/bigquery_mock/__init__.py
--rw-r--r--   0 phtremblay (2028354092) 932231305     2501 2023-05-16 16:40:07.000000 py-bigquery-mock-0.1.8/bigquery_mock/bigquery_mock.py
--rw-r--r--   0 phtremblay (2028354092) 932231305      672 2023-05-16 16:33:05.000000 py-bigquery-mock-0.1.8/bigquery_mock/temp.py
-drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-16 17:14:51.857512 py-bigquery-mock-0.1.8/py_bigquery_mock.egg-info/
--rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-16 17:14:51.000000 py-bigquery-mock-0.1.8/py_bigquery_mock.egg-info/PKG-INFO
--rw-r--r--   0 phtremblay (2028354092) 932231305      265 2023-05-16 17:14:51.000000 py-bigquery-mock-0.1.8/py_bigquery_mock.egg-info/SOURCES.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305        1 2023-05-16 17:14:51.000000 py-bigquery-mock-0.1.8/py_bigquery_mock.egg-info/dependency_links.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305       14 2023-05-16 17:14:51.000000 py-bigquery-mock-0.1.8/py_bigquery_mock.egg-info/top_level.txt
--rw-r--r--   0 phtremblay (2028354092) 932231305       38 2023-05-16 17:14:51.858050 py-bigquery-mock-0.1.8/setup.cfg
--rw-r--r--   0 phtremblay (2028354092) 932231305      407 2023-05-16 16:48:38.000000 py-bigquery-mock-0.1.8/setup.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-16 19:51:55.118710 py-bigquery-mock-0.1.9/
+-rw-r--r--   0 phtremblay (2028354092) 932231305    35149 2023-05-16 15:50:35.000000 py-bigquery-mock-0.1.9/LICENSE
+-rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-16 19:51:55.118582 py-bigquery-mock-0.1.9/PKG-INFO
+-rw-r--r--   0 phtremblay (2028354092) 932231305      458 2023-05-16 19:44:40.000000 py-bigquery-mock-0.1.9/README.md
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-16 19:51:55.117942 py-bigquery-mock-0.1.9/bigquery_mock/
+-rw-r--r--   0 phtremblay (2028354092) 932231305       52 2023-05-16 19:46:21.000000 py-bigquery-mock-0.1.9/bigquery_mock/__init__.py
+-rw-r--r--   0 phtremblay (2028354092) 932231305     2495 2023-05-16 19:24:07.000000 py-bigquery-mock-0.1.9/bigquery_mock/bigquery_mock.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-16 19:51:55.118419 py-bigquery-mock-0.1.9/py_bigquery_mock.egg-info/
+-rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-16 19:51:55.000000 py-bigquery-mock-0.1.9/py_bigquery_mock.egg-info/PKG-INFO
+-rw-r--r--   0 phtremblay (2028354092) 932231305      243 2023-05-16 19:51:55.000000 py-bigquery-mock-0.1.9/py_bigquery_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305        1 2023-05-16 19:51:55.000000 py-bigquery-mock-0.1.9/py_bigquery_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305       14 2023-05-16 19:51:55.000000 py-bigquery-mock-0.1.9/py_bigquery_mock.egg-info/top_level.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305       38 2023-05-16 19:51:55.118753 py-bigquery-mock-0.1.9/setup.cfg
+-rw-r--r--   0 phtremblay (2028354092) 932231305      407 2023-05-16 19:49:28.000000 py-bigquery-mock-0.1.9/setup.py
```

### Comparing `py-bigquery-mock-0.1.8/LICENSE` & `py-bigquery-mock-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py-bigquery-mock-0.1.8/bigquery_mock/bigquery_mock.py` & `py-bigquery-mock-0.1.9/bigquery_mock/bigquery_mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def values(self, *args, **kwargs):
         return self._values
 
     def keys(self, *args, **kwargs):
         return self.info.keys()
 
-class BigQueryMock:
+class Client:
 
     def _test_valid_data(self):
         if not isinstance(self.data, list):
             raise InvalidData(f'{self.data} is not a list')
         errors = []
         for n, i in enumerate(self.data):
             if not isinstance(i, list):
```

