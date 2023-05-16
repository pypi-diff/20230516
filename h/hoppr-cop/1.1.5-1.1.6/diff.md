# Comparing `tmp/hoppr_cop-1.1.5.tar.gz` & `tmp/hoppr_cop-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr_cop-1.1.5.tar", max compression
+gzip compressed data, was "hoppr_cop-1.1.6.tar", max compression
```

## Comparing `hoppr_cop-1.1.5.tar` & `hoppr_cop-1.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1084 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/LICENSE.md
--rw-r--r--   0        0        0       55 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/combined/__init__.py
--rw-r--r--   0        0        0     3336 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/combined/cli.py
--rw-r--r--   0        0        0     4488 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/combined/combined_scanner.py
--rw-r--r--   0        0        0        0 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/gemnasium/__init__.py
--rw-r--r--   0        0        0     9223 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/gemnasium/gemnasium_scanner.py
--rw-r--r--   0        0        0     1134 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/gemnasium/models.py
--rwxr-xr-x   0        0        0      113 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/gemnasium/semver
--rw-r--r--   0        0        0        0 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/grype/__init__.py
--rw-r--r--   0        0        0     5953 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/grype/grype_scanner.py
--rw-r--r--   0        0        0     5289 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/grype/models.py
--rw-r--r--   0        0        0     9731 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/hoppr_plugin/hopprcop_plugin.py
--rw-r--r--   0        0        0      478 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/README.md
--rw-r--r--   0        0        0        0 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/__init__.py
--rw-r--r--   0        0        0      832 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/api/__init__.py
--rw-r--r--   0        0        0     1029 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/api/exception.py
--rw-r--r--   0        0        0     9487 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/api/model.py
--rw-r--r--   0        0        0    11624 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/api/ossindex.py
--rw-r--r--   0        0        0      153 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/api/py.typed
--rw-r--r--   0        0        0     3147 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/api/serializer.py
--rw-r--r--   0        0        0     4924 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/oss_index_scanner.py
--rw-r--r--   0        0        0        0 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/trivy/__init__.py
--rw-r--r--   0        0        0     5558 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/trivy/trivy_scanner.py
--rw-r--r--   0        0        0      853 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 hoppr_cop-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/LICENSE.md
+-rw-r--r--   0        0        0       55 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/combined/__init__.py
+-rw-r--r--   0        0        0     3336 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/combined/cli.py
+-rw-r--r--   0        0        0     4488 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/combined/combined_scanner.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/gemnasium/__init__.py
+-rw-r--r--   0        0        0     9223 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/gemnasium/gemnasium_scanner.py
+-rw-r--r--   0        0        0     1134 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/gemnasium/models.py
+-rwxr-xr-x   0        0        0      113 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/gemnasium/semver
+-rw-r--r--   0        0        0        0 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/grype/__init__.py
+-rw-r--r--   0        0        0     5953 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/grype/grype_scanner.py
+-rw-r--r--   0        0        0     5289 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/grype/models.py
+-rw-r--r--   0        0        0     9731 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/hoppr_plugin/hopprcop_plugin.py
+-rw-r--r--   0        0        0      478 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/__init__.py
+-rw-r--r--   0        0        0      832 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/api/__init__.py
+-rw-r--r--   0        0        0     1029 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/api/exception.py
+-rw-r--r--   0        0        0     9487 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/api/model.py
+-rw-r--r--   0        0        0    11624 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/api/ossindex.py
+-rw-r--r--   0        0        0      153 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/api/py.typed
+-rw-r--r--   0        0        0     3147 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/api/serializer.py
+-rw-r--r--   0        0        0     4924 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/ossindex/oss_index_scanner.py
+-rw-r--r--   0        0        0        0 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/trivy/__init__.py
+-rw-r--r--   0        0        0     5558 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/hopprcop/trivy/trivy_scanner.py
+-rw-r--r--   0        0        0      853 2023-05-16 18:09:34.000000 hoppr_cop-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 hoppr_cop-1.1.6/PKG-INFO
```

### Comparing `hoppr_cop-1.1.5/LICENSE.md` & `hoppr_cop-1.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.5/hopprcop/combined/cli.py` & `hoppr_cop-1.1.6/hopprcop/combined/cli.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.5/hopprcop/combined/combined_scanner.py` & `hoppr_cop-1.1.6/hopprcop/combined/combined_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.5/hopprcop/gemnasium/gemnasium_scanner.py` & `hoppr_cop-1.1.6/hopprcop/gemnasium/gemnasium_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.5/hopprcop/gemnasium/models.py` & `hoppr_cop-1.1.6/hopprcop/gemnasium/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.5/hopprcop/grype/grype_scanner.py` & `hoppr_cop-1.1.6/hopprcop/grype/grype_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.5/hopprcop/grype/models.py` & `hoppr_cop-1.1.6/hopprcop/grype/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.5/hopprcop/hoppr_plugin/hopprcop_plugin.py` & `hoppr_cop-1.1.6/hopprcop/hoppr_plugin/hopprcop_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.5/hopprcop/ossindex/api/__init__.py` & `hoppr_cop-1.1.6/hopprcop/ossindex/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.5/hopprcop/ossindex/api/exception.py` & `hoppr_cop-1.1.6/hopprcop/ossindex/api/exception.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.5/hopprcop/ossindex/api/model.py` & `hoppr_cop-1.1.6/hopprcop/ossindex/api/model.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.5/hopprcop/ossindex/api/ossindex.py` & `hoppr_cop-1.1.6/hopprcop/ossindex/api/ossindex.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.5/hopprcop/ossindex/api/serializer.py` & `hoppr_cop-1.1.6/hopprcop/ossindex/api/serializer.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.5/hopprcop/ossindex/oss_index_scanner.py` & `hoppr_cop-1.1.6/hopprcop/ossindex/oss_index_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.5/hopprcop/trivy/trivy_scanner.py` & `hoppr_cop-1.1.6/hopprcop/trivy/trivy_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.5/pyproject.toml` & `hoppr_cop-1.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr-cop"
-version = "1.1.5"
+version = "1.1.6"
 description = ""
 authors = ["kganger <keith.e.ganger@lmco.com>"]
 license = "MIT"
 
 [[tool.poetry.packages]]
 include = "hopprcop"
 
