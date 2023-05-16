# Comparing `tmp/mkdocs_apicall_plugin-0.1.6.tar.gz` & `tmp/mkdocs_apicall_plugin-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_apicall_plugin-0.1.6.tar", max compression
+gzip compressed data, was "mkdocs_apicall_plugin-0.1.7.tar", max compression
```

## Comparing `mkdocs_apicall_plugin-0.1.6.tar` & `mkdocs_apicall_plugin-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-03-27 08:49:55.736765 mkdocs_apicall_plugin-0.1.6/LICENSE
--rw-r--r--   0        0        0     5919 2023-03-27 08:49:55.740765 mkdocs_apicall_plugin-0.1.6/README.md
--rw-r--r--   0        0        0       22 2023-03-27 08:49:55.740765 mkdocs_apicall_plugin-0.1.6/mkdocs_apicall_plugin/__init__.py
--rw-r--r--   0        0        0     2801 2023-03-27 08:49:55.740765 mkdocs_apicall_plugin-0.1.6/mkdocs_apicall_plugin/abstract.py
--rw-r--r--   0        0        0     1078 2023-03-27 08:49:55.740765 mkdocs_apicall_plugin-0.1.6/mkdocs_apicall_plugin/curl.py
--rw-r--r--   0        0        0     1119 2023-03-27 08:49:55.740765 mkdocs_apicall_plugin-0.1.6/mkdocs_apicall_plugin/javascript.py
--rw-r--r--   0        0        0     5625 2023-03-27 08:49:55.740765 mkdocs_apicall_plugin-0.1.6/mkdocs_apicall_plugin/main.py
--rw-r--r--   0        0        0      795 2023-03-27 08:49:55.740765 mkdocs_apicall_plugin-0.1.6/mkdocs_apicall_plugin/python.py
--rw-r--r--   0        0        0      713 2023-03-27 08:49:55.740765 mkdocs_apicall_plugin-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6844 1970-01-01 00:00:00.000000 mkdocs_apicall_plugin-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 09:24:10.142624 mkdocs_apicall_plugin-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5919 2023-05-16 09:24:10.142624 mkdocs_apicall_plugin-0.1.7/README.md
+-rw-r--r--   0        0        0       22 2023-05-16 09:24:10.146624 mkdocs_apicall_plugin-0.1.7/mkdocs_apicall_plugin/__init__.py
+-rw-r--r--   0        0        0     2801 2023-05-16 09:24:10.146624 mkdocs_apicall_plugin-0.1.7/mkdocs_apicall_plugin/abstract.py
+-rw-r--r--   0        0        0     1078 2023-05-16 09:24:10.146624 mkdocs_apicall_plugin-0.1.7/mkdocs_apicall_plugin/curl.py
+-rw-r--r--   0        0        0     1119 2023-05-16 09:24:10.146624 mkdocs_apicall_plugin-0.1.7/mkdocs_apicall_plugin/javascript.py
+-rw-r--r--   0        0        0     5625 2023-05-16 09:24:10.146624 mkdocs_apicall_plugin-0.1.7/mkdocs_apicall_plugin/main.py
+-rw-r--r--   0        0        0      795 2023-05-16 09:24:10.146624 mkdocs_apicall_plugin-0.1.7/mkdocs_apicall_plugin/python.py
+-rw-r--r--   0        0        0      713 2023-05-16 09:24:10.146624 mkdocs_apicall_plugin-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6844 1970-01-01 00:00:00.000000 mkdocs_apicall_plugin-0.1.7/PKG-INFO
```

### Comparing `mkdocs_apicall_plugin-0.1.6/LICENSE` & `mkdocs_apicall_plugin-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_apicall_plugin-0.1.6/README.md` & `mkdocs_apicall_plugin-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_apicall_plugin-0.1.6/mkdocs_apicall_plugin/abstract.py` & `mkdocs_apicall_plugin-0.1.7/mkdocs_apicall_plugin/abstract.py`

 * *Files identical despite different names*

### Comparing `mkdocs_apicall_plugin-0.1.6/mkdocs_apicall_plugin/curl.py` & `mkdocs_apicall_plugin-0.1.7/mkdocs_apicall_plugin/curl.py`

 * *Files identical despite different names*

### Comparing `mkdocs_apicall_plugin-0.1.6/mkdocs_apicall_plugin/javascript.py` & `mkdocs_apicall_plugin-0.1.7/mkdocs_apicall_plugin/javascript.py`

 * *Files identical despite different names*

### Comparing `mkdocs_apicall_plugin-0.1.6/mkdocs_apicall_plugin/main.py` & `mkdocs_apicall_plugin-0.1.7/mkdocs_apicall_plugin/main.py`

 * *Files identical despite different names*

### Comparing `mkdocs_apicall_plugin-0.1.6/mkdocs_apicall_plugin/python.py` & `mkdocs_apicall_plugin-0.1.7/mkdocs_apicall_plugin/python.py`

 * *Files identical despite different names*

### Comparing `mkdocs_apicall_plugin-0.1.6/pyproject.toml` & `mkdocs_apicall_plugin-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-apicall-plugin"
-version = "0.1.6"
+version = "0.1.7"
 description = "Auto-generate code samples to make API calls"
 authors = ["Alban Siffer <alban@situation.sh>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/asiffer/mkdocs-apicall-plugin"
 
 [tool.poetry.dependencies]
```

### Comparing `mkdocs_apicall_plugin-0.1.6/PKG-INFO` & `mkdocs_apicall_plugin-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-apicall-plugin
-Version: 0.1.6
+Version: 0.1.7
 Summary: Auto-generate code samples to make API calls
 Home-page: https://github.com/asiffer/mkdocs-apicall-plugin
 License: Apache-2.0
 Author: Alban Siffer
 Author-email: alban@situation.sh
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: Apache Software License
```

