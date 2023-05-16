# Comparing `tmp/aida_tools-0.1.1.tar.gz` & `tmp/aida_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aida_tools-0.1.1.tar", max compression
+gzip compressed data, was "aida_tools-0.1.2.tar", max compression
```

## Comparing `aida_tools-0.1.1.tar` & `aida_tools-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,26 @@
--rw-r--r--   0        0        0      588 2023-05-16 14:13:51.801833 aida_tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      351 2023-05-12 14:26:11.085379 aida_tools-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-12 14:21:34.969685 aida_tools-0.1.1/src/aida_tools/__init__.py
--rw-r--r--   0        0        0      798 2023-05-12 14:54:59.187563 aida_tools-0.1.1/src/aida_tools/importer.py
--rw-r--r--   0        0        0      769 2023-05-15 14:49:13.767873 aida_tools-0.1.1/src/aida_tools/utils.py
--rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 aida_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      667 2023-05-16 14:17:07.898262 aida_tools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      351 2023-05-12 14:26:11.085379 aida_tools-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 14:21:34.969685 aida_tools-0.1.2/src/aida_tools/__init__.py
+-rw-r--r--   0        0        0      798 2023-05-12 14:54:59.187563 aida_tools-0.1.2/src/aida_tools/importer.py
+-rw-r--r--   0        0        0      769 2023-05-15 14:49:13.767873 aida_tools-0.1.2/src/aida_tools/utils.py
+-rw-r--r--   0        0        0     5261 2023-05-16 13:52:36.134095 aida_tools-0.1.2/src/cli/autpe/app.py
+-rw-r--r--   0        0        0      897 2023-05-15 15:38:59.462942 aida_tools-0.1.2/src/cli/autpe/config.py
+-rw-r--r--   0        0        0      686 2023-05-12 14:51:08.882329 aida_tools-0.1.2/src/cli/importer.py
+-rw-r--r--   0        0        0     9012 2023-05-15 13:51:25.394549 aida_tools-0.1.2/src/cli/tommasoli/app.py
+-rw-r--r--   0        0        0     1084 2023-05-15 13:50:51.991308 aida_tools-0.1.2/src/cli/tommasoli/config.py
+-rw-r--r--   0        0        0     1770 2023-05-15 13:24:46.493819 aida_tools-0.1.2/src/models/attachment.py
+-rw-r--r--   0        0        0     9788 2023-05-15 16:26:37.548689 aida_tools-0.1.2/src/models/autpe.py
+-rw-r--r--   0        0        0     2035 2023-05-10 10:20:17.801900 aida_tools-0.1.2/src/models/autpe_has_item.py
+-rw-r--r--   0        0        0     2542 2023-05-15 16:25:19.084401 aida_tools-0.1.2/src/models/autpe_has_place.py
+-rw-r--r--   0        0        0     3742 2023-05-15 13:23:59.595273 aida_tools-0.1.2/src/models/date.py
+-rw-r--r--   0        0        0     1118 2023-05-15 15:41:47.205596 aida_tools-0.1.2/src/models/db.py
+-rw-r--r--   0        0        0     2652 2023-05-02 14:18:38.418573 aida_tools-0.1.2/src/models/folder.py
+-rw-r--r--   0        0        0    11735 2023-05-15 14:49:50.826739 aida_tools-0.1.2/src/models/item.py
+-rw-r--r--   0        0        0     2043 2023-05-03 13:07:27.287005 aida_tools-0.1.2/src/models/item_has_place.py
+-rw-r--r--   0        0        0     1698 2023-05-10 10:25:20.053272 aida_tools-0.1.2/src/models/log_form.py
+-rw-r--r--   0        0        0     1447 2023-05-03 09:35:14.702119 aida_tools-0.1.2/src/models/medium.py
+-rw-r--r--   0        0        0     2171 2023-05-15 15:07:12.004097 aida_tools-0.1.2/src/models/mult_value.py
+-rw-r--r--   0        0        0     2367 2023-05-15 13:22:27.476486 aida_tools-0.1.2/src/models/names.py
+-rw-r--r--   0        0        0     1422 2023-04-29 10:00:26.594384 aida_tools-0.1.2/src/models/ogt_d.py
+-rw-r--r--   0        0        0     1218 2023-05-03 09:16:22.878354 aida_tools-0.1.2/src/models/stcc_d.py
+-rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 aida_tools-0.1.2/PKG-INFO
```

### Comparing `aida_tools-0.1.1/pyproject.toml` & `aida_tools-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [tool.poetry]
 name = "aida-tools"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Matteo Spanio <dev2@audioinnova.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
-    {include = "aida_tools", from = "src"}
+    {include = "aida_tools", from = "src"},
+    {include = "cli", from = "src"},
+    {include = "models", from = "src"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 rich = "^13.3.5"
 mariadb = "^1.1.6"
```

### Comparing `aida_tools-0.1.1/src/aida_tools/importer.py` & `aida_tools-0.1.2/src/aida_tools/importer.py`

 * *Files identical despite different names*

### Comparing `aida_tools-0.1.1/src/aida_tools/utils.py` & `aida_tools-0.1.2/src/aida_tools/utils.py`

 * *Files identical despite different names*

### Comparing `aida_tools-0.1.1/PKG-INFO` & `aida_tools-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aida-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Author: Matteo Spanio
 Author-email: dev2@audioinnova.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

