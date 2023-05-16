# Comparing `tmp/merqube_client_lib-0.7.0.tar.gz` & `tmp/merqube_client_lib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merqube_client_lib-0.7.0.tar", max compression
+gzip compressed data, was "merqube_client_lib-0.8.0.tar", max compression
```

## Comparing `merqube_client_lib-0.7.0.tar` & `merqube_client_lib-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/LICENSE
--rw-r--r--   0        0        0     5272 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/api_client/__init__.py
--rw-r--r--   0        0        0     1100 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/api_client/base.py
--rw-r--r--   0        0        0     2535 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/api_client/indexapi.py
--rw-r--r--   0        0        0     4706 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/api_client/merqube_client.py
--rw-r--r--   0        0        0      367 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/constants.py
--rw-r--r--   0        0        0      482 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/exceptions.py
--rw-r--r--   0        0        0     1934 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/logging.py
--rw-r--r--   0        0        0     3476 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/mocker.py
--rw-r--r--   0        0        0        0 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/py.typed
--rw-r--r--   0        0        0    71154 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/pydantic_types.py
--rw-r--r--   0        0        0        0 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/secapi/__init__.py
--rw-r--r--   0        0        0    11729 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/secapi/client.py
--rw-r--r--   0        0        0    11754 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/session.py
--rw-r--r--   0        0        0      414 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/types/__init__.py
--rw-r--r--   0        0        0      418 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/types/secapi.py
--rw-r--r--   0        0        0      677 2023-05-16 10:38:48.080447 merqube_client_lib-0.7.0/merqube_client_lib/util.py
--rw-r--r--   0        0        0     1799 2023-05-16 10:38:48.084447 merqube_client_lib-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5974 1970-01-01 00:00:00.000000 merqube_client_lib-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/LICENSE
+-rw-r--r--   0        0        0     5272 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/api_client/__init__.py
+-rw-r--r--   0        0        0     1129 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/api_client/base.py
+-rw-r--r--   0        0        0     2535 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/api_client/indexapi.py
+-rw-r--r--   0        0        0     6722 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/api_client/merqube_client.py
+-rw-r--r--   0        0        0    11322 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/api_client/secapi.py
+-rw-r--r--   0        0        0      367 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/constants.py
+-rw-r--r--   0        0        0      482 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/exceptions.py
+-rw-r--r--   0        0        0     1934 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/logging.py
+-rw-r--r--   0        0        0     4170 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/mocker.py
+-rw-r--r--   0        0        0        0 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/py.typed
+-rw-r--r--   0        0        0    71154 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/pydantic_types.py
+-rw-r--r--   0        0        0        0 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/secapi/__init__.py
+-rw-r--r--   0        0        0    11497 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/session.py
+-rw-r--r--   0        0        0      414 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/types/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/types/secapi.py
+-rw-r--r--   0        0        0      677 2023-05-16 20:00:52.711122 merqube_client_lib-0.8.0/merqube_client_lib/util.py
+-rw-r--r--   0        0        0     1829 2023-05-16 20:00:52.715122 merqube_client_lib-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6013 1970-01-01 00:00:00.000000 merqube_client_lib-0.8.0/PKG-INFO
```

### Comparing `merqube_client_lib-0.7.0/LICENSE` & `merqube_client_lib-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.7.0/README.md` & `merqube_client_lib-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.7.0/merqube_client_lib/api_client/base.py` & `merqube_client_lib-0.8.0/merqube_client_lib/api_client/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 Base class for all Merqube API Clients
 """
 from typing import Any, Iterable, Optional
 
-from merqube_client_lib.session import MerqubeAPISession, get_merqube_session
+# import like this so monkeypatch works as expected
+from merqube_client_lib import session
 from merqube_client_lib.types import ManifestList
 
 
 class MerqubeApiClientBase:
     """
     base class that contains validation functions
     """
 
     def __init__(
         self,
-        user_session: Optional[MerqubeAPISession] = None,
+        user_session: Optional[session.MerqubeAPISession] = None,
         token: Optional[str] = None,
         **session_kwargs: Any,
     ):
-        self.session = user_session or get_merqube_session(token=token, **session_kwargs)
+        self.session = user_session or session.get_merqube_session(token=token, **session_kwargs)
 
     def _collection_helper(
         self,
         *,
         url: str,
         query_options: dict[str, str | Iterable[str] | None] | None = None,
     ) -> ManifestList:
```

### Comparing `merqube_client_lib-0.7.0/merqube_client_lib/api_client/indexapi.py` & `merqube_client_lib-0.8.0/merqube_client_lib/api_client/indexapi.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.7.0/merqube_client_lib/logging.py` & `merqube_client_lib-0.8.0/merqube_client_lib/logging.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.7.0/merqube_client_lib/mocker.py` & `merqube_client_lib-0.8.0/merqube_client_lib/mocker.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,42 +61,58 @@
     for function in [get_session_function_path, get_client_function_path]:
         # Checks if all the function exists
         importlib.find_loader(function)
 
     client_function_module_name = get_client_function_path[: get_client_function_path.rindex(".")]
     client_module = importlib.import_module(client_function_module_name)
 
-    def mock_secapi(monkeypatch, method_name_function_map: dict[str, Callable[..., Any]]) -> None:
+    def mock_secapi(
+        monkeypatch,
+        method_name_function_map: dict[str, Callable[..., Any]],
+        session_func_map: dict[str, Callable[..., Any]] | None = None,
+        **get_client_kwargs: Any,
+    ) -> None:
         """
         get a client with some methods patched with swapout functions
         """
         if secapi_client_cache is not None:
             logger.debug("Clearing client cache")
             secapi_client_cache.clear()
         else:
             logger.debug("No client cache to clear")
 
         sess = MagicMock()
-        logger.debug(f"Mocking session at {get_session_function_path}")
-        monkeypatch.setattr(get_session_function_path, MagicMock(return_value=sess))
 
-        client = client_module.get_client()
+        if session_func_map is not None:
+            for method_name, func in session_func_map.items():
+                if getattr(sess, method_name) is None:
+                    raise ValueError(f"Trying to patch a nonexisting session method: {method_name}")
+                logger.debug(f"Mocking session method {method_name}")
+                setattr(sess, method_name, func)
+
+        def get_session(*args: Any, **kwargs: Any):
+            logger.debug("Returning mocked session")
+            return sess
+
+        logger.debug(f"Mocking get_session call at {get_session_function_path}")
+        monkeypatch.setattr(get_session_function_path, get_session)
+
+        client = client_module.get_client(**get_client_kwargs)
 
         if "get_supported_secapi_types" not in method_name_function_map:
             setattr(client, "get_supported_secapi_types", _sec_types)
 
-        # inside
-
         for method_name, func in method_name_function_map.items():
             if getattr(client, method_name) is None:
-                raise ValueError("Trying to patch a function that doesnt exist in the client")
+                raise ValueError(f"Trying to patch a nonexisting client method: {method_name}")
             logger.debug(f"Mocking method {method_name}")
             setattr(client, method_name, func)
 
         def get_client(*args: Any, **kwargs: Any):
+            logger.debug("Returning mocked client")
             return client
 
         # now a get_client call from the main code will return this mocked client:
-        logger.debug(f"Mocking client at {get_client_function_path}")
+        logger.debug(f"Mocking get_client call at {get_client_function_path}")
         monkeypatch.setattr(get_client_function_path, get_client)
 
     return mock_secapi
```

### Comparing `merqube_client_lib-0.7.0/merqube_client_lib/pydantic_types.py` & `merqube_client_lib-0.8.0/merqube_client_lib/pydantic_types.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.7.0/merqube_client_lib/secapi/client.py` & `merqube_client_lib-0.8.0/merqube_client_lib/api_client/secapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 MerqubeAPIClient is a superset of this and the other clients.
 """
 import operator
 from collections import abc
 from typing import Any, Iterable, Optional
 
 import pandas as pd
