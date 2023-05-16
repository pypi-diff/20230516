# Comparing `tmp/flask-httpx-request-converted-to-flask-test-client-request-0.1.2.tar.gz` & `tmp/flask-httpx-request-converted-to-flask-test-client-request-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-httpx-request-converted-to-flask-test-client-request-0.1.2.tar", last modified: Thu Jun 30 07:33:16 2022, max compression
+gzip compressed data, was "flask-httpx-request-converted-to-flask-test-client-request-0.1.4.tar", last modified: Tue May 16 12:07:04 2023, max compression
```

## Comparing `flask-httpx-request-converted-to-flask-test-client-request-0.1.2.tar` & `flask-httpx-request-converted-to-flask-test-client-request-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dvv       (1101) staff       (20)        0 2022-06-30 07:33:16.498321 flask-httpx-request-converted-to-flask-test-client-request-0.1.2/
--rw-r--r--   0 dvv       (1101) staff       (20)      665 2022-06-01 11:29:09.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.2/LICENSE
--rw-r--r--   0 dvv       (1101) staff       (20)     3642 2022-06-30 07:33:16.498200 flask-httpx-request-converted-to-flask-test-client-request-0.1.2/PKG-INFO
--rw-r--r--   0 dvv       (1101) staff       (20)     2946 2022-06-30 07:30:30.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.2/README.md
-drwxr-xr-x   0 dvv       (1101) staff       (20)        0 2022-06-30 07:33:16.497394 flask-httpx-request-converted-to-flask-test-client-request-0.1.2/flask_httpx_request_converted_to_flask_test_client_request/
--rw-r--r--   0 dvv       (1101) staff       (20)     2608 2022-06-30 07:27:15.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.2/flask_httpx_request_converted_to_flask_test_client_request/__init__.py
-drwxr-xr-x   0 dvv       (1101) staff       (20)        0 2022-06-30 07:33:16.498026 flask-httpx-request-converted-to-flask-test-client-request-0.1.2/flask_httpx_request_converted_to_flask_test_client_request.egg-info/
--rw-r--r--   0 dvv       (1101) staff       (20)     3642 2022-06-30 07:33:16.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.2/flask_httpx_request_converted_to_flask_test_client_request.egg-info/PKG-INFO
--rw-r--r--   0 dvv       (1101) staff       (20)      440 2022-06-30 07:33:16.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.2/flask_httpx_request_converted_to_flask_test_client_request.egg-info/SOURCES.txt
--rw-r--r--   0 dvv       (1101) staff       (20)        1 2022-06-30 07:33:16.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.2/flask_httpx_request_converted_to_flask_test_client_request.egg-info/dependency_links.txt
--rw-r--r--   0 dvv       (1101) staff       (20)       59 2022-06-30 07:33:16.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.2/flask_httpx_request_converted_to_flask_test_client_request.egg-info/top_level.txt
--rw-r--r--   0 dvv       (1101) staff       (20)      110 2022-06-01 11:29:43.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.2/pyproject.toml
--rw-r--r--   0 dvv       (1101) staff       (20)       38 2022-06-30 07:33:16.498365 flask-httpx-request-converted-to-flask-test-client-request-0.1.2/setup.cfg
--rw-r--r--   0 dvv       (1101) staff       (20)     1125 2022-06-01 13:21:13.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:07:04.979305 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-16 12:06:52.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-16 12:07:04.979305 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-16 12:06:52.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:07:04.979305 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request/
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-16 12:06:52.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:07:04.979305 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-16 12:07:04.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-16 12:07:04.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:07:04.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 12:07:04.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-16 12:06:52.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:07:04.979305 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-16 12:06:52.000000 flask-httpx-request-converted-to-flask-test-client-request-0.1.4/setup.py
```

### Comparing `flask-httpx-request-converted-to-flask-test-client-request-0.1.2/LICENSE` & `flask-httpx-request-converted-to-flask-test-client-request-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-httpx-request-converted-to-flask-test-client-request-0.1.2/PKG-INFO` & `flask-httpx-request-converted-to-flask-test-client-request-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-httpx-request-converted-to-flask-test-client-request
-Version: 0.1.2
+Version: 0.1.4
 Summary: Unittest Tool: This is a `flask.test_client_class` I wrote to making the libraries created by `openapi-python-client` work with `flask.test_client()`
 Home-page: https://github.com/dvaerum/flask-httpx-request-converted-to-flask-test-client-requests
 Author: Dennis Vestergaard Værum
 Author-email: convert_httpx_2_flask_test_client@varum.dk
 License: 0BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flask-httpx-request-converted-to-flask-test-client-request-0.1.2/README.md` & `flask-httpx-request-converted-to-flask-test-client-request-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `flask-httpx-request-converted-to-flask-test-client-request-0.1.2/flask_httpx_request_converted_to_flask_test_client_request/__init__.py` & `flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-__version__ = "0.1.2"
+__version__ = "0.1.4"
 
 import json
-from typing import Any, Dict
+from typing import Any, Dict, TYPE_CHECKING
 from unittest.mock import patch
 
-from flask.testing import FlaskClient
 from urllib3.util import parse_url
+from flask.testing import FlaskClient
 from werkzeug.test import TestResponse
 
 
 class ConvertHttpx2FlaskTestClient(FlaskClient):
     def __init__(self, *args: Any,
                  base_url: str = "http://localhost",
                  headers: Dict[str, str] = None,
                  cookies: Dict[str, Any] = None,
                  timeout: float = 10.0,
                  verify_ssl: bool = True,
+                 follow_redirects: bool = False,
                  **kwargs: Any):
         self.base_url = base_url
         self._headers = headers if headers else {}
         self._cookies = cookies if cookies else {}
         self._timeout = timeout
         self.verify_ssl = verify_ssl
+        self.follow_redirects = follow_redirects
 
         self.mock_httpx_request = patch("httpx.Client.request",
                                         side_effect=self._convert_httpx_request_2_flask_client_open)
 
         super().__init__(*args, **kwargs)
 
     def get_headers(self):
@@ -38,41 +40,44 @@
         kwargs.pop("content")
         kwargs.pop("files")
         kwargs.pop("params")
         try:
             resp = self.open(*args, **kwargs)
         except Exception as err:
             resp = TestResponse(
-                response=json.dumps({"error_type": str(err.__class__), "args": err.args}).encode(),
+                response=json.dumps({"error_type": str(err.__class__),
+                                     "args": err.args}).encode(),
                 status="500",
                 headers={"Content-Type": "application/json"},
                 request=None)
         resp.content = resp.data
 
-        # Make `resp.json` return the method resp.get_json, instead of the result resp.get_json()
+        # Make `resp.json` return the method resp.get_json,
+        # instead of the result resp.get_json()
         resp._get_json = resp.get_json
         resp.get_json = lambda: resp._get_json
 
         return resp
 
     def get_cookies(self):
         return self._cookies
 
     def get_timeout(self):
         return self._timeout
 
-    def __enter__(self) -> "FlaskClient":
+    def __enter__(self) -> FlaskClient:
         self.mock_httpx_request.start()
         return super().__enter__()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.mock_httpx_request.stop()
         return super().__exit__(exc_type, exc_val, exc_tb)
 
 
 class ConvertHttpx2FlaskTestClientWithoutEnterAndExit(ConvertHttpx2FlaskTestClient):
     def __init__(self, *args, **kwargs):
-        super(ConvertHttpx2FlaskTestClientWithoutEnterAndExit, self).__init__(*args, **kwargs)
+        super(ConvertHttpx2FlaskTestClientWithoutEnterAndExit,
+              self).__init__(*args, **kwargs)
         self.mock_httpx_request.start()
 
     def __del__(self):
         self.mock_httpx_request.stop()
```

