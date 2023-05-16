# Comparing `tmp/highlight_io-0.4.7.tar.gz` & `tmp/highlight_io-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highlight_io-0.4.7.tar", max compression
+gzip compressed data, was "highlight_io-0.4.8.tar", max compression
```

## Comparing `highlight_io-0.4.7.tar` & `highlight_io-0.4.8.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0      350 2023-03-06 07:22:47.581214 highlight_io-0.4.7/README.md
--rw-r--r--   0        0        0       64 2023-03-06 07:22:47.585934 highlight_io-0.4.7/highlight_io/__init__.py
--rw-r--r--   0        0        0      155 2023-03-06 07:22:47.586006 highlight_io-0.4.7/highlight_io/integrations/__init__.py
--rw-r--r--   0        0        0      717 2023-03-21 17:03:02.999163 highlight_io-0.4.7/highlight_io/integrations/aws.py
--rw-r--r--   0        0        0      740 2023-03-21 17:03:02.999423 highlight_io-0.4.7/highlight_io/integrations/azure.py
--rw-r--r--   0        0        0     1631 2023-03-06 07:22:47.586615 highlight_io-0.4.7/highlight_io/integrations/django.py
--rw-r--r--   0        0        0      722 2023-03-06 07:22:47.586847 highlight_io-0.4.7/highlight_io/integrations/fastapi.py
--rw-r--r--   0        0        0     1519 2023-03-06 07:22:47.586917 highlight_io-0.4.7/highlight_io/integrations/flask.py
--rw-r--r--   0        0        0      747 2023-03-21 17:03:02.999649 highlight_io-0.4.7/highlight_io/integrations/gcp.py
--rw-r--r--   0        0        0     1072 2023-03-21 17:03:02.999930 highlight_io-0.4.7/highlight_io/integrations/serverless.py
--rw-r--r--   0        0        0     6801 2023-03-26 23:01:47.736358 highlight_io-0.4.7/highlight_io/sdk.py
--rw-r--r--   0        0        0     1698 2023-03-26 23:01:47.736693 highlight_io-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 highlight_io-0.4.7/setup.py
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 highlight_io-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0      350 2023-05-16 18:48:46.021901 highlight_io-0.4.8/README.md
+-rw-r--r--   0        0        0       64 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/__init__.py
+-rw-r--r--   0        0        0      155 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/__init__.py
+-rw-r--r--   0        0        0      717 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/aws.py
+-rw-r--r--   0        0        0      740 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/azure.py
+-rw-r--r--   0        0        0     1631 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/django.py
+-rw-r--r--   0        0        0      722 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/fastapi.py
+-rw-r--r--   0        0        0     1519 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/flask.py
+-rw-r--r--   0        0        0      747 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/gcp.py
+-rw-r--r--   0        0        0     1072 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/integrations/serverless.py
+-rw-r--r--   0        0        0     6801 2023-05-16 18:48:46.021901 highlight_io-0.4.8/highlight_io/sdk.py
+-rw-r--r--   0        0        0     1698 2023-05-16 18:48:46.021901 highlight_io-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 highlight_io-0.4.8/PKG-INFO
```

### Comparing `highlight_io-0.4.7/highlight_io/integrations/aws.py` & `highlight_io-0.4.8/highlight_io/integrations/aws.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.7/highlight_io/integrations/azure.py` & `highlight_io-0.4.8/highlight_io/integrations/azure.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.7/highlight_io/integrations/django.py` & `highlight_io-0.4.8/highlight_io/integrations/django.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.7/highlight_io/integrations/fastapi.py` & `highlight_io-0.4.8/highlight_io/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.7/highlight_io/integrations/flask.py` & `highlight_io-0.4.8/highlight_io/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.7/highlight_io/integrations/gcp.py` & `highlight_io-0.4.8/highlight_io/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.7/highlight_io/integrations/serverless.py` & `highlight_io-0.4.8/highlight_io/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.7/highlight_io/sdk.py` & `highlight_io-0.4.8/highlight_io/sdk.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.4.7/pyproject.toml` & `highlight_io-0.4.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "highlight-io"
-version = "0.4.7"
+version = "0.4.8"
 description = "Session replay and error monitoring: stop guessing why bugs happen!"
 license = "Apache-2.0"
 authors = [
     "Vadim Korolik <vadim@highlight.io>",
     "Jay Khatri <jay@highlight.io>",
 ]
 readme = "README.md"
```

### Comparing `highlight_io-0.4.7/PKG-INFO` & `highlight_io-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highlight-io
-Version: 0.4.7
+Version: 0.4.8
 Summary: Session replay and error monitoring: stop guessing why bugs happen!
 Home-page: https://www.highlight.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Vadim Korolik
 Author-email: vadim@highlight.io
 Requires-Python: >=3.8,<4.0
```

