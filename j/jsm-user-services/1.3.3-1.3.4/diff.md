# Comparing `tmp/jsm_user_services-1.3.3.tar.gz` & `tmp/jsm_user_services-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsm_user_services-1.3.3.tar", max compression
+gzip compressed data, was "jsm_user_services-1.3.4.tar", max compression
```

## Comparing `jsm_user_services-1.3.3.tar` & `jsm_user_services-1.3.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1070 2023-04-20 13:29:37.852234 jsm_user_services-1.3.3/LICENSE
--rw-r--r--   0        0        0    10306 2023-04-20 13:29:37.852234 jsm_user_services-1.3.3/README.md
--rw-r--r--   0        0        0       54 2023-04-20 13:29:37.852234 jsm_user_services-1.3.3/jsm_user_services/__init__.py
--rw-r--r--   0        0        0      107 2023-04-20 13:29:37.852234 jsm_user_services-1.3.3/jsm_user_services/apps.py
--rw-r--r--   0        0        0        0 2023-04-20 13:29:37.852234 jsm_user_services-1.3.3/jsm_user_services/decorators/__init__.py
--rw-r--r--   0        0        0     3795 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/decorators/lgpd.py
--rw-r--r--   0        0        0     5933 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/decorators/lgpd_utils.py
--rw-r--r--   0        0        0        0 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/drf_tools/__init__.py
--rw-r--r--   0        0        0     2475 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/drf_tools/helpers.py
--rw-r--r--   0        0        0    14221 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/drf_tools/permissions.py
--rw-r--r--   0        0        0      692 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/exception.py
--rw-r--r--   0        0        0        0 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/flask/__init__.py
--rw-r--r--   0        0        0     3462 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/flask/middleware.py
--rw-r--r--   0        0        0     3167 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/middleware.py
--rw-r--r--   0        0        0        0 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/services/__init__.py
--rw-r--r--   0        0        0     4258 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/services/everest.py
--rw-r--r--   0        0        0     1996 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/services/google.py
--rw-r--r--   0        0        0     4657 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/services/user.py
--rw-r--r--   0        0        0     1840 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/settings.py
--rw-r--r--   0        0        0        0 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/__init__.py
--rw-r--r--   0        0        0     1007 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/auth_jwt.py
--rw-r--r--   0        0        0      866 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/email_utils.py
--rw-r--r--   0        0        0     2333 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/http_utils.py
--rw-r--r--   0        0        0      304 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/import_utils.py
--rw-r--r--   0        0        0      419 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/local_threading_utils.py
--rw-r--r--   0        0        0      268 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/logging_utils.py
--rw-r--r--   0        0        0     1971 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/request_id.py
--rw-r--r--   0        0        0      618 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/settings_utils.py
--rw-r--r--   0        0        0      237 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/jsm_user_services/support/string_utils.py
--rw-r--r--   0        0        0     1572 2023-04-20 13:29:37.864234 jsm_user_services-1.3.3/pyproject.toml
--rw-r--r--   0        0        0    11435 1970-01-01 00:00:00.000000 jsm_user_services-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/LICENSE
+-rw-r--r--   0        0        0    10306 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/README.md
+-rw-r--r--   0        0        0       54 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/apps.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/decorators/__init__.py
+-rw-r--r--   0        0        0     3795 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/decorators/lgpd.py
+-rw-r--r--   0        0        0     5933 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/decorators/lgpd_utils.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/drf_tools/__init__.py
+-rw-r--r--   0        0        0     2475 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/drf_tools/helpers.py
+-rw-r--r--   0        0        0    14221 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/drf_tools/permissions.py
+-rw-r--r--   0        0        0      692 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/exception.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/flask/__init__.py
+-rw-r--r--   0        0        0     3462 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/flask/middleware.py
+-rw-r--r--   0        0        0     3167 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/services/__init__.py
+-rw-r--r--   0        0        0     4258 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/services/everest.py
+-rw-r--r--   0        0        0     1996 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/services/google.py
+-rw-r--r--   0        0        0     4657 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/services/user.py
+-rw-r--r--   0        0        0     1840 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/settings.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/__init__.py
+-rw-r--r--   0        0        0     1007 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/auth_jwt.py
+-rw-r--r--   0        0        0      866 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/email_utils.py
+-rw-r--r--   0        0        0     2333 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/http_utils.py
+-rw-r--r--   0        0        0      304 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/import_utils.py
+-rw-r--r--   0        0        0      419 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/local_threading_utils.py
+-rw-r--r--   0        0        0      268 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/logging_utils.py
+-rw-r--r--   0        0        0     2185 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/request_id.py
+-rw-r--r--   0        0        0      618 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/settings_utils.py
+-rw-r--r--   0        0        0      237 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/jsm_user_services/support/string_utils.py
+-rw-r--r--   0        0        0     1572 2023-05-16 17:51:50.854743 jsm_user_services-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0    11435 1970-01-01 00:00:00.000000 jsm_user_services-1.3.4/PKG-INFO
```

### Comparing `jsm_user_services-1.3.3/LICENSE` & `jsm_user_services-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/README.md` & `jsm_user_services-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/jsm_user_services/decorators/lgpd.py` & `jsm_user_services-1.3.4/jsm_user_services/decorators/lgpd.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/jsm_user_services/decorators/lgpd_utils.py` & `jsm_user_services-1.3.4/jsm_user_services/decorators/lgpd_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/jsm_user_services/drf_tools/helpers.py` & `jsm_user_services-1.3.4/jsm_user_services/drf_tools/helpers.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/jsm_user_services/drf_tools/permissions.py` & `jsm_user_services-1.3.4/jsm_user_services/drf_tools/permissions.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/jsm_user_services/exception.py` & `jsm_user_services-1.3.4/jsm_user_services/exception.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/jsm_user_services/flask/middleware.py` & `jsm_user_services-1.3.4/jsm_user_services/flask/middleware.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/jsm_user_services/middleware.py` & `jsm_user_services-1.3.4/jsm_user_services/middleware.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/jsm_user_services/services/everest.py` & `jsm_user_services-1.3.4/jsm_user_services/services/everest.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/jsm_user_services/services/google.py` & `jsm_user_services-1.3.4/jsm_user_services/services/google.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/jsm_user_services/services/user.py` & `jsm_user_services-1.3.4/jsm_user_services/services/user.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/jsm_user_services/settings.py` & `jsm_user_services-1.3.4/jsm_user_services/settings.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/jsm_user_services/support/auth_jwt.py` & `jsm_user_services-1.3.4/jsm_user_services/support/auth_jwt.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/jsm_user_services/support/email_utils.py` & `jsm_user_services-1.3.4/jsm_user_services/support/email_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/jsm_user_services/support/http_utils.py` & `jsm_user_services-1.3.4/jsm_user_services/support/http_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/jsm_user_services/support/request_id.py` & `jsm_user_services-1.3.4/jsm_user_services/support/request_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from importlib import import_module
 from typing import Callable
 
 from jsm_user_services.exception import RequestIDModuleNotFound
 from jsm_user_services.support.import_utils import import_module_otherwise_none
 
 
