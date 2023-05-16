# Comparing `tmp/dh_facebook_client-0.2.2.tar.gz` & `tmp/dh_facebook_client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dh_facebook_client-0.2.2.tar", max compression
+gzip compressed data, was "dh_facebook_client-0.2.3.tar", max compression
```

## Comparing `dh_facebook_client-0.2.2.tar` & `dh_facebook_client-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1086 2023-05-03 19:25:20.013300 dh_facebook_client-0.2.2/dh_facebook_client/__init__.py
--rw-r--r--   0        0        0    11071 2023-05-03 19:25:20.013488 dh_facebook_client-0.2.2/dh_facebook_client/client.py
--rw-r--r--   0        0        0      260 2023-05-04 15:33:07.172663 dh_facebook_client-0.2.2/dh_facebook_client/constants.py
--rw-r--r--   0        0        0     5353 2023-05-03 19:25:20.013782 dh_facebook_client-0.2.2/dh_facebook_client/dataclasses.py
--rw-r--r--   0        0        0      521 2023-05-03 19:25:20.013909 dh_facebook_client-0.2.2/dh_facebook_client/error_code.py
--rw-r--r--   0        0        0     4502 2023-05-03 19:25:20.014061 dh_facebook_client-0.2.2/dh_facebook_client/exceptions.py
--rw-r--r--   0        0        0     2903 2023-05-08 15:18:15.116678 dh_facebook_client-0.2.2/dh_facebook_client/helpers.py
--rw-r--r--   0        0        0     1049 2023-05-03 19:25:20.014307 dh_facebook_client-0.2.2/dh_facebook_client/page_client.py
--rw-r--r--   0        0        0      435 2023-05-03 19:25:20.014436 dh_facebook_client-0.2.2/dh_facebook_client/typings.py
--rw-r--r--   0        0        0     1894 2023-05-03 19:25:20.014566 dh_facebook_client-0.2.2/dh_facebook_client/user_client.py
--rw-r--r--   0        0        0      651 2023-05-08 15:18:15.117219 dh_facebook_client-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 dh_facebook_client-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-05-03 19:25:20.013300 dh_facebook_client-0.2.3/dh_facebook_client/__init__.py
+-rw-r--r--   0        0        0    11318 2023-05-16 18:34:00.341106 dh_facebook_client-0.2.3/dh_facebook_client/client.py
+-rw-r--r--   0        0        0      260 2023-05-04 15:33:07.172663 dh_facebook_client-0.2.3/dh_facebook_client/constants.py
+-rw-r--r--   0        0        0     5353 2023-05-03 19:25:20.013782 dh_facebook_client-0.2.3/dh_facebook_client/dataclasses.py
+-rw-r--r--   0        0        0      521 2023-05-03 19:25:20.013909 dh_facebook_client-0.2.3/dh_facebook_client/error_code.py
+-rw-r--r--   0        0        0     4568 2023-05-16 18:34:00.341547 dh_facebook_client-0.2.3/dh_facebook_client/exceptions.py
+-rw-r--r--   0        0        0     2903 2023-05-16 16:07:13.207975 dh_facebook_client-0.2.3/dh_facebook_client/helpers.py
+-rw-r--r--   0        0        0     1049 2023-05-03 19:25:20.014307 dh_facebook_client-0.2.3/dh_facebook_client/page_client.py
+-rw-r--r--   0        0        0      435 2023-05-03 19:25:20.014436 dh_facebook_client-0.2.3/dh_facebook_client/typings.py
+-rw-r--r--   0        0        0     1894 2023-05-03 19:25:20.014566 dh_facebook_client-0.2.3/dh_facebook_client/user_client.py
+-rw-r--r--   0        0        0      651 2023-05-16 18:34:00.342043 dh_facebook_client-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 dh_facebook_client-0.2.3/PKG-INFO
```

### Comparing `dh_facebook_client-0.2.2/dh_facebook_client/__init__.py` & `dh_facebook_client-0.2.3/dh_facebook_client/__init__.py`

 * *Files identical despite different names*

### Comparing `dh_facebook_client-0.2.2/dh_facebook_client/client.py` & `dh_facebook_client-0.2.3/dh_facebook_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import logging
-from typing import Any, Final, Iterator, Optional, cast
+from types import TracebackType
+from typing import Any, Final, Iterator, Optional, Type, cast
 
 import backoff
 from requests import Response, Session
 
 from .constants import GRAPH_API_URL, GRAPH_API_VERSIONS
 from .dataclasses import AppUsageDetails, GraphAPIResponse, TokenDebugPayload
 from .error_code import GraphAPICommonErrorCode
@@ -275,7 +276,15 @@
             items = cast(list[JSONTypeSimple], result.data)
             for i in items:
                 yield i
 
             if not result.after_cursor:
                 break
             params['after'] = result.after_cursor
+
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc: Optional[BaseException],
+        traceback: Optional[TracebackType],
+    ) -> None:
+        self._session.close()
```

### Comparing `dh_facebook_client-0.2.2/dh_facebook_client/dataclasses.py` & `dh_facebook_client-0.2.3/dh_facebook_client/dataclasses.py`

 * *Files identical despite different names*

### Comparing `dh_facebook_client-0.2.2/dh_facebook_client/error_code.py` & `dh_facebook_client-0.2.3/dh_facebook_client/error_code.py`

 * *Files identical despite different names*

### Comparing `dh_facebook_client-0.2.2/dh_facebook_client/exceptions.py` & `dh_facebook_client-0.2.3/dh_facebook_client/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         """
         Scrapes Graph API error body and HTTP response
         :param response: An instance of requests.Response encapsulating the graph API call
         :param error_details: Parsed error details / body from Graph API,
             this is done ahead of time in Client
         :param params_to_mask: A list of additional query params to mask in error messages
         """
+        super().__init__(response, error_details, params_to_mask)
         self.status_code = response.status_code
         self.reason = response.reason
         self.fb_error_msg = error_details.get('message', GraphAPIError.DETAIL_NOT_FOUND_PLACEHOLDER)
         self.type = error_details.get('type', GraphAPIError.DETAIL_NOT_FOUND_PLACEHOLDER)
         self.code = error_details.get('code', GraphAPIError.DETAIL_NOT_FOUND_PLACEHOLDER)
         self.subcode = error_details.get(
             'error_subcode', GraphAPIError.DETAIL_NOT_FOUND_PLACEHOLDER
```

### Comparing `dh_facebook_client-0.2.2/dh_facebook_client/helpers.py` & `dh_facebook_client-0.2.3/dh_facebook_client/helpers.py`

 * *Files identical despite different names*

### Comparing `dh_facebook_client-0.2.2/dh_facebook_client/page_client.py` & `dh_facebook_client-0.2.3/dh_facebook_client/page_client.py`

 * *Files identical despite different names*

### Comparing `dh_facebook_client-0.2.2/dh_facebook_client/user_client.py` & `dh_facebook_client-0.2.3/dh_facebook_client/user_client.py`

 * *Files identical despite different names*

### Comparing `dh_facebook_client-0.2.2/pyproject.toml` & `dh_facebook_client-0.2.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dh-facebook-client"
-version = "0.2.2"
+version = "0.2.3"
 description = "Simple client for interacting with the Facebook Graph API"
 authors = ["pchisholm <chisholm.p@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.26.0"
 backoff = "^1.11.1"
```