-from cachetools import LRUCache, TTLCache, cached, cachedmethod
+from cachetools import TTLCache, cachedmethod
 
 from merqube_client_lib.api_client.base import MerqubeApiClientBase
 from merqube_client_lib.constants import DEFAULT_CACHE_TTL
 from merqube_client_lib.session import MerqubeAPISession
 from merqube_client_lib.types.secapi import (
     AddlSecapiOptions,
     MappingTable,
@@ -37,15 +37,15 @@
 
         self.type_cache = TTLCache(1, ttl=DEFAULT_CACHE_TTL)  # type: ignore
 
     def get_supported_secapi_types(self) -> list[dict[str, str]]:
         """
         Get the list of supported security types
         """
-        return self.session.get_collection("/security")
+        return self.session.get_collection(url="/security")
 
     @cachedmethod(operator.attrgetter("type_cache"))
     def _validate_secapi_type(self, sec_type: str) -> None:
         """Validate security_type"""
         assert sec_type in (
             supported_types := [x["name"] for x in self.get_supported_secapi_types()]
         ), f"sec_type must be one of {supported_types}"
@@ -275,20 +275,7 @@
             .groupby(["eff_ts", "id"])
             .last()
             .reset_index()
             .sort_values(["id", "eff_ts"])
             .reset_index()
             .drop("index", axis=1)
         )
