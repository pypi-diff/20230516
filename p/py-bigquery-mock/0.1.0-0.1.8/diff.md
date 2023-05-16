# Comparing `tmp/py-bigquery-mock-0.1.0.tar.gz` & `tmp/py-bigquery-mock-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-bigquery-mock-0.1.0.tar", last modified: Tue May 16 05:49:39 2023, max compression
+gzip compressed data, was "py-bigquery-mock-0.1.8.tar", last modified: Tue May 16 17:14:51 2023, max compression
```

## Comparing `py-bigquery-mock-0.1.0.tar` & `py-bigquery-mock-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-16 05:49:39.838984 py-bigquery-mock-0.1.0/
--rw-rw-r--   0 henry     (1000) henry     (1000)    35149 2023-05-16 04:04:28.000000 py-bigquery-mock-0.1.0/LICENSE
--rw-rw-r--   0 henry     (1000) henry     (1000)      339 2023-05-16 05:49:39.838984 py-bigquery-mock-0.1.0/PKG-INFO
--rw-rw-r--   0 henry     (1000) henry     (1000)       18 2023-05-16 04:04:28.000000 py-bigquery-mock-0.1.0/README.md
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-16 05:49:39.838984 py-bigquery-mock-0.1.0/bigquery_mock/
--rw-rw-r--   0 henry     (1000) henry     (1000)       52 2023-05-16 05:47:11.000000 py-bigquery-mock-0.1.0/bigquery_mock/__init__.py
--rw-r--r--   0 henry     (1000) henry     (1000)     1386 2023-05-16 05:19:59.000000 py-bigquery-mock-0.1.0/bigquery_mock/bigquery_mock.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-05-16 05:49:39.838984 py-bigquery-mock-0.1.0/py_bigquery_mock.egg-info/
--rw-rw-r--   0 henry     (1000) henry     (1000)      339 2023-05-16 05:49:39.000000 py-bigquery-mock-0.1.0/py_bigquery_mock.egg-info/PKG-INFO
--rw-rw-r--   0 henry     (1000) henry     (1000)      243 2023-05-16 05:49:39.000000 py-bigquery-mock-0.1.0/py_bigquery_mock.egg-info/SOURCES.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-05-16 05:49:39.000000 py-bigquery-mock-0.1.0/py_bigquery_mock.egg-info/dependency_links.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)       14 2023-05-16 05:49:39.000000 py-bigquery-mock-0.1.0/py_bigquery_mock.egg-info/top_level.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-05-16 05:49:39.838984 py-bigquery-mock-0.1.0/setup.cfg
--rw-rw-r--   0 henry     (1000) henry     (1000)      407 2023-05-16 05:38:47.000000 py-bigquery-mock-0.1.0/setup.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-16 17:14:51.857996 py-bigquery-mock-0.1.8/
+-rw-r--r--   0 phtremblay (2028354092) 932231305    35149 2023-05-16 15:50:35.000000 py-bigquery-mock-0.1.8/LICENSE
+-rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-16 17:14:51.857822 py-bigquery-mock-0.1.8/PKG-INFO
+-rw-r--r--   0 phtremblay (2028354092) 932231305       18 2023-05-16 15:50:35.000000 py-bigquery-mock-0.1.8/README.md
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-16 17:14:51.856855 py-bigquery-mock-0.1.8/bigquery_mock/
+-rw-r--r--   0 phtremblay (2028354092) 932231305       52 2023-05-16 16:48:27.000000 py-bigquery-mock-0.1.8/bigquery_mock/__init__.py
+-rw-r--r--   0 phtremblay (2028354092) 932231305     2501 2023-05-16 16:40:07.000000 py-bigquery-mock-0.1.8/bigquery_mock/bigquery_mock.py
+-rw-r--r--   0 phtremblay (2028354092) 932231305      672 2023-05-16 16:33:05.000000 py-bigquery-mock-0.1.8/bigquery_mock/temp.py
+drwxr-xr-x   0 phtremblay (2028354092) 932231305        0 2023-05-16 17:14:51.857512 py-bigquery-mock-0.1.8/py_bigquery_mock.egg-info/
+-rw-r--r--   0 phtremblay (2028354092) 932231305      311 2023-05-16 17:14:51.000000 py-bigquery-mock-0.1.8/py_bigquery_mock.egg-info/PKG-INFO
+-rw-r--r--   0 phtremblay (2028354092) 932231305      265 2023-05-16 17:14:51.000000 py-bigquery-mock-0.1.8/py_bigquery_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305        1 2023-05-16 17:14:51.000000 py-bigquery-mock-0.1.8/py_bigquery_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305       14 2023-05-16 17:14:51.000000 py-bigquery-mock-0.1.8/py_bigquery_mock.egg-info/top_level.txt
+-rw-r--r--   0 phtremblay (2028354092) 932231305       38 2023-05-16 17:14:51.858050 py-bigquery-mock-0.1.8/setup.cfg
+-rw-r--r--   0 phtremblay (2028354092) 932231305      407 2023-05-16 16:48:38.000000 py-bigquery-mock-0.1.8/setup.py
```

### Comparing `py-bigquery-mock-0.1.0/LICENSE` & `py-bigquery-mock-0.1.8/LICENSE`

 * *Files identical despite different names*

