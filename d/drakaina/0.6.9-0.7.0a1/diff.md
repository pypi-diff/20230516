# Comparing `tmp/drakaina-0.6.9.tar.gz` & `tmp/drakaina-0.7.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drakaina-0.6.9.tar", max compression
+gzip compressed data, was "drakaina-0.7.0a1.tar", max compression
```

## Comparing `drakaina-0.6.9.tar` & `drakaina-0.7.0a1.tar`

### file list

```diff
@@ -1,43 +1,42 @@
--rw-r--r--   0        0        0     9542 2023-04-06 14:03:56.083341 drakaina-0.6.9/drakaina/__init__.py
--rw-r--r--   0        0        0     5953 2023-04-04 20:58:00.642760 drakaina-0.6.9/drakaina/_types.py
--rw-r--r--   0        0        0     1494 2023-01-27 12:48:38.216236 drakaina-0.6.9/drakaina/asgi.py
--rw-r--r--   0        0        0     3699 2023-02-13 13:22:12.183448 drakaina-0.6.9/drakaina/client/__init__.py
--rw-r--r--   0        0        0     6158 2022-07-08 05:47:38.000000 drakaina-0.6.9/drakaina/client/base.py
--rw-r--r--   0        0        0     1832 2022-07-08 05:47:38.000000 drakaina-0.6.9/drakaina/client/http.py
--rw-r--r--   0        0        0    11280 2023-01-27 12:55:37.114745 drakaina-0.6.9/drakaina/client/tcp.py
--rw-r--r--   0        0        0     8797 2022-07-08 05:47:38.000000 drakaina-0.6.9/drakaina/client/websocket.py
--rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.6.9/drakaina/contrib/__init__.py
--rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.6.9/drakaina/contrib/django/__init__.py
--rw-r--r--   0        0        0     1670 2023-04-04 16:03:12.444188 drakaina-0.6.9/drakaina/contrib/django/__rpc_methods.py
--rw-r--r--   0        0        0     6176 2023-04-05 13:26:05.508215 drakaina-0.6.9/drakaina/contrib/django/middleware.py
--rw-r--r--   0        0        0     3182 2023-04-05 13:26:05.517214 drakaina-0.6.9/drakaina/contrib/django/views.py
--rw-r--r--   0        0        0      340 2023-04-06 13:41:31.135135 drakaina-0.6.9/drakaina/contrib/jwt/__init__.py
--rw-r--r--   0        0        0     4831 2023-02-21 13:52:45.250648 drakaina-0.6.9/drakaina/contrib/jwt/auth_procedures.py
--rw-r--r--   0        0        0      348 2023-03-10 11:02:10.213372 drakaina-0.6.9/drakaina/contrib/jwt/errors.py
--rw-r--r--   0        0        0     9194 2023-04-06 14:03:56.084341 drakaina-0.6.9/drakaina/contrib/jwt/middleware.py
--rw-r--r--   0        0        0      913 2023-04-03 15:58:34.495338 drakaina-0.6.9/drakaina/contrib/jwt/types.py
--rw-r--r--   0        0        0    11530 2023-04-06 14:03:56.084341 drakaina-0.6.9/drakaina/contrib/jwt/utils.py
--rw-r--r--   0        0        0     1147 2023-04-05 18:02:08.709862 drakaina-0.6.9/drakaina/exceptions.py
--rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.6.9/drakaina/middleware/__init__.py
--rw-r--r--   0        0        0     1378 2023-03-29 21:57:07.601330 drakaina-0.6.9/drakaina/middleware/base.py
--rw-r--r--   0        0        0     7586 2023-04-06 14:03:56.085341 drakaina-0.6.9/drakaina/middleware/cors.py
--rw-r--r--   0        0        0     2112 2023-04-06 14:03:56.086341 drakaina-0.6.9/drakaina/middleware/exception.py
--rw-r--r--   0        0        0      406 2023-04-04 11:19:41.598921 drakaina-0.6.9/drakaina/middleware/gzip.py
--rw-r--r--   0        0        0      983 2023-04-04 11:19:41.525282 drakaina-0.6.9/drakaina/middleware/logging.py
--rw-r--r--   0        0        0     1138 2023-01-18 00:52:37.644550 drakaina-0.6.9/drakaina/middleware/openapi/__init__.py
--rw-r--r--   0        0        0     1079 2023-04-04 11:19:41.580823 drakaina-0.6.9/drakaina/middleware/request_wrapper.py
--rw-r--r--   0        0        0     3678 2023-04-06 14:03:56.086341 drakaina-0.6.9/drakaina/registries.py
--rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.6.9/drakaina/rpc_protocols/__init__.py
--rw-r--r--   0        0        0     4767 2023-04-06 14:00:17.561234 drakaina-0.6.9/drakaina/rpc_protocols/base.py
--rw-r--r--   0        0        0     8968 2023-04-06 14:00:17.568229 drakaina-0.6.9/drakaina/rpc_protocols/jsonrpc20.py
--rw-r--r--   0        0        0      200 2023-01-09 10:12:10.047554 drakaina-0.6.9/drakaina/rsgi.py
--rw-r--r--   0        0        0     4646 2023-02-27 17:00:44.197509 drakaina-0.6.9/drakaina/serializers.py
--rw-r--r--   0        0        0    11142 2023-01-27 12:51:42.029067 drakaina-0.6.9/drakaina/tcp.py
--rw-r--r--   0        0        0      937 2023-04-06 14:03:56.086869 drakaina-0.6.9/drakaina/utils.py
--rw-r--r--   0        0        0      162 2023-01-25 16:44:10.299855 drakaina-0.6.9/drakaina/ws.py
--rw-r--r--   0        0        0     7896 2023-04-06 14:03:56.086869 drakaina-0.6.9/drakaina/wsgi.py
--rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.6.9/LICENSE
--rw-r--r--   0        0        0     2461 2023-04-06 12:11:59.718408 drakaina-0.6.9/pyproject.toml
--rw-r--r--   0        0        0     5017 2023-04-06 14:03:56.083341 drakaina-0.6.9/README.md
--rw-r--r--   0        0        0     6109 1970-01-01 00:00:00.000000 drakaina-0.6.9/setup.py
--rw-r--r--   0        0        0     6371 1970-01-01 00:00:00.000000 drakaina-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     9580 2023-05-16 17:22:16.258425 drakaina-0.7.0a1/drakaina/__init__.py
+-rw-r--r--   0        0        0    11618 2023-05-16 17:22:16.259425 drakaina-0.7.0a1/drakaina/_types.py
+-rw-r--r--   0        0        0     1494 2023-01-27 12:48:38.216236 drakaina-0.7.0a1/drakaina/asgi.py
+-rw-r--r--   0        0        0     3699 2023-02-13 13:22:12.183448 drakaina-0.7.0a1/drakaina/client/__init__.py
+-rw-r--r--   0        0        0     6158 2022-07-08 05:47:38.000000 drakaina-0.7.0a1/drakaina/client/base.py
+-rw-r--r--   0        0        0     1832 2022-07-08 05:47:38.000000 drakaina-0.7.0a1/drakaina/client/http.py
+-rw-r--r--   0        0        0    11280 2023-01-27 12:55:37.114745 drakaina-0.7.0a1/drakaina/client/tcp.py
+-rw-r--r--   0        0        0     8797 2022-07-08 05:47:38.000000 drakaina-0.7.0a1/drakaina/client/websocket.py
+-rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.0a1/drakaina/contrib/__init__.py
+-rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.0a1/drakaina/contrib/django/__init__.py
+-rw-r--r--   0        0        0     6132 2023-04-11 08:46:20.669302 drakaina-0.7.0a1/drakaina/contrib/django/middleware.py
+-rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.0a1/drakaina/contrib/django/views.py
+-rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.0a1/drakaina/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0      348 2023-03-10 11:02:10.213372 drakaina-0.7.0a1/drakaina/contrib/jwt/errors.py
+-rw-r--r--   0        0        0     9102 2023-05-16 17:22:16.260425 drakaina-0.7.0a1/drakaina/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0      913 2023-04-03 15:58:34.495338 drakaina-0.7.0a1/drakaina/contrib/jwt/types.py
+-rw-r--r--   0        0        0    18791 2023-05-16 17:22:16.261447 drakaina-0.7.0a1/drakaina/contrib/jwt/utils.py
+-rw-r--r--   0        0        0     1651 2023-05-05 11:41:17.675178 drakaina-0.7.0a1/drakaina/drakaina_openapi.py
+-rw-r--r--   0        0        0     1327 2023-05-11 09:46:59.367413 drakaina-0.7.0a1/drakaina/exceptions.py
+-rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.0a1/drakaina/middleware/__init__.py
+-rw-r--r--   0        0        0     1378 2023-03-29 21:57:07.601330 drakaina-0.7.0a1/drakaina/middleware/base.py
+-rw-r--r--   0        0        0     7586 2023-05-16 17:22:16.262429 drakaina-0.7.0a1/drakaina/middleware/cors.py
+-rw-r--r--   0        0        0     2040 2023-05-16 17:22:16.263429 drakaina-0.7.0a1/drakaina/middleware/exception.py
+-rw-r--r--   0        0        0      430 2023-04-13 16:28:59.822156 drakaina-0.7.0a1/drakaina/middleware/gzip.py
+-rw-r--r--   0        0        0      983 2023-04-04 11:19:41.525282 drakaina-0.7.0a1/drakaina/middleware/logging.py
+-rw-r--r--   0        0        0     1138 2023-01-18 00:52:37.644550 drakaina-0.7.0a1/drakaina/middleware/openapi/__init__.py
+-rw-r--r--   0        0        0     1079 2023-04-04 11:19:41.580823 drakaina-0.7.0a1/drakaina/middleware/request_wrapper.py
+-rw-r--r--   0        0        0    11854 2023-05-16 17:22:16.264433 drakaina-0.7.0a1/drakaina/registries.py
+-rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.0a1/drakaina/rpc_protocols/__init__.py
+-rw-r--r--   0        0        0    11979 2023-05-16 17:22:16.265431 drakaina-0.7.0a1/drakaina/rpc_protocols/base.py
+-rw-r--r--   0        0        0    10772 2023-05-16 17:22:16.266445 drakaina-0.7.0a1/drakaina/rpc_protocols/jsonrpc20.py
+-rw-r--r--   0        0        0      200 2023-01-09 10:12:10.047554 drakaina-0.7.0a1/drakaina/rsgi.py
+-rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.0a1/drakaina/serializers.py
+-rw-r--r--   0        0        0    11142 2023-01-27 12:51:42.029067 drakaina-0.7.0a1/drakaina/tcp.py
+-rw-r--r--   0        0        0     3740 2023-05-16 17:22:16.267427 drakaina-0.7.0a1/drakaina/utils.py
+-rw-r--r--   0        0        0      162 2023-01-25 16:44:10.299855 drakaina-0.7.0a1/drakaina/ws.py
+-rw-r--r--   0        0        0     8181 2023-05-16 17:22:16.268428 drakaina-0.7.0a1/drakaina/wsgi.py
+-rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.0a1/LICENSE
+-rw-r--r--   0        0        0     2715 2023-05-16 17:22:16.269432 drakaina-0.7.0a1/pyproject.toml
+-rw-r--r--   0        0        0     5358 2023-05-16 17:22:16.257427 drakaina-0.7.0a1/README.md
+-rw-r--r--   0        0        0     6643 1970-01-01 00:00:00.000000 drakaina-0.7.0a1/setup.py
+-rw-r--r--   0        0        0     6876 1970-01-01 00:00:00.000000 drakaina-0.7.0a1/PKG-INFO
```

### Comparing `drakaina-0.6.9/drakaina/__init__.py` & `drakaina-0.7.0a1/drakaina/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ENV_APP = "drakaina.app"
 ENV_IS_AUTHENTICATED = "auth.is_authenticated"
 ENV_USER = "user"
 ENV_USER_ID = "user_id"
 ENV_AUTH_PAYLOAD = "auth.payload"
 ENV_AUTH_SCOPES = "auth.scopes"
 