-
-
-secapi_client_cache: LRUCache = LRUCache(maxsize=256)  # type: ignore
-
-
-@cached(cache=secapi_client_cache)
-def get_client(
-    user_session: Optional[MerqubeAPISession] = None, token: Optional[str] = None, **session_kwargs: Any
-) -> SecAPIClient:
-    """
-    Cached; returns a secapi client for token
-    """
-    return SecAPIClient(user_session=user_session, token=token, **session_kwargs)
```

### Comparing `merqube_client_lib-0.7.0/merqube_client_lib/session.py` & `merqube_client_lib-0.8.0/merqube_client_lib/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,16 +298,7 @@
 
 @cached(cache=LRUCache(maxsize=256))
 def get_merqube_session(token: str | None = None, **session_args: Any) -> MerqubeAPISession:
     """
     Cached; returns a session with the given token
     """
     return MerqubeAPISession(token=token, **session_args)
-
-
-@cached(cache=LRUCache(maxsize=1))
-def get_public_merqube_session() -> MerqubeAPISession:
-    """
-    Returns a (no token) session.
-    This can be used to access all data in the `default` namespace (world viewable)
-    """
-    return MerqubeAPISession()
```

### Comparing `merqube_client_lib-0.7.0/merqube_client_lib/util.py` & `merqube_client_lib-0.8.0/merqube_client_lib/util.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.7.0/pyproject.toml` & `merqube_client_lib-0.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "merqube-client-lib"
-version = "0.7.0"
+version = "0.8.0"
 description = "MerQube IndexAPI + SecAPI client library"
 authors = ["Merqube"]
 readme = "README.md"
 license = "APACHE-2.0"
 homepage = "https://github.com/merqube/merqube-client-lib"
 include = [
     "LICENSE",
@@ -14,14 +14,15 @@
 python = "^3.10,<4.0"
 requests = "*"
 pydantic = {"version" = "^1.10.5"}
 pandas = "^1.3.0"
 Flask = "~2"
 Flask-Cors = "~3"
 cachetools = "^5.2.0"
+pandas_market_calendars = "*"
 
 [tool.poetry.dev-dependencies]
 coverage =  {version="*"}
 pdbpp = {version="*"}
 pytest = {version="*"}
 pytest-cov =  {version="*"}
 pytest-timeout =  {version="*"}
```

### Comparing `merqube_client_lib-0.7.0/PKG-INFO` & `merqube_client_lib-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: merqube-client-lib
-Version: 0.7.0
+Version: 0.8.0
 Summary: MerQube IndexAPI + SecAPI client library
 Home-page: https://github.com/merqube/merqube-client-lib
 License: Apache-2.0
 Author: Merqube
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Flask (>=2,<3)
 Requires-Dist: Flask-Cors (>=3,<4)
 Requires-Dist: cachetools (>=5.2.0,<6.0.0)
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
+Requires-Dist: pandas_market_calendars
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # merqube-client-lib
 MerQube API Client Library (Python)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/merqube/merqube-client-lib/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/merqube/merqube-client-lib/tree/main)
```

