# Comparing `tmp/qdrant_haystack-1.0.0.tar.gz` & `tmp/qdrant_haystack-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_haystack-1.0.0.tar", max compression
+gzip compressed data, was "qdrant_haystack-1.0.1.tar", max compression
```

## Comparing `qdrant_haystack-1.0.0.tar` & `qdrant_haystack-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-04-14 09:42:32.838009 qdrant_haystack-1.0.0/LICENSE
--rw-r--r--   0        0        0     3160 2023-04-14 09:42:32.838009 qdrant_haystack-1.0.0/README.md
--rw-r--r--   0        0        0      746 2023-04-14 09:42:32.842009 qdrant_haystack-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      100 2023-04-14 09:42:32.842009 qdrant_haystack-1.0.0/src/qdrant_haystack/__init__.py
--rw-r--r--   0        0        0      107 2023-04-14 09:42:32.842009 qdrant_haystack-1.0.0/src/qdrant_haystack/document_stores/__init__.py
--rw-r--r--   0        0        0     2285 2023-04-14 09:42:32.842009 qdrant_haystack-1.0.0/src/qdrant_haystack/document_stores/converters.py
--rw-r--r--   0        0        0     8295 2023-04-14 09:42:32.842009 qdrant_haystack-1.0.0/src/qdrant_haystack/document_stores/filters.py
--rw-r--r--   0        0        0    20253 2023-04-14 09:42:32.842009 qdrant_haystack-1.0.0/src/qdrant_haystack/document_stores/qdrant.py
--rw-r--r--   0        0        0        0 2023-04-14 09:42:32.842009 qdrant_haystack-1.0.0/src/qdrant_haystack/utils.py
--rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 qdrant_haystack-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 14:42:23.052573 qdrant_haystack-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3160 2023-05-16 14:42:23.052573 qdrant_haystack-1.0.1/README.md
+-rw-r--r--   0        0        0      764 2023-05-16 14:42:23.052573 qdrant_haystack-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-05-16 14:42:23.052573 qdrant_haystack-1.0.1/src/qdrant_haystack/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-16 14:42:23.052573 qdrant_haystack-1.0.1/src/qdrant_haystack/document_stores/__init__.py
+-rw-r--r--   0        0        0     2285 2023-05-16 14:42:23.052573 qdrant_haystack-1.0.1/src/qdrant_haystack/document_stores/converters.py
+-rw-r--r--   0        0        0     8295 2023-05-16 14:42:23.052573 qdrant_haystack-1.0.1/src/qdrant_haystack/document_stores/filters.py
+-rw-r--r--   0        0        0    20288 2023-05-16 14:42:23.052573 qdrant_haystack-1.0.1/src/qdrant_haystack/document_stores/qdrant.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:42:23.052573 qdrant_haystack-1.0.1/src/qdrant_haystack/utils.py
+-rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 qdrant_haystack-1.0.1/PKG-INFO
```

### Comparing `qdrant_haystack-1.0.0/LICENSE` & `qdrant_haystack-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.0/README.md` & `qdrant_haystack-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.0/pyproject.toml` & `qdrant_haystack-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "qdrant-haystack"
-version = "1.0.0"
+version = "1.0.1"
 description = "An integration of Qdrant ANN vector database backend with Haystack"
 authors = ["Kacper Łukawski <kacper.lukawski@qdrant.com>"]
 packages = [
     {include = "qdrant_haystack", from = "src"}
 ]
 readme = "README.md"
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<=3.11"
 qdrant-client = "^1.1.4"
 farm-haystack = "^1.13.0"
+torch = "<=2.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
 pre-commit = "^3.1.0"
 black = "^23.1.0"
 isort = "^5.12.0"
 mypy = "^1.0.1"
```

### Comparing `qdrant_haystack-1.0.0/src/qdrant_haystack/document_stores/converters.py` & `qdrant_haystack-1.0.1/src/qdrant_haystack/document_stores/converters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.0/src/qdrant_haystack/document_stores/filters.py` & `qdrant_haystack-1.0.1/src/qdrant_haystack/document_stores/filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.0/src/qdrant_haystack/document_stores/qdrant.py` & `qdrant_haystack-1.0.1/src/qdrant_haystack/document_stores/qdrant.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,14 +387,15 @@
                 )
 
                 progress_bar.update(batch_size)
 
     def update_document_meta(
         self, id: str, meta: Dict[str, Any], index: Optional[str] = None
     ):
+        index = index or self.inde
         document = self.get_document_by_id(id, index)
         if document is None:
             logger.warning(
                 "Requested to update document meta for non-existing id %s", id
             )
             return
```

### Comparing `qdrant_haystack-1.0.0/PKG-INFO` & `qdrant_haystack-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: qdrant-haystack
-Version: 1.0.0
+Version: 1.0.1
 Summary: An integration of Qdrant ANN vector database backend with Haystack
 License: Apache 2.0
 Author: Kacper Łukawski
 Author-email: kacper.lukawski@qdrant.com
 Requires-Python: >=3.8.1,<=3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: farm-haystack (>=1.13.0,<2.0.0)
 Requires-Dist: qdrant-client (>=1.1.4,<2.0.0)
+Requires-Dist: torch (<=2.0.0)
 Description-Content-Type: text/markdown
 
 # qdrant-haystack
 
 An integration of [Qdrant](https://qdrant.tech) vector database with [Haystack](https://haystack.deepset.ai/)
 by [deepset](https://www.deepset.ai).
```