+def parse_meta_header_to_request_header(value: str) -> str:
+    return value.replace("HTTP_", "").replace("_", "-")
+
+
 def get_request_id_header_name() -> str:
     """
     Helper function to get request_id header name to included in request to another application
     REQUEST_ID_CONFIG dict configuration exists in the projects with similarity structure below
     REQUEST_ID_CONFIG = {
         "REQUEST_ID_HEADER": "HTTP_X_REQUEST_ID",
         "GENERATE_REQUEST_ID_IF_NOT_FOUND": True,
@@ -20,16 +24,18 @@
     default_request_id_config = {
         "GENERATE_REQUEST_ID_IF_NOT_FOUND": True,
         "REQUEST_ID_HEADER": default_request_id_header_name,
         "RESPONSE_HEADER_REQUEST_ID": default_request_id_header_name,
     }
     request_id_config = getattr(settings, "REQUEST_ID_CONFIG", default_request_id_config)
     if request_id_config and type(request_id_config) == dict and request_id_config.get("REQUEST_ID_HEADER"):
-        return request_id_config.get("REQUEST_ID_HEADER", default_request_id_header_name)
-    return default_request_id_header_name
+        return parse_meta_header_to_request_header(
+            request_id_config.get("REQUEST_ID_HEADER", default_request_id_header_name)
+        )
+    return parse_meta_header_to_request_header(default_request_id_header_name)
 
 
 def get_current_request_id_callable() -> Callable:
     django_request_id_module, flask_request_id_module = (
         import_module_otherwise_none("request_id_django_log.request_id"),
         import_module_otherwise_none("flask_log_request_id"),
     )
```

### Comparing `jsm_user_services-1.3.3/jsm_user_services/support/settings_utils.py` & `jsm_user_services-1.3.4/jsm_user_services/support/settings_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.3.3/pyproject.toml` & `jsm_user_services-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jsm-user-services"
-version = "1.3.3"
+version = "1.3.4"
 description = "Middleware to intercept JWT auth token and more utils functions"
 authors = ["Juntos Somos Mais <labs@juntossomosmais.com.br>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "jsm_user_services"}]
 classifiers=[
     "Programming Language :: Python",
```

### Comparing `jsm_user_services-1.3.3/PKG-INFO` & `jsm_user_services-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsm-user-services
-Version: 1.3.3
+Version: 1.3.4
 Summary: Middleware to intercept JWT auth token and more utils functions
 License: MIT
 Author: Juntos Somos Mais
 Author-email: labs@juntossomosmais.com.br
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

