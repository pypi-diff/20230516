# Comparing `tmp/lz_import-0.1.0.tar.gz` & `tmp/lz_import-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lz_import-0.1.0.tar", max compression
+gzip compressed data, was "lz_import-0.1.1.tar", max compression
```

## Comparing `lz_import-0.1.0.tar` & `lz_import-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1415 2023-05-16 10:04:15.715763 lz_import-0.1.0/README.md
--rw-r--r--   0        0        0      164 2023-05-16 10:04:15.715763 lz_import-0.1.0/lazy_import/__init__.py
--rw-r--r--   0        0        0     8893 2023-05-16 10:04:15.715763 lz_import-0.1.0/lazy_import/lazy_import.py
--rw-r--r--   0        0        0        0 2023-05-16 10:04:15.715763 lz_import-0.1.0/lazy_import/py.typed
--rw-r--r--   0        0        0     1005 2023-05-16 10:04:15.715763 lz_import-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2054 1970-01-01 00:00:00.000000 lz_import-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1489 2023-05-16 10:08:15.158864 lz_import-0.1.1/README.md
+-rw-r--r--   0        0        0      164 2023-05-16 10:08:15.158864 lz_import-0.1.1/lazy_import/__init__.py
+-rw-r--r--   0        0        0     8893 2023-05-16 10:08:15.158864 lz_import-0.1.1/lazy_import/lazy_import.py
+-rw-r--r--   0        0        0        0 2023-05-16 10:08:15.158864 lz_import-0.1.1/lazy_import/py.typed
+-rw-r--r--   0        0        0      987 2023-05-16 10:08:15.158864 lz_import-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2089 1970-01-01 00:00:00.000000 lz_import-0.1.1/PKG-INFO
```

### Comparing `lz_import-0.1.0/README.md` & `lz_import-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Lazy Import
 
+### Installation
+```
+pip install lz-import
+# Or
+poetry add lz-import
+```
+
 ### Usage
 ```python
 # File: company.py
 from user import User
 
 class Company:
     name = "company"
```

### Comparing `lz_import-0.1.0/lazy_import/lazy_import.py` & `lz_import-0.1.1/lazy_import/lazy_import.py`

 * *Files identical despite different names*

### Comparing `lz_import-0.1.0/pyproject.toml` & `lz_import-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "lz-import"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Ja-sonYun <killa30867@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "lazy_import"}]
 keywords = ["import", "lazy", "circular"]
 homepage = "https://github.com/Ja-sonYun/lazy_import"
 repository = "https://github.com/Ja-sonYun/lazy_import"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-pytest = "^7.3.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.group.lint.dependencies]
```

### Comparing `lz_import-0.1.0/PKG-INFO` & `lz_import-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 Metadata-Version: 2.1
 Name: lz-import
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Home-page: https://github.com/Ja-sonYun/lazy_import
 License: MIT
 Keywords: import,lazy,circular
 Author: Ja-sonYun
 Author-email: killa30867@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Project-URL: Repository, https://github.com/Ja-sonYun/lazy_import
 Description-Content-Type: text/markdown
 
 # Lazy Import
 
+### Installation
+```
+pip install lz-import
+# Or
+poetry add lz-import
+```
+
 ### Usage
 ```python
 # File: company.py
 from user import User
 
 class Company:
     name = "company"
```

