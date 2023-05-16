# Comparing `tmp/blockpipe-0.1.2.tar.gz` & `tmp/blockpipe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockpipe-0.1.2.tar", max compression
+gzip compressed data, was "blockpipe-0.1.3.tar", max compression
```

## Comparing `blockpipe-0.1.2.tar` & `blockpipe-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10935 2023-05-12 16:42:57.356759 blockpipe-0.1.2/LICENSE
--rw-r--r--   0        0        0     1791 2023-05-16 01:24:30.517678 blockpipe-0.1.2/README.md
--rw-r--r--   0        0        0      738 2023-05-16 01:24:45.129032 blockpipe-0.1.2/blockpipe/__init__.py
--rw-r--r--   0        0        0      331 2023-05-16 01:25:10.090642 blockpipe-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2126 1970-01-01 00:00:00.000000 blockpipe-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    10935 2023-05-12 16:42:57.356759 blockpipe-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1791 2023-05-16 01:24:30.517678 blockpipe-0.1.3/README.md
+-rw-r--r--   0        0        0      738 2023-05-16 01:24:45.129032 blockpipe-0.1.3/blockpipe/__init__.py
+-rw-r--r--   0        0        0      331 2023-05-16 01:26:38.456060 blockpipe-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2371 1970-01-01 00:00:00.000000 blockpipe-0.1.3/PKG-INFO
```

### Comparing `blockpipe-0.1.2/LICENSE` & `blockpipe-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blockpipe-0.1.2/README.md` & `blockpipe-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `blockpipe-0.1.2/blockpipe/__init__.py` & `blockpipe-0.1.3/blockpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `blockpipe-0.1.2/PKG-INFO` & `blockpipe-0.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: blockpipe
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Sorawit Suriyakarn
 Author-email: thepsint@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.6
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Blockpipe Client for Python
 
 Blockpipe Client is a Python library for interacting with Blockpipe Endpoint API. It provides a simple interface for fetching data from the API and supports both single endpoint and multiple endpoints.
```

