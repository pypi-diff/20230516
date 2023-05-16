# Comparing `tmp/pybricks_jedi-1.8.0.tar.gz` & `tmp/pybricks_jedi-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybricks_jedi-1.8.0.tar", max compression
+gzip compressed data, was "pybricks_jedi-1.9.0.tar", max compression
```

## Comparing `pybricks_jedi-1.8.0.tar` & `pybricks_jedi-1.9.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1077 2023-04-21 22:27:39.399066 pybricks_jedi-1.8.0/LICENSE
--rw-r--r--   0        0        0      612 2023-04-21 22:27:39.399066 pybricks_jedi-1.8.0/pyproject.toml
--rw-r--r--   0        0        0    14663 2023-04-21 22:27:39.399066 pybricks_jedi-1.8.0/src/pybricks_jedi/__init__.py
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 pybricks_jedi-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-16 20:44:10.840456 pybricks_jedi-1.9.0/LICENSE
+-rw-r--r--   0        0        0      612 2023-05-16 20:44:10.840456 pybricks_jedi-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    14663 2023-05-16 20:44:10.840456 pybricks_jedi-1.9.0/src/pybricks_jedi/__init__.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 pybricks_jedi-1.9.0/PKG-INFO
```

### Comparing `pybricks_jedi-1.8.0/LICENSE` & `pybricks_jedi-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybricks_jedi-1.8.0/pyproject.toml` & `pybricks_jedi-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "pybricks_jedi"
-version = "1.8.0"
+version = "1.9.0"
 description = "Code completion for Pybricks."
 authors = ["The Pybricks Authors <team@pybricks.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">= 3.10, < 3.12"
-pybricks = "3.3.0a4"
+pybricks = "3.3.0a5"
 jedi = "0.18.1"
 typing-extensions = "4.2.0"
 docstring-parser = "0.14.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 black = "^22.3.0"
```

### Comparing `pybricks_jedi-1.8.0/src/pybricks_jedi/__init__.py` & `pybricks_jedi-1.9.0/src/pybricks_jedi/__init__.py`

 * *Files identical despite different names*

### Comparing `pybricks_jedi-1.8.0/PKG-INFO` & `pybricks_jedi-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pybricks-jedi
-Version: 1.8.0
+Version: 1.9.0
 Summary: Code completion for Pybricks.
 License: MIT
 Author: The Pybricks Authors
 Author-email: team@pybricks.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docstring-parser (==0.14.1)
 Requires-Dist: jedi (==0.18.1)
-Requires-Dist: pybricks (==3.3.0a4)
+Requires-Dist: pybricks (==3.3.0a5)
 Requires-Dist: typing-extensions (==4.2.0)
```