@@ -17,15 +17,15 @@
 packageurl-python = "^0.10.1"
 tabulate = "^0.9.0"
 tinydb = "^4.7.0"
 rich = ">12.5.1"
 mkdocs = "^1.3.1"
 mkdocs-mermaid2-plugin = "^0.6.0"
 hoppr = "^1.8.0"
-pytest = "7.3.0"
+pytest = "7.3.1"
 coverage = "^7.0.0"
 hoppr-security-commons = "^0.0.13"
 mkdocs-glightbox = "^0.3.1"
 pygments = "^2.14.0"
 pymdown-extensions = "^9.9.2"
 
 [tool.poetry.scripts]
```

### Comparing `hoppr_cop-1.1.5/PKG-INFO` & `hoppr_cop-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr-cop
-Version: 1.1.5
+Version: 1.1.6
 Summary: 
 License: MIT
 Author: kganger
 Author-email: keith.e.ganger@lmco.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,12 +18,12 @@
 Requires-Dist: hoppr-security-commons (>=0.0.13,<0.0.14)
 Requires-Dist: mkdocs (>=1.3.1,<2.0.0)
 Requires-Dist: mkdocs-glightbox (>=0.3.1,<0.4.0)
 Requires-Dist: mkdocs-mermaid2-plugin (>=0.6.0,<0.7.0)
 Requires-Dist: packageurl-python (>=0.10.1,<0.11.0)
 Requires-Dist: pygments (>=2.14.0,<3.0.0)
 Requires-Dist: pymdown-extensions (>=9.9.2,<10.0.0)
-Requires-Dist: pytest (==7.3.0)
+Requires-Dist: pytest (==7.3.1)
 Requires-Dist: rich (>12.5.1)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tinydb (>=4.7.0,<5.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
```