### Comparing `flask-httpx-request-converted-to-flask-test-client-request-0.1.2/flask_httpx_request_converted_to_flask_test_client_request.egg-info/PKG-INFO` & `flask-httpx-request-converted-to-flask-test-client-request-0.1.4/flask_httpx_request_converted_to_flask_test_client_request.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-httpx-request-converted-to-flask-test-client-request
-Version: 0.1.2
+Version: 0.1.4
 Summary: Unittest Tool: This is a `flask.test_client_class` I wrote to making the libraries created by `openapi-python-client` work with `flask.test_client()`
 Home-page: https://github.com/dvaerum/flask-httpx-request-converted-to-flask-test-client-requests
 Author: Dennis Vestergaard Værum
 Author-email: convert_httpx_2_flask_test_client@varum.dk
 License: 0BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flask-httpx-request-converted-to-flask-test-client-request-0.1.2/setup.py` & `flask-httpx-request-converted-to-flask-test-client-request-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 setuptools.setup(
     name="flask-httpx-request-converted-to-flask-test-client-request",
     version=flask_httpx_request_converted_to_flask_test_client_request.__version__,
     author="Dennis Vestergaard Værum",
     author_email="convert_httpx_2_flask_test_client@varum.dk",
     license="0BSD",
-    description="Unittest Tool: This is a `flask.test_client_class` I wrote to making the libraries created by "
+    description="Unittest Tool: This is a `flask.test_client_class` "
+                "I wrote to making the libraries created by "
                 "`openapi-python-client` work with `flask.test_client()`",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dvaerum/flask-httpx-request-converted-to-flask-test-client-requests",
     packages=["flask_httpx_request_converted_to_flask_test_client_request"],
     install_requires=[],
     classifiers=[
```

