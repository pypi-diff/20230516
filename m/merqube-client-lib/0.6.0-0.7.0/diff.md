# Comparing `tmp/merqube_client_lib-0.6.0.tar.gz` & `tmp/merqube_client_lib-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merqube_client_lib-0.6.0.tar", max compression
+gzip compressed data, was "merqube_client_lib-0.7.0.tar", max compression
```

## Comparing `merqube_client_lib-0.6.0.tar` & `merqube_client_lib-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    11357 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/LICENSE
--rw-r--r--   0        0        0      377 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/api_client/__init__.py
--rw-r--r--   0        0        0     1100 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/api_client/base.py
--rw-r--r--   0        0        0     1361 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/api_client/indexapi.py
--rw-r--r--   0        0        0      767 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/api_client/merqube_client.py
--rw-r--r--   0        0        0      367 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/constants.py
--rw-r--r--   0        0        0      482 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/exceptions.py
--rw-r--r--   0        0        0     1934 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/logging.py
--rw-r--r--   0        0        0     3476 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/mocker.py
--rw-r--r--   0        0        0        0 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/py.typed
--rw-r--r--   0        0        0        0 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/secapi/__init__.py
--rw-r--r--   0        0        0    11729 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/secapi/client.py
--rw-r--r--   0        0        0    11754 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/session.py
--rw-r--r--   0        0        0      414 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/types/__init__.py
--rw-r--r--   0        0        0      418 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/types/secapi.py
--rw-r--r--   0        0        0      677 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/merqube_client_lib/util.py
--rw-r--r--   0        0        0     1713 2023-05-11 20:54:33.507233 merqube_client_lib-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 merqube_client_lib-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5272 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/api_client/__init__.py
+-rw-r--r--   0        0        0     1100 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/api_client/base.py
+-rw-r--r--   0        0        0     2535 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/api_client/indexapi.py
+-rw-r--r--   0        0        0     4706 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/api_client/merqube_client.py
+-rw-r--r--   0        0        0      367 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/constants.py
+-rw-r--r--   0        0        0      482 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/exceptions.py
+-rw-r--r--   0        0        0     1934 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/logging.py
+-rw-r--r--   0        0        0     3476 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/mocker.py
+-rw-r--r--   0        0        0        0 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/py.typed
+-rw-r--r--   0        0        0    71154 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/pydantic_types.py
+-rw-r--r--   0        0        0        0 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/secapi/__init__.py
+-rw-r--r--   0        0        0    11729 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/secapi/client.py
+-rw-r--r--   0        0        0    11754 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/session.py
+-rw-r--r--   0        0        0      414 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/types/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/types/secapi.py
+-rw-r--r--   0        0        0      677 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/util.py
+-rw-r--r--   0        0        0     1799 2023-05-16 10:38:48.084447 merqube_client_lib-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5974 1970-01-01 00:00:00.000000 merqube_client_lib-0.7.0/PKG-INFO
```

### Comparing `merqube_client_lib-0.6.0/LICENSE` & `merqube_client_lib-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.6.0/merqube_client_lib/api_client/base.py` & `merqube_client_lib-0.7.0/merqube_client_lib/api_client/base.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.6.0/merqube_client_lib/api_client/indexapi.py` & `merqube_client_lib-0.7.0/merqube_client_lib/api_client/indexapi.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 Client library for Indexapi
 """
+from typing import cast
+
 from merqube_client_lib.api_client.base import MerqubeApiClientBase
+from merqube_client_lib.pydantic_types import IndexDefinitionPatchPutGet as Index
 from merqube_client_lib.types import Manifest
 
 
 class IndexAPIClient(MerqubeApiClientBase):
     """
-    Indexapi Client
+    Indexapi class that contains methods that deal with multiple indices, creation of indices etc
     """
 
     def get_index_defs(
         self, index_names: str | list[str] | None = None, include_nonprod: bool = False
     ) -> dict[str, Manifest]:
         """
         Get index definitions for specified names, or all permissioned indices as a dictionary with ids as keys and index definitions as values
@@ -34,7 +37,34 @@
 
         names_arg = index_names if isinstance(index_names, str) else ",".join(index_names)
 
         prod_clause = "&type=all" if include_nonprod else ""
         url = f"/index?names={names_arg}{prod_clause}"
         res = self.session.get_collection(url)
         return {i["id"]: i for i in res}
+
+    def create_index(self, index_def: Index) -> dict[str, str]:
+        """
+        Create an index
+        Returns a dictionary containing the id of the index and its related securities (index, intraday_index)
+
+        TODO: examples and index templates to be added to this repo.
+        """
+        return cast(dict[str, str], self.session.post("/index", json=index_def.dict()).json())
+
+    def update_index(self, index_id: str, index_def: Index) -> None:
+        """
+        Update (full object replacement) an index
+        """
+        self.session.put(f"/index/{index_id}", json=index_def.dict())
+
+    def patch_index(self, index_id: str, index_updates: Manifest) -> None:
+        """
+        Patch an index - index_updates is a partial index manifest
+        """
+        self.session.patch(f"/index/{index_id}", json=index_updates)
+
+    def delete_index(self, index_id: str) -> None:
+        """
+        Delete an index
+        """
+        self.session.delete(f"/index/{index_id}")
```

### Comparing `merqube_client_lib-0.6.0/merqube_client_lib/logging.py` & `merqube_client_lib-0.7.0/merqube_client_lib/logging.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.6.0/merqube_client_lib/mocker.py` & `merqube_client_lib-0.7.0/merqube_client_lib/mocker.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.6.0/merqube_client_lib/secapi/client.py` & `merqube_client_lib-0.7.0/merqube_client_lib/secapi/client.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.6.0/merqube_client_lib/session.py` & `merqube_client_lib-0.7.0/merqube_client_lib/session.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.6.0/merqube_client_lib/util.py` & `merqube_client_lib-0.7.0/merqube_client_lib/util.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.6.0/pyproject.toml` & `merqube_client_lib-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "merqube-client-lib"
-version = "0.6.0"
+version = "0.7.0"
 description = "MerQube IndexAPI + SecAPI client library"
 authors = ["Merqube"]
 readme = "README.md"
 license = "APACHE-2.0"
 homepage = "https://github.com/merqube/merqube-client-lib"
 include = [
     "LICENSE",
@@ -47,24 +47,26 @@
 sections = "FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
 
 [tool.mypy]
 ignore_missing_imports = true
 # the pydantic types file is autogenerated and overwritten each time
 exclude = [
     "merqube_client_lib/mocker.py",
+    "merqube_client_lib/pydantic_types.py"
 ]
 
 disable_error_code = [
 ]
 
 [tool.pyright]
 # missing types in 3rd parties:
 reportMissingImports = false
 reportMissingModuleSource = false
 exclude = [
+    "merqube_client_lib/pydantic_types.py"
 ]
 
 # https://mypy.readthedocs.io/en/stable/config_file.html#example-pyproject-toml
 # https://mypy.readthedocs.io/en/stable/running_mypy.html#missing-library-stubs-or-py-typed-marker
 [[tool.mypy.overrides]]
 module = [
      "flask_cors",
```