-T = TypeVar("T")
+T = TypeVar("T", bound=Callable)
 
 
 def remote_procedure(
     name: Optional[str] = None,
     registry: Optional[RPCRegistry] = None,
     provide_request: Optional[bool] = None,
     metadata: Optional[dict[str, Any]] = None,
@@ -76,15 +76,15 @@
     """
 
     def __decorator(
         procedure: T,
         _registry: RPCRegistry = None,
         _name: str = None,
         _provide_request: bool = None,
-        **_meta_options,
+        _metadata: dict | None = None,
     ) -> T:
         """Returns a registered procedure"""
 
         if iscoroutinefunction(procedure):
 
             async def wrapper(*args, **kwargs):
                 if not _provide_request:
@@ -107,47 +107,44 @@
         # Need to update the wrapper before registering in the registry
         decorated_procedure = update_wrapper(wrapper, procedure)
 
         if _registry is None:
             _registry = rpc_registry
         if _name is None:
             _name = procedure.__name__
-        _metadata = _meta_options.pop("metadata") or {}
         _registry.register_procedure(
             decorated_procedure,
             name=_name,
             provide_request=_provide_request,
-            metadata={**_metadata, **_meta_options},
+            metadata=_metadata,
         )
 
         return decorated_procedure
 
     if callable(name):
         return __decorator(
-            name,
-            registry,
-            None,
-            provide_request,
-            metadata=metadata,
-            **meta_options,
+            procedure=name,
+            _registry=registry,
+            _name=None,
+            _provide_request=provide_request,
+            _metadata={**(metadata or {}), **meta_options},
         )
     elif not isinstance(name, (str, type(None))):
         raise TypeError(
             "Expected first argument to be an str, a callable, or None",
         )
 
     def decorator(procedure):
         assert callable(procedure)
         return __decorator(
-            procedure,
-            registry,
-            name,
-            provide_request,
-            metadata=metadata,
-            **meta_options,
+            procedure=procedure,
+            _registry=registry,
+            _name=name,
+            _provide_request=provide_request,
+            _metadata={**(metadata or {}), **meta_options},
         )
 
     return decorator
 
 
 def login_required(*_args) -> Callable:
     """Requires login decorator.
```

### Comparing `drakaina-0.6.9/drakaina/asgi.py` & `drakaina-0.7.0a1/drakaina/asgi.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.6.9/drakaina/client/__init__.py` & `drakaina-0.7.0a1/drakaina/client/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.6.9/drakaina/client/base.py` & `drakaina-0.7.0a1/drakaina/client/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.6.9/drakaina/client/http.py` & `drakaina-0.7.0a1/drakaina/client/http.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.6.9/drakaina/client/tcp.py` & `drakaina-0.7.0a1/drakaina/client/tcp.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.6.9/drakaina/client/websocket.py` & `drakaina-0.7.0a1/drakaina/client/websocket.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.6.9/drakaina/contrib/django/__init__.py` & `drakaina-0.7.0a1/drakaina/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.6.9/drakaina/contrib/django/middleware.py` & `drakaina-0.7.0a1/drakaina/contrib/django/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 from django.utils.module_loading import import_string
 
 from drakaina import ENV_AUTH_PAYLOAD
 from drakaina import ENV_AUTH_SCOPES
 from drakaina import ENV_IS_AUTHENTICATED
 from drakaina import ENV_USER_ID
 from drakaina.contrib import django as default_settings
+from drakaina.contrib.django.views import RPCView
 from drakaina.contrib.jwt.errors import InvalidJWTTokenError
 from drakaina.contrib.jwt.utils import decode_jwt_token
 from drakaina.exceptions import AuthenticationFailedError
 from drakaina.exceptions import ForbiddenError
-from drakaina.rpc_protocols import BaseRPCProtocol
 
 __all__ = ("JWTAuthenticationMiddleware",)
 
 UserModel = get_user_model()
 ARG_PREFIX = "DRAKAINA_"
 
 
 class DjangoRPCView(Protocol):
-    handler: BaseRPCProtocol
+    cls: RPCView
 
     def __call__(self, request: HttpRequest, *args, **kwargs) -> HttpResponse:
         ...
 
 
 def get_settings_arg(settings_attribute: str) -> Any:
     return getattr(
@@ -50,28 +50,29 @@
 
     """
 
     csrf_exempt = True
 
     def __init__(self, view: DjangoRPCView):
         assert hasattr(
-            getattr(view, "cls", None),
+            view.cls,
             "handler",
         ), "The view must contain the BaseRPCProtocol implementation instance."
 
         self._rpc_view = view
-        self._rpc_handler = view.cls.handler  # noqa
+        self._rpc_handler = view.cls.handler
 
         self.credentials_required = get_settings_arg("CREDENTIALS_REQUIRED")
         self.prefix = get_settings_arg("JWT_PREFIX")
         self.cookie_key = get_settings_arg("JWT_COOKIE_KEY")
         self.use_cookies = get_settings_arg("JWT_USE_COOKIES")
         self.algorithms = get_settings_arg("JWT_ALGORITHMS")
-        self.secret_key = get_settings_arg("JWT_SECRET_KEY")
-        self.public_key = get_settings_arg("JWT_PUBLIC_KEY")
+        secret_key = get_settings_arg("JWT_SECRET_KEY")
+        public_key = get_settings_arg("JWT_PUBLIC_KEY")
+        self.__verify_key = secret_key or public_key
         self.decode_options = get_settings_arg("JWT_DECODE_OPTIONS")
         self.verify_values = get_settings_arg("JWT_VERIFY_VALUES")
         self.leeway = get_settings_arg("JWT_LEEWAY")
         self.user_id_field = get_settings_arg("JWT_USER_ID_FIELD")
 
         self.get_token = self._get_token
         token_getter = get_settings_arg("JWT_TOKEN_GETTER")
@@ -104,16 +105,15 @@
                 AuthenticationFailedError("Credential required"),
             )
 
         if token is not None:
             payload = decode_jwt_token(
                 token,
                 algorithms=self.algorithms,
-                signing_key=self.secret_key,
-                verify_key=self.public_key,
+                verify_key=self.__verify_key,
                 verify=True,
                 decode_options=self.decode_options,
                 verify_values=self.verify_values,
                 leeway=self.leeway,
             )
 
             if callable(self.token_is_revoked):
@@ -137,15 +137,15 @@
 
         return self._rpc_view(request, *args, **kwargs)
 
     def _get_token(self, request: HttpRequest) -> Optional[str]:
         if self.use_cookies:
             return request.COOKIES.get(self.cookie_key)
         else:
-            auth_header = request.META.get("Authorization")
+            auth_header = request.headers.get("Authorization")
             if auth_header is None:
                 return None
 
             try:
                 parts = auth_header.strip().split(" ")
             except ValueError:
                 raise AuthenticationFailedError(
@@ -166,15 +166,15 @@
     def _get_user(
         self,
         request: HttpRequest,
         payload: dict[str, Any],
     ) -> Optional[UserModel]:
         user_id = payload.get(self.user_id_field)
         if user_id is None:
-            return None  # todo: try returns request.user
+            return getattr(request, "user", None)
         return UserModel.objects.get(pk=user_id)
 
     def _error_response(self, error: Exception) -> HttpResponse:
         return HttpResponse(
             content=self._rpc_handler.get_raw_error(error),
             content_type=self._rpc_handler.content_type,
         )
```

### Comparing `drakaina-0.6.9/drakaina/contrib/django/views.py` & `drakaina-0.7.0a1/drakaina/contrib/django/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,26 +55,32 @@
 
         # Scan specified sub-modules
         autodiscover_modules(autodiscover)
 
         return csrf_exempt(view)
 
     def post(self, request: HttpRequest, *args, **kwargs) -> HttpResponse:
+        response_headers = {}
         if request.content_type != self.content_type:
             response = partial(HttpResponse, status=415)
             content = self.handler.get_raw_error(BadRequestError())
         elif len(request.body) > int(request.headers["Content-Length"]):
             response = HttpResponseBadRequest
             content = self.handler.get_raw_error(BadRequestError())
         else:
-            response = HttpResponse
             content = self.handler.handle_raw_request(
                 request.body,
                 request=request,
             )
+            if hasattr(request, "response"):
+                _response = request.response
+                if isinstance(_response, dict) and "headers" in _response:
+                    for header in _response["headers"]:
+                        response_headers[header[0]] = header[1]
+            response = partial(HttpResponse, headers=response_headers)
 
         return response(content=content, content_type=self.content_type)
 
     def http_method_not_allowed(
         self,
         request: HttpRequest,
         *args,
```

### Comparing `drakaina-0.6.9/drakaina/contrib/jwt/middleware.py` & `drakaina-0.7.0a1/drakaina/contrib/jwt/middleware.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import re
 from typing import Iterable
-from typing import Optional
 
 from drakaina import ENV_AUTH_PAYLOAD
 from drakaina import ENV_AUTH_SCOPES
 from drakaina import ENV_IS_AUTHENTICATED
 from drakaina import ENV_USER
 from drakaina import ENV_USER_ID
 from drakaina._types import ASGIReceive
@@ -61,41 +60,40 @@
             "verify_iss": False,  # Issuer
             "verify_aud": False,  # Audience
             "verify_exp": True,   # Expiry
             "verify_nbf": False,  # Not Before
             "verify_iat": True,   # Issued at
             "verify_jti": False,  # JWT ID
         }`
-    :type decode_options: Optional[dict[str, bool | Iterable[str]]]
+    :type decode_options: dict[str, bool | Iterable[str]] | None
     :param verify_values: A dictionary of key-value pairs, where key is
         the name of the key in the token payload, and the value to check can be
         a specific value, a list of possible values, or a re.Pattern object
         (the result of re.compile).
-    :type verify_values: Optional[dict[str, str | Iterable[str] | re.Pattern]]
+    :type verify_values: dict[str, str | Iterable[str] | re.Pattern] | None
     :param leeway_value: The value of leeway in seconds. Default: `0`.
     :type leeway_value: int | float
     :param user_id_field: The name of the key in the token payload to store
         the user ID. Default: `"user_id"`.
     :type user_id_field: str
     :param token_getter: Callable for an alternative way to get a token.
-    :type token_getter: TokenGetter
+    :type token_getter: TokenGetter | None
     :param user_getter: Callable to retrieve a user object.
-    :type user_getter: UserGetter
+    :type user_getter: UserGetter | None
     :param scopes_getter: Callable to get permission scopes.
-    :type scopes_getter: ScopesGetter
+    :type scopes_getter: ScopesGetter | None
     :param revoke_checker: Callable to verify that the token is revoked.
-    :type revoke_checker: RevokeChecker
+    :type revoke_checker: RevokeChecker | None
     :param kwargs: Other arguments to pass to the constructor of the base class.
 
     """
 
     __slots__ = (
         "_algorithms",
-        "__secret_key",
-        "__public_key",
+        "__verify_key",
         "_credentials_required",
         "_prefix",
         "_cookie_key",
         "_decode_options",
         "_verify_values",
         "_leeway",
         "_user_id_field",
@@ -111,29 +109,29 @@
         algorithms: str | Iterable[str] = SUPPORTED_ALGORITHMS,
         secret_key: str = None,
         public_key: str = None,
         credentials_required: bool = True,
         prefix: str = "Bearer",
         use_cookies: bool = False,
         cookie_key: str = "jwt",
-        decode_options: dict[bool | list[str]] = None,
-        verify_values: dict[str, str | Iterable[str] | re.Pattern] = None,
+        decode_options: dict[str, bool | list[str]] | None = None,
+        verify_values: dict[str, str | Iterable[str] | re.Pattern]
+        | None = None,
         leeway_value: int | float = 0,
         user_id_field: str = "user_id",
-        token_getter: Optional[TokenGetter] = None,
-        user_getter: Optional[UserGetter] = None,
-        scopes_getter: Optional[ScopesGetter] = None,
-        revoke_checker: Optional[RevokeChecker] = None,
+        token_getter: TokenGetter | None = None,
+        user_getter: UserGetter | None = None,
+        scopes_getter: ScopesGetter | None = None,
+        revoke_checker: RevokeChecker | None = None,
         **kwargs,
     ):
         super().__init__(app, **kwargs)
 
         self._algorithms = iterable_str_arg(algorithms)
-        self.__secret_key = secret_key
-        self.__public_key = public_key
+        self.__verify_key = secret_key or public_key
         self._credentials_required = credentials_required
         self._prefix = prefix
         self._cookie_key = cookie_key
         self._decode_options = (
             decode_options
             if decode_options is not None
             else {
@@ -174,27 +172,26 @@
         if not token and self._credentials_required:
             raise AuthenticationFailedError("Credential required")
 
         if token is not None:
             token_payload = decode_jwt_token(
                 token=token,
                 algorithms=self._algorithms,
-                signing_key=self.__secret_key,
-                verify_key=self.__public_key,
+                verify_key=self.__verify_key,
                 verify=True,
                 decode_options=self._decode_options,
                 verify_values=self._verify_values,
                 leeway=self._leeway,
             )
 
             if callable(self.is_revoked):
                 if self.is_revoked(environ, token_payload):
                     raise ForbiddenError("Token is revoked")
 
-            environ[ENV_USER_ID] = token_payload[self._user_id_field]
+            environ[ENV_USER_ID] = token_payload.get(self._user_id_field)
             environ[ENV_IS_AUTHENTICATED] = True
             environ[ENV_AUTH_PAYLOAD] = token_payload
 
             if callable(self.get_user):
                 environ[ENV_USER] = self.get_user(environ, token_payload)
             if callable(self.get_scopes):
                 environ[ENV_AUTH_SCOPES] = self.get_scopes(
@@ -211,15 +208,15 @@
         send: ASGISend,
     ):
         await self.app(scope, receive, send)
 
     def _token_from_auth_header(
         self,
         request: ASGIScope | WSGIEnvironment,
-    ) -> Optional[str]:
+    ) -> str | None:
         auth_header = request.get("HTTP_AUTHORIZATION")
 
         if auth_header is None:
             return None
 
         try:
             parts = auth_header.strip().split(" ")
@@ -236,15 +233,15 @@
             )
 
         return parts[1]
 
     def _token_from_cookies(
         self,
         request: ASGIScope | WSGIEnvironment,
-    ) -> Optional[str]:
+    ) -> str | None:
         cookie_header = request.get("HTTP_COOKIE")
 
         if cookie_header is None:
             return None
 
         cookies = get_cookies(cookie_header)
```

### Comparing `drakaina-0.6.9/drakaina/contrib/jwt/types.py` & `drakaina-0.7.0a1/drakaina/contrib/jwt/types.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.6.9/drakaina/contrib/jwt/utils.py` & `drakaina-0.7.0a1/drakaina/contrib/jwt/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 import re
 from datetime import datetime
 from datetime import timedelta
 
 try:
     from datetime import UTC
 except ImportError:
-    from datetime import tzinfo
+    from datetime import timezone
 
-    UTC = tzinfo(timedelta(minutes=0))  # noqa
+    UTC = timezone(timedelta(0), "UTC")
 
 from typing import Any
 from typing import Iterable
-from typing import Optional
+from typing import MutableMapping
 from uuid import uuid4
 
-from jwt import get_unverified_header
 from jwt import InvalidAlgorithmError
 from jwt import InvalidTokenError
 from jwt import PyJWKClient
+from jwt.algorithms import has_crypto
+from jwt.algorithms import requires_cryptography
 from jwt.api_jwt import decode_complete
+from jwt.api_jwt import encode
 
+from drakaina.contrib.jwt import RESERVED_FIELDS
+from drakaina.contrib.jwt import SUPPORTED_ALGORITHMS
 from drakaina.contrib.jwt.errors import InvalidJWTTokenError
 from drakaina.contrib.jwt.errors import JWTBackendError
 from drakaina.contrib.jwt.errors import ValidationJWTTokenError
 from drakaina.utils import iterable_str_arg
 
 
 def datetime_utc_now() -> datetime:
@@ -97,76 +101,89 @@
 
     """
     payload[claim] = value
 
 
 def set_expiration(
     payload: dict[str, Any],
-    now: datetime,
-    lifetime: timedelta,
+    expiration_time: datetime | int,
     claim: str = "exp",
 ):
     """Sets the expiration time of a token.
 
     https://tools.ietf.org/html/rfc7519#section-4.1.4
 
     :param payload: Token payload.
-    :param now: Current date/time value to set the claim.
-    :param lifetime: The value of the token lifetime to set the claim.
+    :param expiration_time: Date/time value to set the claim.
     :param claim: Claim short name (key).
 
     """
-    payload[claim] = datetime_to_timestamp(now + lifetime)
+    if isinstance(expiration_time, (int, float)):
+        payload[claim] = int(expiration_time)
+    else:
+        payload[claim] = datetime_to_timestamp(expiration_time)
 
 
 def set_not_before(
     payload: dict[str, Any],
-    activation_time: datetime,
+    activation_time: datetime | int,
     claim: str = "nbf",
 ):
     """Sets the time `Not before`.
 
     https://tools.ietf.org/html/rfc7519#section-4.1.5
 
     :param payload: Token payload.
     :param activation_time: Date/time value to set the claim.
     :param claim: Claim short name (key).
 
     """
-    payload[claim] = datetime_to_timestamp(activation_time)
+    if isinstance(activation_time, (int, float)):
+        payload[claim] = int(activation_time)
+    else:
+        payload[claim] = datetime_to_timestamp(activation_time)
 
 
-def set_issued_at(payload: dict[str, Any], now: datetime, claim: str = "iat"):
+def set_issued_at(
+    payload: dict[str, Any],
+    now: datetime | int,
+    claim: str = "iat",
+):
     """Sets the time of token issuance.
 
     https://tools.ietf.org/html/rfc7519#section-4.1.6
 
     :param payload: Token payload.
     :param now: Current date/time value to set the claim.
     :param claim: Claim short name (key).
 
     """
-    payload[claim] = datetime_to_timestamp(now)
+    if isinstance(now, (int, float)):
+        payload[claim] = int(now)
+    else:
+        payload[claim] = datetime_to_timestamp(now)
 
 
 def set_token_id(
     payload: dict[str, Any],
-    value: Optional[str] = None,
+    value: str | bool | None = None,
     claim: str = "jti",
 ):
     """Sets the token identifier.
 
     https://tools.ietf.org/html/rfc7519#section-4.1.7
 
     :param payload: Token payload.
     :param value: Value to set the claim. Default UUID4.
     :param claim: Claim short name (key).
 
     """
-    payload[claim] = value if value else uuid4().hex
+    if value is True or value is None:
+        value = uuid4().hex
+    payload[claim] = value
 
 
 def check_expiration(
     payload: dict[str, Any],
     now: datetime,
     claim: str = "exp",
 ):
@@ -249,134 +266,325 @@
 
 
 # Token handlers
 
 
 def decode_jwt_token(
     token: str,
-    algorithms: Iterable[str],
-    signing_key: str,
     verify_key: str,
+    algorithms: Iterable[str] = SUPPORTED_ALGORITHMS,
     verify: bool = True,
-    decode_options: dict[bool | list[str]] = None,
-    verify_values: dict[str, str | Iterable[str] | re.Pattern | None] = None,
+    decode_options: dict[str, bool | list[str]] | None = None,
+    verify_values: dict[str, str | Iterable[str] | re.Pattern] | None = None,
     leeway: int | float = 0,
-    jwk_url: Optional[str] = None,
+    jwk_url: str | None = None,
 ) -> dict[str, Any]:
     """Performs validation of the provided token and returns
     its payload dictionary.
 
     :param token: JWT token.
+    :param verify_key: The token verification key.
+        May be a signature key in symmetric algorithms, or a public key
+        in asymmetric signature algorithms.
     :param algorithms: Supported algorithms.
-    :param signing_key: Signing key if used symmetric algorithm.
-    :param verify_key: Public key if used asymmetric algorithm.
     :param verify: Verify token.
     :param decode_options: Options argument for `pyjwt.decode`.
-        Example:
+        Default PyJWT values:
         `{
-            "require": ["iss", "exp", "jti"],
-            "verify_iss": False,
+            "verify_signature": True,
             "verify_exp": True,
-            "verify_jti": False,
+            "verify_nbf": True,
+            "verify_iat": True,
+            "verify_aud": True,
+            "verify_iss": True,
+            "require": [],
         }`
     :param verify_values: Values to be verified.
     :param leeway: Leeway time in seconds.
     :param jwk_url: URL for the PyJWK client.
         It gets the validation key for the specified jwt-token.
     :return: Decoded JWT token payload.
 
     :raise JWTBackendError: In the case of incorrectly passed
         parameters and arguments.
     :raise ValidationJWTTokenError: In case the token has an invalid signature
         or invalid payload data.
 
     """
 
-    header = get_unverified_header(token)
-    if header["alg"].startswith("HS"):
-        verifying_key = signing_key
-    elif jwk_url:
+    if jwk_url:
         jwks_client = PyJWKClient(jwk_url)
-        verifying_key = jwks_client.get_signing_key_from_jwt(token).key
-    else:
-        verifying_key = verify_key
+        verify_key = jwks_client.get_signing_key_from_jwt(token).key
 
     verify_values = {} if verify_values is None else verify_values.copy()
-    options = {"verify_signature": verify, **decode_options}
+    options = {"verify_signature": verify, **(decode_options or {})}
     params = {"leeway": leeway}
 
     # Provide values to check in the pyjwt module
-    if "verify_iss" in options and options["verify_iss"] is True:
-        # Issuer - One
-        params["issuer"] = verify_values.pop("iss")
-    if "verify_aud" in options and options["verify_aud"] is True:
-        # Audience - One or Many
-        if isinstance(verify_values.get("aud"), (str, list)):
-            params["audience"] = verify_values.pop("aud")
-        else:
-            # todo: will be validate in `_extra_validation`
-            options["verify_aud"] = False
+    if "iss" in verify_values and not isinstance(
+        verify_values["iss"],
+        (Iterable, re.Pattern),  # for pyjwt issuer must be single
+    ):
+        params["issuer"] = verify_values.pop("iss", None)
+    if "aud" in verify_values and not isinstance(
+        verify_values["aud"],
+        re.Pattern,  # for pyjwt audience must be single or iterable
+    ):
+        params["audience"] = verify_values.pop("aud")
 
     try:
         token_data = decode_complete(
             jwt=token,
-            key=verifying_key,
+            key=verify_key,
             algorithms=algorithms,
             options=options,
-            verify=verify,
             **params,
         )
     except InvalidAlgorithmError as error:
         raise JWTBackendError("Invalid algorithm specified") from error
     except InvalidTokenError:
-        raise ValidationJWTTokenError("Token is invalid or expired")
+        raise InvalidJWTTokenError("Token is invalid or expired")
 
     if verify:
         _extra_validation(token_data, verify_values)
 
     return token_data["payload"]
 
 
+def encode_jwt_token(
+    signing_key: str,
+    algorithm: str = "HS256",
+    payload: dict[str, Any] | None = None,
+    issuer: str | None = None,
+    subject: str | None = None,
+    audience: str | None = None,
+    expiration: datetime | timedelta | int | None = None,
+    not_before: datetime | timedelta | int | bool | None = None,
+    issued_at: datetime | int | bool | None = None,
+    token_id: int | str | bool | None = None,
+    token_type: str | None = None,
+    permission_scopes: str | Iterable[str] | None = None,
+    headers: dict[str, Any] | None = None,
+) -> str:
+    """Returns an encoded token with the specified payload and
+    specified parameters.
+
+    The claims from the specification for JWT tokens are expected in
+    the corresponding key parameters.
+
+    :param signing_key: The secret key to sign a token.
+    :param algorithm: Token Signing Algorithm.
+    :param payload: Token payload.
+    :param issuer: Issuer.
+    :param subject: Subject.
+    :param audience: Audience.
+    :param expiration: Expiration time.
+    :param not_before: Not before time.
+        If `True`, the current time is applied.
+    :param issued_at: Issued at the time.
+        If `True`, the current time is applied. Default: `True`.
+    :param token_id: Token ID.
+        If `True`, then uuid4 is generated.
+    :param token_type: The type of token, if you need it.
+        It has the standard claim `jtt'.
+    :param permission_scopes: Scope of permits, if you need them.
+        It has the standard claim `scp'.
+    :param headers: JWT token headers. RFC7519#section5
+    :return: Encoded JWT token.
+
+    """
+    _validate_algorithm(algorithm)
+
+    if not isinstance(payload, (dict, MutableMapping)):
+        payload = {}
+    else:
+        payload = payload.copy()
+        _validate_payload(payload)
+
+    if issuer:
+        set_issuer(payload, issuer)
+    if subject:
+        set_subject(payload, subject)
+    if audience:
+        set_audience(payload, audience)
+
+    now = datetime_utc_now()
+
+    if expiration:
+        if isinstance(expiration, timedelta):
+            expiration = now + expiration
+        set_expiration(payload, expiration)
+    if not_before:
+        if isinstance(not_before, timedelta):
+            not_before = now + not_before
+        elif not_before is True:
+            not_before = now
+        set_not_before(payload, not_before)
+    if issued_at:
+        if issued_at is True:
+            issued_at = now
+        set_issued_at(payload, issued_at)
+
+    if token_id:
+        set_token_id(payload, token_id)
+
+    if token_type:
+        set_token_type(payload, token_type)
+    if permission_scopes:
+        set_permission_scopes(payload, permission_scopes)
+
+    return encode(
+        payload=payload,
+        key=signing_key,
+        algorithm=algorithm,
+        headers=headers,
+    )
+
+
+# Helpful functions
+
+
+def copy_payload(
+    payload: dict[str, Any],
+    no_copy: Iterable[str] = ("exp", "nbf", "iat", "jti", "jtt", "scp"),
+) -> tuple[dict[str, Any], ...]:
+    """This function helps to copy the data of the old token and prepare
+    the payload and parameters of the new token creation function.
+
+    The data that can be safely copied will be returned by the first mapping.
+    And the data of the JWT specification fields expected by
+    the `encode_jwt_token` function as function parameters will be
+    returned by the second mapping.
+
+    This can be applied e.g. when updating an old token, keeping
+    permanent data, and updating data critical for token verification
+    and rotation.
+
+    Example ::
+
+        >>> payload, params = copy_payload(old_token_payload)
+        >>> token = encode_jwt_token("_secret_", payload=payload, **params)
+
+    :param payload: The payload for copying.
+    :param no_copy: Claims that don't require copying.
+    :return: A tuple of two elements, where the first is a filtered copy
+        of the payload and the second is a mapping with parameters
+        to pass to the `encode_jwt_token` function.
+
+    """
+    payload = payload.copy()
+
+    # Mapping as { claim_abbr: param_name }
+    encode_params_map = {
+        "iss": "issuer",
+        "sub": "subject",
+        "aud": "audience",
+        "exp": "expiration",
+        "nbf": "not_before",
+        "iat": "issued_at",
+        "jti": "token_id",
+        "jtt": "token_type",
+        "scp": "permission_scopes",
+    }
+    # Preparing parameters for the `encode_jwt_token` function
+    new_encode_params = {}
+    for claim, param_name in encode_params_map.items():
+        if claim in payload and claim not in no_copy:
+            new_encode_params[param_name] = payload.pop(claim)
+
+    # Copying the remaining payload
+    new_payload = {
+        claim: value for claim, value in payload.items() if claim not in no_copy
+    }
+
+    return new_payload, new_encode_params
+
+
 def _extra_validation(
     decoded_token: dict[str, dict[str, Any] | str],
-    verify_values: dict[str, str | Iterable[str] | re.Pattern] = None,
+    verify_values: dict[str, str | Iterable[str] | re.Pattern | dict] = None,
 ):
     """Performs an additional check that is not performed by the pyjwt module.
 
     The check is performed by comparing the data provided for the check with
     the data included in the token payload with the same keys.
 
     :param decoded_token: Dict returned from `pyjwt.decode_complete`. Must
         contain a `header' and `payload'.
     :param verify_values: Dict with data to be validated. The keys must match
         the dictionary fields with the token payload.
     :raise ValidationJWTTokenError: In case the token has an invalid
         payload or header data.
 
     """
-    header = decoded_token["header"]
-    verify_header_values = verify_values.pop("header", [])
-    payload = decoded_token["payload"]
+    if verify_values is None:
+        verify_values = {}
 
+    header = decoded_token["header"]
+    verify_header_values = verify_values.pop("header", {})
     try:
-        for key, value in verify_header_values:
+        for key, verify_value in verify_header_values.items():
             token_value = header.get(key)
-            if isinstance(value, (str, int)):
-                assert value == token_value
-            elif isinstance(value, Iterable):
-                assert token_value in value
-            elif isinstance(value, re.Pattern):
-                assert re.match(value, token_value)
+            if isinstance(verify_value, (str, int)):
+                assert token_value == verify_value
+            elif isinstance(verify_value, (list, set, tuple)):
+                assert token_value in verify_value
+            elif isinstance(verify_value, re.Pattern):
+                assert re.match(verify_value, token_value)
     except AssertionError as error:
         raise ValidationJWTTokenError("Invalid token header") from error
 
+    payload = decoded_token["payload"]
     try:
-        for key, value in verify_values:
+        for key, verify_value in verify_values.items():
             token_value = payload.get(key)
-            if isinstance(value, (str, int)):
-                assert value != token_value
-            elif isinstance(value, Iterable):
-                assert token_value not in value
-            elif isinstance(value, re.Pattern):
-                assert value.match(token_value)
+            if isinstance(verify_value, (str, int)):
+                assert token_value == verify_value
+            elif isinstance(verify_value, (list, set, tuple)):
+                assert token_value in verify_value
+            elif isinstance(verify_value, re.Pattern):
+                assert verify_value.match(token_value)
     except AssertionError as error:
         raise ValidationJWTTokenError("Invalid token payload") from error
+
+
+def _validate_algorithm(algorithm: str):
+    """Check that the specified algorithm is recognized, and that
+    `cryptography' is installed for those algorithms that require it.
+
+    :param algorithm: Algorithm to verify.
+    :raise JWTBackendError: If the algorithm is not recognized or not supported.
+    :raise ModuleNotFoundError: If the `cryptography' package is not installed.
+
+    """
+    if algorithm not in SUPPORTED_ALGORITHMS:
+        raise JWTBackendError(f"Unrecognized algorithm type '{algorithm}'")
+
+    if algorithm in requires_cryptography and not has_crypto:
+        raise ModuleNotFoundError(
+            f"To use `{algorithm}` you must install the `cryptography` package",
+        )
+
+
+def _validate_payload(payload: dict[str, Any]):
+    """Checks that the payload does not use reserved fields.
+
+    :param payload: Payload to verify.
+    :raise JWTBackendError: If the provided payload has reserved fields.
+
+    """
+    for reserved_jwt_claim in RESERVED_FIELDS:
+        if reserved_jwt_claim in payload:
+            if reserved_jwt_claim == "jtt":
+                raise JWTBackendError(
+                    f"The claim `{reserved_jwt_claim}` is reserved in "
+                    f"Drakaina to be specified as `token_type`.",
+                )
+            elif reserved_jwt_claim == "scp":
+                raise JWTBackendError(
+                    f"The claim `{reserved_jwt_claim}` is reserved in "
+                    f"Drakaina to be specified as `permission_scopes`.",
+                )
+            raise JWTBackendError(
+                "Please use keyword arguments to fill in "
+                "the JWT specification fields.",
+            )
```

### Comparing `drakaina-0.6.9/drakaina/exceptions.py` & `drakaina-0.7.0a1/drakaina/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,18 +7,24 @@
     message: str = None
 
     def __init__(self, *args):
         super().__init__(*args)
         if len(args) > 0:
             self.message = str(args[0])
 
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__} ({self.message})"
+
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__} ({self.message})>"
+
     def as_dict(self) -> dict[str, str]:
         return {
             "error": self.__class__.__name__,
-            "message": str(self.message or self),
+            "message": self.message or "",
         }
 
 
 class SerializationError(RPCError):
     """Serialization error"""
```

### Comparing `drakaina-0.6.9/drakaina/middleware/base.py` & `drakaina-0.7.0a1/drakaina/middleware/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.6.9/drakaina/middleware/cors.py` & `drakaina-0.7.0a1/drakaina/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.6.9/drakaina/middleware/exception.py` & `drakaina-0.7.0a1/drakaina/middleware/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
+
 from logging import Logger
-from typing import Optional
 
 from drakaina._types import ASGIApplication
 from drakaina._types import ASGIReceive
 from drakaina._types import ASGIScope
 from drakaina._types import ASGISend
 from drakaina._types import WSGIApplication
 from drakaina._types import WSGIEnvironment
@@ -15,42 +16,41 @@
 
 class ExceptionMiddleware(BaseMiddleware):
     """The middleware for handling unhandled exceptions in the application
     according to the RPC protocol.
 
     """
 
-    __slots__ = ("handler", "_rpc_content_type", "_logger")
+    __slots__ = ("handler", "_logger")
 
     def __init__(
         self,
         app: ASGIApplication | WSGIApplication,
         handler: BaseRPCProtocol,
-        logger: Optional[Logger] = None,
+        logger: Logger | None = None,
         is_async: bool = False,
     ):
         super().__init__(app=app, is_async=is_async)
 
         self.handler = handler
-        self._rpc_content_type = self.handler.content_type
         self._logger = logger
 
     def __wsgi_call__(
         self,
         environ: WSGIEnvironment,
         start_response: WSGIStartResponse,
     ) -> WSGIResponse:
         try:
             return self.app(environ, start_response)
         except Exception as error:
             if self._logger is not None:
                 self._logger.exception(error)
             response_body = self.handler.get_raw_error(error)
             response_headers = [
-                ("Content-Type", self._rpc_content_type),
+                ("Content-Type", self.handler.content_type),
                 ("Content-Length", str(len(response_body))),
             ]
             start_response("200 OK", response_headers)
             return (response_body,)
 
     async def __asgi_call__(
         self,
```

### Comparing `drakaina-0.6.9/drakaina/middleware/logging.py` & `drakaina-0.7.0a1/drakaina/middleware/logging.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.6.9/drakaina/middleware/openapi/__init__.py` & `drakaina-0.7.0a1/drakaina/middleware/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.6.9/drakaina/middleware/request_wrapper.py` & `drakaina-0.7.0a1/drakaina/middleware/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.6.9/drakaina/serializers.py` & `drakaina-0.7.0a1/drakaina/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         super().__init__()
         self.dumps = partial(ujson.dumps, ensure_ascii=False, **encode_kw or {})
         self.loads = partial(ujson.loads, **decode_kw or {})
         self.DecodeError = ujson.JSONDecodeError
 
 
 class MSGPackSerializer(BaseSerializer):
-    content_type: str = "application/octet-stream"
+    content_type: str = "application/x-msgpack"
 
     def __init__(
         self,
         packer: Optional[Type["msgpack.Packer"]] = None,
         unpacker: Optional[Type["msgpack.Unpacker"]] = None,
         pack_kw: Optional[dict] = None,
         unpack_kw: Optional[dict] = None,
```

### Comparing `drakaina-0.6.9/drakaina/tcp.py` & `drakaina-0.7.0a1/drakaina/tcp.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.6.9/drakaina/wsgi.py` & `drakaina-0.7.0a1/drakaina/wsgi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,114 +1,132 @@
 from __future__ import annotations
 
+import re
 from functools import partial
 from logging import Logger
+from sys import version_info
 from typing import Iterable
-from typing import Optional
-from typing import Type
-from typing import Union
 
 from drakaina import ENV_APP
 from drakaina._types import WSGIApplication
 from drakaina._types import WSGIEnvironment
 from drakaina._types import WSGIInputStream
 from drakaina._types import WSGIResponse
 from drakaina._types import WSGIStartResponse
 from drakaina.exceptions import BadRequestError
 from drakaina.middleware.base import BaseMiddleware
 from drakaina.middleware.exception import ExceptionMiddleware
 from drakaina.middleware.request_wrapper import RequestWrapperMiddleware
 from drakaina.rpc_protocols import BaseRPCProtocol
 from drakaina.rpc_protocols import JsonRPCv2
+from drakaina.utils import match_path
+
+if version_info < (3, 9):
+    from typing import Type
+    from typing import Union
+    from typing_extensions import TypeAlias
+
+    Middlewares: TypeAlias = Iterable[
+        Union[Type[BaseMiddleware], partial[BaseMiddleware]],
+    ]
+elif version_info < (3, 10):
+    from typing import Union
+    from typing_extensions import TypeAlias
+
+    Middlewares: TypeAlias = Iterable[
+        Union[type[BaseMiddleware], partial[BaseMiddleware]],
+    ]
+else:
+    from typing import TypeAlias
+
+    Middlewares: TypeAlias = Iterable[
+        type[BaseMiddleware] | partial[BaseMiddleware],
+    ]
+
+__all__ = ("WSGIHandler",)
 
 ALLOWED_METHODS = ("OPTIONS", "GET", "POST")
-Middlewares = Iterable[Type[BaseMiddleware] | partial[BaseMiddleware]]
 
 
 class WSGIHandler:
     """Implementation of WSGI protocol.
 
     :param route:
-    :type route: str
+    :type route: str | re.Pattern
     :param handler: RPC protocol implementation.
     :type handler: BaseRPCProtocol
     :param middlewares: List of WSGI middlewares.
-    :type middlewares: Iterable[Type[BaseMiddleware] | partial[BaseMiddleware]]
+    :type middlewares: Iterable[type[BaseMiddleware] | partial[BaseMiddleware]]
     :param logger: A `logging.Logger` object.
     :type logger: Logger
     :param max_content_size: Limiting request body size for DoS protection.
     :type max_content_size: int
-    :param provide_smd:
-    :type provide_smd: bool | str
-    :param provide_openrpc:
-    :type provide_openrpc: bool | str
-    :param provide_openapi:
-    :type provide_openapi: bool | str
+    :param openrpc_url: OpenRPC Schema URL.
+        The recommended document name is `openrpc.json`.
+    :type openrpc_url: str | re.Pattern
+    :param openapi_url: OpenAPI Schema URL.
+        The recommended document name is `openapi.json`.
+    :type openapi_url: str | re.Pattern
 
     """
 
     __slots__ = (
         "environ",
         "start_response",
         "handler",
         "route",
         "logger",
         "max_content_size",
-        "provide_smd",
-        "provide_openrpc",
-        "provide_openapi",
+        "openrpc_url",
+        "openapi_url",
         "_rpc_content_type",
         "_allowed_methods",
         "_middlewares_chain",
     )
 
     environ: WSGIEnvironment
     start_response: WSGIStartResponse
-    _middlewares_chain: Union[WSGIApplication, BaseMiddleware]
+    _middlewares_chain: WSGIApplication | BaseMiddleware
 
     def __init__(
         self,
-        route: Optional[str] = None,
-        handler: Optional[BaseRPCProtocol] = None,
-        middlewares: Optional[Middlewares] = None,
-        logger: Optional[Logger] = None,
+        route: str | re.Pattern | None = None,
+        handler: BaseRPCProtocol | None = None,
+        middlewares: Middlewares | None = None,
+        logger: Logger | None = None,
         max_content_size: int = 4096,
-        provide_smd: Optional[Union[bool, str]] = False,
-        provide_openrpc: Optional[Union[bool, str]] = False,
-        provide_openapi: Optional[Union[bool, str]] = False,
+        openrpc_url: str | re.Pattern | None = None,
+        openapi_url: str | re.Pattern | None = None,
     ):
         self.handler = handler if handler is not None else JsonRPCv2()
         self._rpc_content_type = self.handler.content_type
 
         self.route = route
         if isinstance(self.route, str) and not self.route.startswith("/"):
             self.route = "/" + self.route
 
         self.logger = logger
         self.max_content_size = int(max_content_size)
-        self.provide_smd = provide_smd
-        self.provide_openrpc = provide_openrpc
-        self.provide_openapi = provide_openapi
+        self.openrpc_url = openrpc_url
+        self.openapi_url = openapi_url
 
-        if provide_smd or provide_openrpc or provide_openapi:
+        if openrpc_url or openapi_url:
             self._allowed_methods = ", ".join(ALLOWED_METHODS)
         else:
             self._allowed_methods = ", ".join(
                 [m for m in ALLOWED_METHODS if m != "GET"],
             )
 
         # Build middleware stack
         self._middlewares_chain = self._wsgi_app
         kw = {"is_async": False}
-        for mw in reversed(middlewares or []):
+        for mw in reversed(middlewares or ()):
             if (
-                isinstance(mw, partial)
-                and issubclass(mw.func, BaseMiddleware)
-                or issubclass(mw, BaseMiddleware)
-            ):
+                isinstance(mw, partial) and issubclass(mw.func, BaseMiddleware)
+            ) or issubclass(mw, BaseMiddleware):
                 self._middlewares_chain = mw(self._middlewares_chain, **kw)
             self._middlewares_chain = mw(self._middlewares_chain)
 
         # The middleware for handling exceptions in the middleware according
         #  to the RPC protocol.
         self._middlewares_chain = ExceptionMiddleware(
             RequestWrapperMiddleware(self._middlewares_chain, **kw),  # noqa
@@ -131,47 +149,41 @@
         start_response: WSGIStartResponse,
     ) -> WSGIResponse:
         self.environ = environ
         self.start_response = start_response
 
         method = environ["REQUEST_METHOD"]
         if method in ALLOWED_METHODS:
-            if self._validate_path(environ["PATH_INFO"]):
-                return getattr(self, method.lower())()
-
-            return self._not_found()
+            return getattr(self, method.lower())()
 
         return self._method_not_allowed()
 
     def get(self) -> WSGIResponse:
-        if self.provide_smd:
-            response_body = self.handler.smd_scheme()
-            response_headers = [
-                ("Content-Type", "application/json"),
-                ("Content-Length", str(len(response_body))),
-            ]
-        elif self.provide_openrpc:
-            response_body = self.handler.openrpc_scheme()
+        if match_path(self.openrpc_url, self.environ["PATH_INFO"]):
+            response_body = self.handler.get_raw_openrpc_schema()
             response_headers = [
-                ("Content-Type", "application/json"),
+                ("Content-Type", self.handler.schema_content_type),
                 ("Content-Length", str(len(response_body))),
             ]
-        elif self.provide_openapi:
-            response_body = self.handler.openapi_scheme()
+        elif match_path(self.openapi_url, self.environ["PATH_INFO"]):
+            response_body = self.handler.get_raw_openapi_schema()
             response_headers = [
-                ("Content-Type", "application/json"),
+                ("Content-Type", self.handler.schema_content_type),
                 ("Content-Length", str(len(response_body))),
             ]
         else:
-            return self._method_not_allowed()
+            return self._not_found()
 
         self.start_response("200 OK", response_headers)
         return (response_body,)
 
     def post(self) -> WSGIResponse:
+        if not match_path(self.route, self.environ["PATH_INFO"]):
+            return self._not_found()
+
         wsgi_input: WSGIInputStream = self.environ["wsgi.input"]
 
         content_type = self.environ.get("CONTENT_TYPE")
         content_length = int(self.environ.get("CONTENT_LENGTH") or 0)
         if (
             not (content_type and content_length)
             or content_type != self._rpc_content_type
@@ -190,17 +202,21 @@
                 request=self.environ,
             )
 
         response_headers = [
             ("Content-Type", self._rpc_content_type),
             ("Content-Length", str(len(response_body))),
         ]
+        env_response_headers = self.environ.get("response", {}).get("headers")
+        if isinstance(env_response_headers, list):
+            response_headers.extend(env_response_headers)
+
         self.start_response(response_status, response_headers)
 
-        yield response_body
+        return (response_body,)
 
     def options(self) -> WSGIResponse:
         response_headers = [
             ("Allow", self._allowed_methods),
             ("Content-Length", "0"),
         ]
         self.start_response("200 OK", response_headers)
@@ -211,14 +227,7 @@
         self.start_response("404 Not Found", response_headers)
         yield b""
 
     def _method_not_allowed(self) -> WSGIResponse:
         response_headers = [("Allow", self._allowed_methods)]
         self.start_response("405 Method Not Allowed", response_headers)
         yield b""
-
-    def _validate_path(self, path_info: str) -> bool:
-        return (
-            self.route is not None
-            and isinstance(path_info, str)
-            and path_info.startswith(self.route)
-        )
```

### Comparing `drakaina-0.6.9/LICENSE` & `drakaina-0.7.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `drakaina-0.6.9/pyproject.toml` & `drakaina-0.7.0a1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,101 @@
-[tool.poetry]
-name = "drakaina"
-version = "0.6.9"
-description = "Module for simple RPC service implementation"
-authors = ["Aleksey Terentyev <terentyev.a@pm.me>"]
-license = "Apache License 2.0"
-readme = "README.md"
-classifiers = [
-    "Development Status :: 4 - Beta",
-    "Environment :: Web Environment",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: Apache Software License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Topic :: System :: Networking",
-    "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
-]
-keywords = ["rpc", "jsonrpc"]
-homepage  = "https://gitlab.com/tau_lex/drakaina"
-repository = "https://gitlab.com/tau_lex/drakaina"
-
-[project.urls]
-"Bug Tracker" = "https://gitlab.com/tau_lex/drakaina/-/issues"
-
-[tool.poetry.dependencies]
-python = "^3.7"
-typing-extensions = "^4.5.0"
-msgpack = { version = "^1.0.4", optional = true }
-orjson = { version = "^3.8.5", optional = true }
-ujson = { version = "^5.7.0", optional = true }
-pyjwt = { version = "^2.6.0", optional = true }
-
-[tool.poetry.extras]
-jwt = ["PyJWT"]
-ujson = ["ujson"]
-orjson = ["orjson"]
-msgpack = ["msgpack"]
-tests = ["pytest", "pyjwt", "django"]
-
-[tool.poetry.group.dev.dependencies]
-black = {extras = ["d"], version = "^22.12.0"}
-pre-commit = {version = "^3.0.0", python = ">=3.8"}
-ruff = "^0.0.236"
-msgpack = "^1.0.4"
-orjson = "^3.8.6"
-pytest = "^7.2.1"
-ujson = "^5.7.0"
-pyjwt = "^2.6.0"
-django = ">=3.2"
-
-[tool.poetry.group.tests.dependencies]
-pytest = "^7.2.1"
-httpx = "^0.23.3"
-
-[tool.pytest.ini_options]
-cache_dir = ".pytest_cache"
-testpaths = "tests"
-
-[tool.ruff]
-# Enable Pyflakes `E` and `F` codes by default.
-select = ["E", "F"]
-ignore = []
-
-# Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = ["A", "B", "C", "D", "E", "F"]
-unfixable = []
-
-exclude = [
-    ".git",
-    ".idea",
-    ".pytest_cache",
-    ".ruff_cache",
-    ".venv",
-    "content",
-    "dist",
-    "venv",
-]
-per-file-ignores = {}
-
-# Same as Black.
-line-length = 80
-
-# Allow unused variables when underscore-prefixed.
-dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
-
-target-version = "py37"
-
-[tool.ruff.mccabe]
-# Unlike Flake8, default to a complexity level of 10.
-max-complexity = 10
-
-[tool.black]
-target-version = ["py37"]
-line-length = 80
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "drakaina"
+version = "0.7.0-alpha.1"
+description = "Module for simple RPC service implementation"
+authors = ["Aleksey Terentyev <terentyev.a@pm.me>"]
+license = "Apache License 2.0"
+readme = "README.md"
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Environment :: Web Environment",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: System :: Networking",
+    "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
+]
+keywords = ["rpc", "jsonrpc"]
+homepage  = "https://gitlab.com/tau_lex/drakaina"
+repository = "https://gitlab.com/tau_lex/drakaina"
+
+[project.urls]
+"Bug Tracker" = "https://gitlab.com/tau_lex/drakaina/-/issues"
+
+[tool.poetry.dependencies]
+python = "^3.7"
+typing-extensions = "^4.5.0"
+msgpack = { version = "^1.0.4", optional = true }
+orjson = { version = "^3.8.5", optional = true }
+ujson = { version = "^5.7.0", optional = true }
+pyjwt = { version = "^2.6.0", optional = true }
+docstring-parser = { version = "^0.15", optional = true }
+
+[tool.poetry.extras]
+jwt = ["PyJWT"]
+ujson = ["ujson"]
+orjson = ["orjson"]
+msgpack = ["msgpack"]
+docs = ["docstring-parser"]
+tests = ["pytest", "httpx", "ujson", "orjson", "msgpack", "pyjwt", "django", "docstring-parser"]
+
+[tool.poetry.group.dev.dependencies]
+black = {extras = ["d"], version = "^22.12.0"}
+pre-commit = {version = "^3.0.0", python = ">=3.8"}
+ruff = "^0.0.236"
+msgpack = "^1.0.4"
+orjson = "^3.8.6"
+pytest = "^7.2.1"
+ujson = "^5.7.0"
+pyjwt = "^2.6.0"
+django = ">=3.2"
+
+[tool.poetry.group.tests.dependencies]
+pytest = "^7.2.1"
+httpx = "^0.23.3"
+
+[tool.pytest.ini_options]
+cache_dir = ".pytest_cache"
+testpaths = "tests"
+
+[tool.ruff]
+# Enable Pyflakes `E` and `F` codes by default.
+select = ["E", "F"]
+ignore = []
+
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+fixable = ["A", "B", "C", "D", "E", "F"]
+unfixable = []
+
+exclude = [
+    ".git",
+    ".idea",
+    ".pytest_cache",
+    ".ruff_cache",
+    ".venv",
+    "content",
+    "dist",
+    "venv",
+]
+per-file-ignores = {}
+
+# Same as Black.
+line-length = 80
+
+# Allow unused variables when underscore-prefixed.
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+target-version = "py37"
+
+[tool.ruff.mccabe]
+# Unlike Flake8, default to a complexity level of 10.
+max-complexity = 10
+
+[tool.black]
+target-version = ["py37"]
+line-length = 80
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `drakaina-0.6.9/README.md` & `drakaina-0.7.0a1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 [![image](https://img.shields.io/pypi/v/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![image](https://img.shields.io/pypi/l/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![image](https://img.shields.io/pypi/pyversions/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
 [![libera manifesto](https://img.shields.io/badge/libera-manifesto-lightgrey.svg)](https://liberamanifesto.com)
 
-❗ WIP
+❗ WIP ❗
 
-Module for simple RPC service implementation
+Framework for simple RPC service implementation.
 
 
 ## Quickstart
 
 Drakaina may be installed via `pip` and requires Python 3.7 or higher :
 
 ```shell
@@ -24,60 +24,39 @@
 
 A minimal Drakaina example is:
 
 ```python
 from drakaina import remote_procedure
 from drakaina.wsgi import WSGIHandler
 
-
-@remote_procedure
-def my_method():
-    return "Hello Bro! ✋️"
-
-
-@remote_procedure(name="something.get")
-def get_some_string():
-    return "You called `something.get`."
-
-
-@remote_procedure(provide_request=True)
-def do_something_with_environ(request):
-    return f"You called `do_something_with_environ`. Request: {request}."
-
-
-@remote_procedure()
-def tell_the_middleware_something():
-    return "You called `tell_the_middleware_something`. It has a some extra conditions."
-
-
-async def asynchronous_procedure():
-    await asyncio.sleep(5)
-    return "Ding-Dong 🔔!"
-
+@remote_procedure("hello")
+def hello_method(name):
+    return f"Hello, {name}!"
 
 """
->>> JsonRPCv2().handle({"jsonrpc": "2.0", "method": "my_method", "id": 1})
-or define WSGI application
+>>> from drakaina.rpc_protocols import JsonRPCv2
+>>> JsonRPCv2().handle({"jsonrpc": "2.0", "method": "hello", "params": ["🐍 Python"] "id": 1})
+{"jsonrpc": "2.0", "result": "Hello, 🐍 Python!", "id": 1}
 """
-app = WSGIHandler(route="/jrpc")
-```
 
-Drakaina may be ran with any WSGI-compliant server,
-such as [Gunicorn](http://gunicorn.org).
+# Or define WSGI application
+app = WSGIHandler(route="/jrpc")
 
-```shell
-gunicorn main:app
 ```
 
 
 ## Features
 
+- Serializers layer.
+  - `json`, `orjson`, `ujson` and `msgpack` serializers.
+- `login_required` and `check_permissions` decorators.
 - WSGI protocol implementation
-  - Implemented CORS middleware
-  - Compatible with simple middlewares for others wsgi-frameworks,
+  - CORS middleware
+  - JWT Authorization middleware.
+  - Compatible with middlewares for others wsgi-frameworks,
     like as [Werkzeug](https://palletsprojects.com/p/werkzeug/),
     [Flask](https://palletsprojects.com/p/flask/)
 
 
 # Documentation
 
 
@@ -98,57 +77,82 @@
 
 Drakaina may be installed via `pip` and requires Python 3.7 or higher :
 
 ```shell
 pip install drakaina[jwt]
 ```
 
-A minimal Drakaina example is:
+Example of using Drakaina:
 
 ```python
 from functools import partial
+from drakaina import check_permissions
 from drakaina import ENV_IS_AUTHENTICATED
 from drakaina import ENV_USER_ID
-from drakaina import remote_procedure
-from drakaina import check_permissions
 from drakaina import login_required
 from drakaina import match_any
+from drakaina import remote_procedure
 from drakaina.contrib.jwt.middleware import JWTAuthenticationMiddleware
 from drakaina.wsgi import WSGIHandler
 
+import user_store
+
 
 @login_required
 @remote_procedure(provide_request=True)
 def my_method(request):
     assert request[ENV_IS_AUTHENTICATED]
     return f"Hello Bro ✋! Your ID={request[ENV_USER_ID]}"
 
 
-@check_permissions(
-    scopes=["user_read", "app/user:admin", "username:johndoe"],
-    comparator=match_any,
-)
+@check_permissions(["user_read", "user:admin", "username:johndoe"], match_any)
 @remote_procedure
 def my_method():
     return "Hello Bro! ✋️"
 
 
+def get_user(request, payload):
+    user_id = request[ENV_USER_ID] or payload["user_id"]
+    return user_store.get(id=user_id)
+
+
+def get_jwt_scopes(request, payload):
+    # here `scp` is the key for the scopes value in the token payload
+    return payload.get("scp")
 
 
 app = WSGIHandler(
     middlewares=[
         partial(
             JWTAuthenticationMiddleware,
             secret_phrase="_secret_",
             credentials_required=True,
+            auth_scheme="Bearer",
+            # token_getter=custom_implementation_get_token,
+            user_getter=get_user,
+            scopes_getter=get_jwt_scopes,
+            # revoke_checker=is_revoked,
         )
     ]
 )
 ```
 
+Drakaina may be ran with any WSGI-compliant server,
+such as [Gunicorn](http://gunicorn.org).
+
+```shell
+gunicorn main:app
+```
+
+or ran with any ASGI-compliant server
+
+```shell
+uvicorn main:app2
+```
+
 
 ### Using with Django
 
 Create file `rpc_views.py` in your django application.
 Define function and wrap it `remote_procedure` decorator:
 
 ```python
@@ -191,15 +195,15 @@
 ```
 
 Define the parameters in the `settings.py` file.
 
 ```python
 ...
 
-DRAKAINA_JWT_SECRET_KEY = SECRET_KEY
+DRAKAINA_JWT_SECRET_KEY = "__SECRET_KEY__"
 
 ...
 ```
 
 
 ## License
```

### Comparing `drakaina-0.6.9/setup.py` & `drakaina-0.7.0a1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,25 +14,30 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['typing-extensions>=4.5.0,<5.0.0']
 
 extras_require = \
-{'jwt': ['pyjwt>=2.6.0,<3.0.0'],
+{'docs': ['docstring-parser>=0.15,<0.16'],
+ 'jwt': ['pyjwt>=2.6.0,<3.0.0'],
  'msgpack': ['msgpack>=1.0.4,<2.0.0'],
  'orjson': ['orjson>=3.8.5,<4.0.0'],
- 'tests': ['pyjwt>=2.6.0,<3.0.0'],
+ 'tests': ['msgpack>=1.0.4,<2.0.0',
+           'orjson>=3.8.5,<4.0.0',
+           'ujson>=5.7.0,<6.0.0',
+           'pyjwt>=2.6.0,<3.0.0',
+           'docstring-parser>=0.15,<0.16'],
  'ujson': ['ujson>=5.7.0,<6.0.0']}
 
 setup_kwargs = {
     'name': 'drakaina',
-    'version': '0.6.9',
+    'version': '0.7.0a1',
     'description': 'Module for simple RPC service implementation',
-    'long_description': '# drakaina\n\n![Drakaina](content/drakaina.png "Drakaina"){width=200px height=205px}\n\n[![image](https://img.shields.io/pypi/v/drakaina.svg)](https://pypi.python.org/pypi/drakaina)\n[![image](https://img.shields.io/pypi/l/drakaina.svg)](https://pypi.python.org/pypi/drakaina)\n[![image](https://img.shields.io/pypi/pyversions/drakaina.svg)](https://pypi.python.org/pypi/drakaina)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n[![libera manifesto](https://img.shields.io/badge/libera-manifesto-lightgrey.svg)](https://liberamanifesto.com)\n\n❗ WIP\n\nModule for simple RPC service implementation\n\n\n## Quickstart\n\nDrakaina may be installed via `pip` and requires Python 3.7 or higher :\n\n```shell\npip install drakaina\n```\n\nA minimal Drakaina example is:\n\n```python\nfrom drakaina import remote_procedure\nfrom drakaina.wsgi import WSGIHandler\n\n\n@remote_procedure\ndef my_method():\n    return "Hello Bro! ✋️"\n\n\n@remote_procedure(name="something.get")\ndef get_some_string():\n    return "You called `something.get`."\n\n\n@remote_procedure(provide_request=True)\ndef do_something_with_environ(request):\n    return f"You called `do_something_with_environ`. Request: {request}."\n\n\n@remote_procedure()\ndef tell_the_middleware_something():\n    return "You called `tell_the_middleware_something`. It has a some extra conditions."\n\n\nasync def asynchronous_procedure():\n    await asyncio.sleep(5)\n    return "Ding-Dong 🔔!"\n\n\n"""\n>>> JsonRPCv2().handle({"jsonrpc": "2.0", "method": "my_method", "id": 1})\nor define WSGI application\n"""\napp = WSGIHandler(route="/jrpc")\n```\n\nDrakaina may be ran with any WSGI-compliant server,\nsuch as [Gunicorn](http://gunicorn.org).\n\n```shell\ngunicorn main:app\n```\n\n\n## Features\n\n- WSGI protocol implementation\n  - Implemented CORS middleware\n  - Compatible with simple middlewares for others wsgi-frameworks,\n    like as [Werkzeug](https://palletsprojects.com/p/werkzeug/),\n    [Flask](https://palletsprojects.com/p/flask/)\n\n\n# Documentation\n\n\n## Installation\n\n```shell\npip install drakaina\n```\n\n\n## Middlewares\n\n\n### CORS\n\n\n### JWT\n\nDrakaina may be installed via `pip` and requires Python 3.7 or higher :\n\n```shell\npip install drakaina[jwt]\n```\n\nA minimal Drakaina example is:\n\n```python\nfrom functools import partial\nfrom drakaina import ENV_IS_AUTHENTICATED\nfrom drakaina import ENV_USER_ID\nfrom drakaina import remote_procedure\nfrom drakaina import check_permissions\nfrom drakaina import login_required\nfrom drakaina import match_any\nfrom drakaina.contrib.jwt.middleware import JWTAuthenticationMiddleware\nfrom drakaina.wsgi import WSGIHandler\n\n\n@login_required\n@remote_procedure(provide_request=True)\ndef my_method(request):\n    assert request[ENV_IS_AUTHENTICATED]\n    return f"Hello Bro ✋! Your ID={request[ENV_USER_ID]}"\n\n\n@check_permissions(\n    scopes=["user_read", "app/user:admin", "username:johndoe"],\n    comparator=match_any,\n)\n@remote_procedure\ndef my_method():\n    return "Hello Bro! ✋️"\n\n\n\n\napp = WSGIHandler(\n    middlewares=[\n        partial(\n            JWTAuthenticationMiddleware,\n            secret_phrase="_secret_",\n            credentials_required=True,\n        )\n    ]\n)\n```\n\n\n### Using with Django\n\nCreate file `rpc_views.py` in your django application.\nDefine function and wrap it `remote_procedure` decorator:\n\n```python\nfrom drakaina import remote_procedure\n\n@remote_procedure\ndef my_method():\n    return "Hello, Django Bro! ✋"\n```\n\nAdd `RPCView` class to urlpatterns. The `as_view` method\nmust accept the `autodiscover` argument as the name of\nthe remote procedure files.\n\n```python\nfrom django.urls import path\nfrom drakaina.contrib.django.views import RPCView\n\nurlpatterns = [\n    ...,\n    path("api/", RPCView.as_view(autodiscover="rpc_views")),\n]\n```\n\n\n### JWT Authentication in your Django project\n\nWrap an instance of `RPCView` with the `JWTAuthenticationMiddleware`.\n\n```python\nfrom django.urls import path\nfrom drakaina.contrib.django import RPCView, JWTAuthenticationMiddleware\n\nurlpatterns = [\n    ...,\n    path("api/", JWTAuthenticationMiddleware(\n        RPCView.as_view(autodiscover="rpc_views")\n    )),\n]\n```\n\nDefine the parameters in the `settings.py` file.\n\n```python\n...\n\nDRAKAINA_JWT_SECRET_KEY = SECRET_KEY\n\n...\n```\n\n\n## License\n\nApache License 2.0\n\n## Artwork\n\n"[drakaina.png](content/drakaina.png)" by Korolko Anastasia is licensed under\n<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="License Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a> ([CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)).\n',
+    'long_description': '# drakaina\n\n![Drakaina](content/drakaina.png "Drakaina"){width=200px height=205px}\n\n[![image](https://img.shields.io/pypi/v/drakaina.svg)](https://pypi.python.org/pypi/drakaina)\n[![image](https://img.shields.io/pypi/l/drakaina.svg)](https://pypi.python.org/pypi/drakaina)\n[![image](https://img.shields.io/pypi/pyversions/drakaina.svg)](https://pypi.python.org/pypi/drakaina)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n[![libera manifesto](https://img.shields.io/badge/libera-manifesto-lightgrey.svg)](https://liberamanifesto.com)\n\n❗ WIP ❗\n\nFramework for simple RPC service implementation.\n\n\n## Quickstart\n\nDrakaina may be installed via `pip` and requires Python 3.7 or higher :\n\n```shell\npip install drakaina\n```\n\nA minimal Drakaina example is:\n\n```python\nfrom drakaina import remote_procedure\nfrom drakaina.wsgi import WSGIHandler\n\n@remote_procedure("hello")\ndef hello_method(name):\n    return f"Hello, {name}!"\n\n"""\n>>> from drakaina.rpc_protocols import JsonRPCv2\n>>> JsonRPCv2().handle({"jsonrpc": "2.0", "method": "hello", "params": ["🐍 Python"] "id": 1})\n{"jsonrpc": "2.0", "result": "Hello, 🐍 Python!", "id": 1}\n"""\n\n# Or define WSGI application\napp = WSGIHandler(route="/jrpc")\n\n```\n\n\n## Features\n\n- Serializers layer.\n  - `json`, `orjson`, `ujson` and `msgpack` serializers.\n- `login_required` and `check_permissions` decorators.\n- WSGI protocol implementation\n  - CORS middleware\n  - JWT Authorization middleware.\n  - Compatible with middlewares for others wsgi-frameworks,\n    like as [Werkzeug](https://palletsprojects.com/p/werkzeug/),\n    [Flask](https://palletsprojects.com/p/flask/)\n\n\n# Documentation\n\n\n## Installation\n\n```shell\npip install drakaina\n```\n\n\n## Middlewares\n\n\n### CORS\n\n\n### JWT\n\nDrakaina may be installed via `pip` and requires Python 3.7 or higher :\n\n```shell\npip install drakaina[jwt]\n```\n\nExample of using Drakaina:\n\n```python\nfrom functools import partial\nfrom drakaina import check_permissions\nfrom drakaina import ENV_IS_AUTHENTICATED\nfrom drakaina import ENV_USER_ID\nfrom drakaina import login_required\nfrom drakaina import match_any\nfrom drakaina import remote_procedure\nfrom drakaina.contrib.jwt.middleware import JWTAuthenticationMiddleware\nfrom drakaina.wsgi import WSGIHandler\n\nimport user_store\n\n\n@login_required\n@remote_procedure(provide_request=True)\ndef my_method(request):\n    assert request[ENV_IS_AUTHENTICATED]\n    return f"Hello Bro ✋! Your ID={request[ENV_USER_ID]}"\n\n\n@check_permissions(["user_read", "user:admin", "username:johndoe"], match_any)\n@remote_procedure\ndef my_method():\n    return "Hello Bro! ✋️"\n\n\ndef get_user(request, payload):\n    user_id = request[ENV_USER_ID] or payload["user_id"]\n    return user_store.get(id=user_id)\n\n\ndef get_jwt_scopes(request, payload):\n    # here `scp` is the key for the scopes value in the token payload\n    return payload.get("scp")\n\n\napp = WSGIHandler(\n    middlewares=[\n        partial(\n            JWTAuthenticationMiddleware,\n            secret_phrase="_secret_",\n            credentials_required=True,\n            auth_scheme="Bearer",\n            # token_getter=custom_implementation_get_token,\n            user_getter=get_user,\n            scopes_getter=get_jwt_scopes,\n            # revoke_checker=is_revoked,\n        )\n    ]\n)\n```\n\nDrakaina may be ran with any WSGI-compliant server,\nsuch as [Gunicorn](http://gunicorn.org).\n\n```shell\ngunicorn main:app\n```\n\nor ran with any ASGI-compliant server\n\n```shell\nuvicorn main:app2\n```\n\n\n### Using with Django\n\nCreate file `rpc_views.py` in your django application.\nDefine function and wrap it `remote_procedure` decorator:\n\n```python\nfrom drakaina import remote_procedure\n\n@remote_procedure\ndef my_method():\n    return "Hello, Django Bro! ✋"\n```\n\nAdd `RPCView` class to urlpatterns. The `as_view` method\nmust accept the `autodiscover` argument as the name of\nthe remote procedure files.\n\n```python\nfrom django.urls import path\nfrom drakaina.contrib.django.views import RPCView\n\nurlpatterns = [\n    ...,\n    path("api/", RPCView.as_view(autodiscover="rpc_views")),\n]\n```\n\n\n### JWT Authentication in your Django project\n\nWrap an instance of `RPCView` with the `JWTAuthenticationMiddleware`.\n\n```python\nfrom django.urls import path\nfrom drakaina.contrib.django import RPCView, JWTAuthenticationMiddleware\n\nurlpatterns = [\n    ...,\n    path("api/", JWTAuthenticationMiddleware(\n        RPCView.as_view(autodiscover="rpc_views")\n    )),\n]\n```\n\nDefine the parameters in the `settings.py` file.\n\n```python\n...\n\nDRAKAINA_JWT_SECRET_KEY = "__SECRET_KEY__"\n\n...\n```\n\n\n## License\n\nApache License 2.0\n\n## Artwork\n\n"[drakaina.png](content/drakaina.png)" by Korolko Anastasia is licensed under\n<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="License Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a> ([CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)).\n',
     'author': 'Aleksey Terentyev',
     'author_email': 'terentyev.a@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/tau_lex/drakaina',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `drakaina-0.6.9/PKG-INFO` & `drakaina-0.7.0a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drakaina
-Version: 0.6.9
+Version: 0.7.0a1
 Summary: Module for simple RPC service implementation
 Home-page: https://gitlab.com/tau_lex/drakaina
 License: Apache-2.0
 Keywords: rpc,jsonrpc
 Author: Aleksey Terentyev
 Author-email: terentyev.a@pm.me
 Requires-Python: >=3.7,<4.0
@@ -19,41 +19,43 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
+Provides-Extra: docs
 Provides-Extra: jwt
 Provides-Extra: msgpack
 Provides-Extra: orjson
 Provides-Extra: tests
 Provides-Extra: ujson
-Requires-Dist: msgpack (>=1.0.4,<2.0.0) ; extra == "msgpack"
-Requires-Dist: orjson (>=3.8.5,<4.0.0) ; extra == "orjson"
+Requires-Dist: docstring-parser (>=0.15,<0.16) ; extra == "docs" or extra == "tests"
+Requires-Dist: msgpack (>=1.0.4,<2.0.0) ; extra == "msgpack" or extra == "tests"
+Requires-Dist: orjson (>=3.8.5,<4.0.0) ; extra == "orjson" or extra == "tests"
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0) ; extra == "jwt" or extra == "tests"
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
-Requires-Dist: ujson (>=5.7.0,<6.0.0) ; extra == "ujson"
+Requires-Dist: ujson (>=5.7.0,<6.0.0) ; extra == "ujson" or extra == "tests"
 Project-URL: Repository, https://gitlab.com/tau_lex/drakaina
 Description-Content-Type: text/markdown
 
 # drakaina
 
 ![Drakaina](content/drakaina.png "Drakaina"){width=200px height=205px}
 
 [![image](https://img.shields.io/pypi/v/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![image](https://img.shields.io/pypi/l/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![image](https://img.shields.io/pypi/pyversions/drakaina.svg)](https://pypi.python.org/pypi/drakaina)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
 [![libera manifesto](https://img.shields.io/badge/libera-manifesto-lightgrey.svg)](https://liberamanifesto.com)
 
-❗ WIP
+❗ WIP ❗
 
-Module for simple RPC service implementation
+Framework for simple RPC service implementation.
 
 
 ## Quickstart
 
 Drakaina may be installed via `pip` and requires Python 3.7 or higher :
 
 ```shell
@@ -62,60 +64,39 @@
 
 A minimal Drakaina example is:
 
 ```python
 from drakaina import remote_procedure
 from drakaina.wsgi import WSGIHandler
 
-
-@remote_procedure
-def my_method():
-    return "Hello Bro! ✋️"
-
-
-@remote_procedure(name="something.get")
-def get_some_string():
-    return "You called `something.get`."
-
-
-@remote_procedure(provide_request=True)
-def do_something_with_environ(request):
-    return f"You called `do_something_with_environ`. Request: {request}."
-
-
-@remote_procedure()
-def tell_the_middleware_something():
-    return "You called `tell_the_middleware_something`. It has a some extra conditions."
-
-
-async def asynchronous_procedure():
-    await asyncio.sleep(5)
-    return "Ding-Dong 🔔!"
-
+@remote_procedure("hello")
+def hello_method(name):
+    return f"Hello, {name}!"
 
 """
->>> JsonRPCv2().handle({"jsonrpc": "2.0", "method": "my_method", "id": 1})
-or define WSGI application
+>>> from drakaina.rpc_protocols import JsonRPCv2
+>>> JsonRPCv2().handle({"jsonrpc": "2.0", "method": "hello", "params": ["🐍 Python"] "id": 1})
+{"jsonrpc": "2.0", "result": "Hello, 🐍 Python!", "id": 1}
 """
-app = WSGIHandler(route="/jrpc")
-```
 
-Drakaina may be ran with any WSGI-compliant server,
-such as [Gunicorn](http://gunicorn.org).
+# Or define WSGI application
+app = WSGIHandler(route="/jrpc")
 
-```shell
-gunicorn main:app
 ```
 
 
 ## Features
 
+- Serializers layer.
+  - `json`, `orjson`, `ujson` and `msgpack` serializers.
+- `login_required` and `check_permissions` decorators.
 - WSGI protocol implementation
-  - Implemented CORS middleware
-  - Compatible with simple middlewares for others wsgi-frameworks,
+  - CORS middleware
+  - JWT Authorization middleware.
+  - Compatible with middlewares for others wsgi-frameworks,
     like as [Werkzeug](https://palletsprojects.com/p/werkzeug/),
     [Flask](https://palletsprojects.com/p/flask/)
 
 
 # Documentation
 
 
@@ -136,57 +117,82 @@
 
 Drakaina may be installed via `pip` and requires Python 3.7 or higher :
 
 ```shell
 pip install drakaina[jwt]
 ```
 
-A minimal Drakaina example is:
+Example of using Drakaina:
 
 ```python
 from functools import partial
+from drakaina import check_permissions
 from drakaina import ENV_IS_AUTHENTICATED
 from drakaina import ENV_USER_ID
-from drakaina import remote_procedure
-from drakaina import check_permissions
 from drakaina import login_required
 from drakaina import match_any
+from drakaina import remote_procedure
 from drakaina.contrib.jwt.middleware import JWTAuthenticationMiddleware
 from drakaina.wsgi import WSGIHandler
 
+import user_store
+
 
 @login_required
 @remote_procedure(provide_request=True)
 def my_method(request):
     assert request[ENV_IS_AUTHENTICATED]
     return f"Hello Bro ✋! Your ID={request[ENV_USER_ID]}"
 
 
-@check_permissions(
-    scopes=["user_read", "app/user:admin", "username:johndoe"],
-    comparator=match_any,
-)
+@check_permissions(["user_read", "user:admin", "username:johndoe"], match_any)
 @remote_procedure
 def my_method():
     return "Hello Bro! ✋️"
 
 
+def get_user(request, payload):
+    user_id = request[ENV_USER_ID] or payload["user_id"]
+    return user_store.get(id=user_id)
+
+
+def get_jwt_scopes(request, payload):
+    # here `scp` is the key for the scopes value in the token payload
+    return payload.get("scp")
 
 
 app = WSGIHandler(
     middlewares=[
         partial(
             JWTAuthenticationMiddleware,
             secret_phrase="_secret_",
             credentials_required=True,
+            auth_scheme="Bearer",
+            # token_getter=custom_implementation_get_token,
+            user_getter=get_user,
+            scopes_getter=get_jwt_scopes,
+            # revoke_checker=is_revoked,
         )
     ]
 )
 ```
 
+Drakaina may be ran with any WSGI-compliant server,
+such as [Gunicorn](http://gunicorn.org).
+
+```shell
+gunicorn main:app
+```
+
+or ran with any ASGI-compliant server
+
+```shell
+uvicorn main:app2
+```
+
 
 ### Using with Django
 
 Create file `rpc_views.py` in your django application.
 Define function and wrap it `remote_procedure` decorator:
 
 ```python
@@ -229,15 +235,15 @@
 ```
 
 Define the parameters in the `settings.py` file.
 
 ```python
 ...
 
-DRAKAINA_JWT_SECRET_KEY = SECRET_KEY
+DRAKAINA_JWT_SECRET_KEY = "__SECRET_KEY__"
 
 ...
 ```
 
 
 ## License
```

