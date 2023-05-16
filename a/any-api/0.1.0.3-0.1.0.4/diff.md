# Comparing `tmp/any_api-0.1.0.3.tar.gz` & `tmp/any_api-0.1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "any_api-0.1.0.3.tar", max compression
+gzip compressed data, was "any_api-0.1.0.4.tar", max compression
```

## Comparing `any_api-0.1.0.3.tar` & `any_api-0.1.0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11357 2022-08-24 12:23:30.000000 any_api-0.1.0.3/LICENSE
--rw-r--r--   0        0        0       25 2023-04-06 06:06:46.055887 any_api-0.1.0.3/any_api/__init__.py
--rw-r--r--   0        0        0        0 2022-10-28 09:49:12.000000 any_api-0.1.0.3/any_api/asyncapi/__init__.py
--rw-r--r--   0        0        0     3851 2022-11-09 10:01:05.000000 any_api-0.1.0.3/any_api/asyncapi/asyncapi.py
--rw-r--r--   0        0        0        0 2022-10-28 09:49:12.000000 any_api-0.1.0.3/any_api/asyncapi/model/__init__.py
--rw-r--r--   0        0        0     5145 2022-11-09 10:01:05.000000 any_api-0.1.0.3/any_api/asyncapi/model/asyncapi_model.py
--rw-r--r--   0        0        0     4502 2022-11-09 09:55:15.000000 any_api-0.1.0.3/any_api/asyncapi/model/operation_model.py
--rw-r--r--   0        0        0        0 2022-10-28 09:09:27.000000 any_api-0.1.0.3/any_api/base_api/__init__.py
--rw-r--r--   0        0        0     5581 2023-01-08 05:19:41.000000 any_api-0.1.0.3/any_api/base_api/base_api.py
--rw-r--r--   0        0        0        0 2022-10-28 09:09:27.000000 any_api-0.1.0.3/any_api/base_api/model/__init__.py
--rw-r--r--   0        0        0      788 2022-11-06 17:22:33.000000 any_api-0.1.0.3/any_api/base_api/model/base_api_model.py
--rw-r--r--   0        0        0      657 2023-04-06 03:37:55.268257 any_api-0.1.0.3/any_api/openapi/__init__.py
--rw-r--r--   0        0        0     5959 2023-04-06 03:37:55.264258 any_api-0.1.0.3/any_api/openapi/model/__init__.py
--rw-r--r--   0        0        0     3980 2023-04-04 03:36:57.298823 any_api-0.1.0.3/any_api/openapi/model/links.py
--rw-r--r--   0        0        0    20056 2023-01-06 03:43:04.000000 any_api-0.1.0.3/any_api/openapi/model/openapi/__init__.py
--rw-r--r--   0        0        0     2884 2022-11-09 10:04:21.000000 any_api-0.1.0.3/any_api/openapi/model/openapi/basic.py
--rw-r--r--   0        0        0     1820 2022-11-09 10:04:21.000000 any_api-0.1.0.3/any_api/openapi/model/openapi/info.py
--rw-r--r--   0        0        0     5672 2022-11-09 10:04:21.000000 any_api-0.1.0.3/any_api/openapi/model/openapi/security.py
--rw-r--r--   0        0        0     1475 2023-04-04 03:56:13.829648 any_api-0.1.0.3/any_api/openapi/model/requests.py
--rw-r--r--   0        0        0     3655 2023-01-13 10:23:53.000000 any_api-0.1.0.3/any_api/openapi/model/responses.py
--rw-r--r--   0        0        0      388 2023-01-10 16:04:06.000000 any_api-0.1.0.3/any_api/openapi/model/util.py
--rw-r--r--   0        0        0    18615 2023-04-06 03:42:47.831202 any_api-0.1.0.3/any_api/openapi/openapi.py
--rw-r--r--   0        0        0        0 2022-10-28 10:06:44.000000 any_api-0.1.0.3/any_api/openapi/to/__init__.py
--rw-r--r--   0        0        0    11232 2023-01-04 16:22:51.000000 any_api-0.1.0.3/any_api/openapi/to/markdown.py
--rw-r--r--   0        0        0      285 2023-01-09 03:46:58.000000 any_api-0.1.0.3/any_api/openapi/web_ui/__init__.py
--rw-r--r--   0        0        0     1042 2022-10-25 03:45:48.000000 any_api-0.1.0.3/any_api/openapi/web_ui/elements.py
--rw-r--r--   0        0        0     1196 2022-10-25 03:54:12.000000 any_api-0.1.0.3/any_api/openapi/web_ui/rapidoc.py
--rw-r--r--   0        0        0     1021 2022-06-18 16:09:46.000000 any_api-0.1.0.3/any_api/openapi/web_ui/redoc.py
--rw-r--r--   0        0        0     1285 2022-06-18 16:09:46.000000 any_api-0.1.0.3/any_api/openapi/web_ui/swagger.py
--rw-r--r--   0        0        0        0 2022-10-28 09:09:27.000000 any_api-0.1.0.3/any_api/util/__init__.py
--rw-r--r--   0        0        0     8208 2023-04-06 03:41:16.387441 any_api-0.1.0.3/any_api/util/by_pydantic.py
--rw-r--r--   0        0        0     4297 2022-11-02 11:53:55.000000 any_api-0.1.0.3/any_api/util/i18n.py
--rw-r--r--   0        0        0      193 2022-10-28 09:09:27.000000 any_api-0.1.0.3/any_api/util/util.py
--rw-r--r--   0        0        0     1634 2023-04-06 06:06:46.055887 any_api-0.1.0.3/pyproject.toml
--rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 any_api-0.1.0.3/setup.py
--rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 any_api-0.1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-08-24 12:23:30.000000 any_api-0.1.0.4/LICENSE
+-rw-r--r--   0        0        0       25 2023-05-16 10:09:38.209717 any_api-0.1.0.4/any_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-28 09:49:12.000000 any_api-0.1.0.4/any_api/asyncapi/__init__.py
+-rw-r--r--   0        0        0     3851 2022-11-09 10:01:05.000000 any_api-0.1.0.4/any_api/asyncapi/asyncapi.py
+-rw-r--r--   0        0        0        0 2022-10-28 09:49:12.000000 any_api-0.1.0.4/any_api/asyncapi/model/__init__.py
+-rw-r--r--   0        0        0     5145 2022-11-09 10:01:05.000000 any_api-0.1.0.4/any_api/asyncapi/model/asyncapi_model.py
+-rw-r--r--   0        0        0     4502 2022-11-09 09:55:15.000000 any_api-0.1.0.4/any_api/asyncapi/model/operation_model.py
+-rw-r--r--   0        0        0        0 2022-10-28 09:09:27.000000 any_api-0.1.0.4/any_api/base_api/__init__.py
+-rw-r--r--   0        0        0     6158 2023-05-16 10:00:16.655653 any_api-0.1.0.4/any_api/base_api/base_api.py
+-rw-r--r--   0        0        0        0 2022-10-28 09:09:27.000000 any_api-0.1.0.4/any_api/base_api/model/__init__.py
+-rw-r--r--   0        0        0      788 2022-11-06 17:22:33.000000 any_api-0.1.0.4/any_api/base_api/model/base_api_model.py
+-rw-r--r--   0        0        0      657 2023-04-06 03:37:55.268257 any_api-0.1.0.4/any_api/openapi/__init__.py
+-rw-r--r--   0        0        0     5399 2023-04-12 14:27:02.953045 any_api-0.1.0.4/any_api/openapi/model/__init__.py
+-rw-r--r--   0        0        0     3980 2023-04-04 03:36:57.298823 any_api-0.1.0.4/any_api/openapi/model/links.py
+-rw-r--r--   0        0        0    20056 2023-01-06 03:43:04.000000 any_api-0.1.0.4/any_api/openapi/model/openapi/__init__.py
+-rw-r--r--   0        0        0     2884 2022-11-09 10:04:21.000000 any_api-0.1.0.4/any_api/openapi/model/openapi/basic.py
+-rw-r--r--   0        0        0     1820 2022-11-09 10:04:21.000000 any_api-0.1.0.4/any_api/openapi/model/openapi/info.py
+-rw-r--r--   0        0        0     6532 2023-05-16 10:08:36.253191 any_api-0.1.0.4/any_api/openapi/model/openapi/security.py
+-rw-r--r--   0        0        0     1475 2023-04-04 03:56:13.829648 any_api-0.1.0.4/any_api/openapi/model/requests.py
+-rw-r--r--   0        0        0     3515 2023-04-12 14:27:02.965022 any_api-0.1.0.4/any_api/openapi/model/responses.py
+-rw-r--r--   0        0        0      388 2023-01-10 16:04:06.000000 any_api-0.1.0.4/any_api/openapi/model/util.py
+-rw-r--r--   0        0        0    18433 2023-04-12 14:27:02.973007 any_api-0.1.0.4/any_api/openapi/openapi.py
+-rw-r--r--   0        0        0        0 2022-10-28 10:06:44.000000 any_api-0.1.0.4/any_api/openapi/to/__init__.py
+-rw-r--r--   0        0        0    11232 2023-01-04 16:22:51.000000 any_api-0.1.0.4/any_api/openapi/to/markdown.py
+-rw-r--r--   0        0        0      285 2023-01-09 03:46:58.000000 any_api-0.1.0.4/any_api/openapi/web_ui/__init__.py
+-rw-r--r--   0        0        0     1042 2022-10-25 03:45:48.000000 any_api-0.1.0.4/any_api/openapi/web_ui/elements.py
+-rw-r--r--   0        0        0     1196 2022-10-25 03:54:12.000000 any_api-0.1.0.4/any_api/openapi/web_ui/rapidoc.py
+-rw-r--r--   0        0        0     1021 2022-06-18 16:09:46.000000 any_api-0.1.0.4/any_api/openapi/web_ui/redoc.py
+-rw-r--r--   0        0        0     1285 2022-06-18 16:09:46.000000 any_api-0.1.0.4/any_api/openapi/web_ui/swagger.py
+-rw-r--r--   0        0        0        0 2022-10-28 09:09:27.000000 any_api-0.1.0.4/any_api/util/__init__.py
+-rw-r--r--   0        0        0     8233 2023-04-12 14:48:45.169102 any_api-0.1.0.4/any_api/util/by_pydantic.py
+-rw-r--r--   0        0        0     4297 2022-11-02 11:53:55.000000 any_api-0.1.0.4/any_api/util/i18n.py
+-rw-r--r--   0        0        0      193 2022-10-28 09:09:27.000000 any_api-0.1.0.4/any_api/util/util.py
+-rw-r--r--   0        0        0     1634 2023-05-16 10:09:38.209717 any_api-0.1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 any_api-0.1.0.4/setup.py
+-rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 any_api-0.1.0.4/PKG-INFO
```

### Comparing `any_api-0.1.0.3/LICENSE` & `any_api-0.1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/asyncapi/asyncapi.py` & `any_api-0.1.0.4/any_api/asyncapi/asyncapi.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/asyncapi/model/asyncapi_model.py` & `any_api-0.1.0.4/any_api/asyncapi/model/asyncapi_model.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/asyncapi/model/operation_model.py` & `any_api-0.1.0.4/any_api/asyncapi/model/operation_model.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/base_api/base_api.py` & `any_api-0.1.0.4/any_api/base_api/base_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 from typing import Any, Callable, Dict, Generic, Optional, Tuple, Type, TypeVar
 
 from pydantic import BaseModel
 
 from any_api.base_api.model.base_api_model import BaseAPIModel, BaseSecurityModel
 from any_api.openapi.model.openapi import TagModel
+from any_api.openapi.model.openapi.security import UserScopesOauth2SecurityModel
 from any_api.util import by_pydantic
 
 __all__ = ["BaseAPI"]
 
 _ModelT = TypeVar("_ModelT", bound=BaseAPIModel)
 
 
@@ -27,20 +28,27 @@
                 raise ValueError(
                     f"tag:{tag.name} already exists, but the description of the tag is inconsistent"
                     f" with the current one"
                 )
 
     def _add_security(self, security_model_dict: Dict[str, BaseSecurityModel]) -> None:
         if "securitySchemes" not in self._api_model.components:
-            self._api_model.components["securitySchemes"] = security_model_dict
+            new_security_model_dict: Dict[str, BaseSecurityModel] = {}
+            for security_key, security_model in security_model_dict.items():
+                if isinstance(security_model, UserScopesOauth2SecurityModel):
+                    security_model = security_model.model
+                new_security_model_dict[security_key] = security_model
+            self._api_model.components["securitySchemes"] = new_security_model_dict
         else:
             for security_key, security_model in security_model_dict.items():
+                if isinstance(security_model, UserScopesOauth2SecurityModel):
+                    security_model = security_model.model
                 if security_key in self._api_model.components["securitySchemes"]:
                     if self._api_model.components["securitySchemes"][security_key] != security_model:
-                        raise KeyError(f"{security_key}already exists, and the security model is the same")
+                        raise KeyError(f"{security_key} already exists, and the security model is the same")
                 else:
                     self._api_model.components["securitySchemes"][security_key] = security_model
 
     def _replace_pydantic_definitions(self, schema: dict, parent_schema: Optional[dict] = None) -> None:
         """update schemas'definitions to components schemas"""
         if not parent_schema:
             parent_schema = schema
```

### Comparing `any_api-0.1.0.3/any_api/base_api/model/base_api_model.py` & `any_api-0.1.0.4/any_api/base_api/model/base_api_model.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/openapi/__init__.py` & `any_api-0.1.0.4/any_api/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/openapi/model/__init__.py` & `any_api-0.1.0.4/any_api/openapi/model/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,28 +84,14 @@
 
     @validator("path")
     def validate_path(cls, path: str) -> str:
         if not path.startswith("/"):
             raise ValueError("path must start with `/`")
         return path
 
-    @validator("response_list")
-    def validate_core_response(
-        cls, response_list: List[Union[Type[BaseResponseModel], Tuple[Type[BaseResponseModel]]]]
-    ) -> List[Union[Type[BaseResponseModel], Tuple[Type[BaseResponseModel]]]]:
-        cnt: int = 0
-        for response in response_list:
-            if isinstance(response, tuple):
-                response = response[0]
-            if response.is_core is True:
-                cnt += 1
-        if cnt > 1:
-            raise ValueError("only one core response model")
-        return response_list
-
     def add_to_operation_model(self, openapi_model: OperationModel) -> None:
         pass
 
     @root_validator
     def after_init(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Data association after initializing data"""
         if "request_dict" in values:
```

### Comparing `any_api-0.1.0.3/any_api/openapi/model/links.py` & `any_api-0.1.0.4/any_api/openapi/model/links.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/openapi/model/openapi/__init__.py` & `any_api-0.1.0.4/any_api/openapi/model/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/openapi/model/openapi/basic.py` & `any_api-0.1.0.4/any_api/openapi/model/openapi/basic.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/openapi/model/openapi/info.py` & `any_api-0.1.0.4/any_api/openapi/model/openapi/info.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/openapi/model/openapi/security.py` & `any_api-0.1.0.4/any_api/openapi/model/openapi/security.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,14 +94,35 @@
             scope_list.extend(self.flows.implicit.scopes.keys())
 
         if self.flows.password:
             scope_list.extend(self.flows.password.scopes.keys())
         return scope_list
 
 
+class UserScopesOauth2SecurityModel(Oauth2SecurityModel):
+    use_scopes: List[str] = Field(description="Scope for the real use Oauth2SecurityModel", default_factory=list)
+    model: Oauth2SecurityModel = Field(description="Parent Oauth2SecurityModel")
+
+    @root_validator(pre=True)
+    def set_type(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+        model: Oauth2SecurityModel = values["model"]
+        values["flows"] = model.flows
+        all_scopes = model.get_security_scope()
+        scopes = values["use_scopes"]
+        _scopes_set = set(scopes) - set(all_scopes)
+        if len(_scopes_set) > 0:
+            raise ValueError(f"{_scopes_set} not in {all_scopes}")
+        return values
+
+    def get_security_scope(self) -> List[str]:
+        if self.use_scopes:
+            return self.use_scopes
+        return self.model.get_security_scope()
+
+
 class HttpSecurityModel(BaseSecurityModel):
     scheme: str = Field(
         description=(
             "The name of the HTTP Authorization scheme to be used in the Authorization header as defined in RFC7235. "
             "The values used SHOULD be registered in the IANA Authentication Scheme registry."
         )
     )
```

### Comparing `any_api-0.1.0.3/any_api/openapi/model/requests.py` & `any_api-0.1.0.4/any_api/openapi/model/requests.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/openapi/model/responses.py` & `any_api-0.1.0.4/any_api/openapi/model/responses.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,14 @@
 
 _resp_model_class_link_dict: Dict[str, Dict[str, openapi_model.LinkModel]] = {}
 
 
 class BaseResponseModel(object):
     """response model https://swagger.io/docs/specification/describing-responses/"""
 
-    # Used for mock response and response checking to determine if the response model is the core response model
-    is_core: bool = False
-
     # response data
     response_data: Union[Type[BaseModel], str, bytes, None]
     # response media type
     media_type: str = "*/*"
 
     # response name, if the value is empty, the name of the response_data object will be used
     name: Optional[str] = None
```

### Comparing `any_api-0.1.0.3/any_api/openapi/openapi.py` & `any_api-0.1.0.4/any_api/openapi/openapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,26 +236,23 @@
 
     def _response_handle(
         self,
         api_model: ApiModel,
         operation_model: openapi_model.OperationModel,
     ) -> None:
         response_schema_dict: Dict[tuple, List[dict]] = {}
-        core_resp_model: Optional[responses.BaseResponseModel] = None
         response_dict = operation_model.responses
 
         for resp_model_class in api_model.response_list:
             _is_array_response: bool = False
             if isinstance(resp_model_class, tuple):
                 _is_array_response = True
                 resp_model_class = resp_model_class[0]
 
             resp_model: responses.BaseResponseModel = resp_model_class()
-            if core_resp_model is None or core_resp_model.is_core:
-                core_resp_model = resp_model
 
             global_model_name: str = ""
             if (
                 getattr(resp_model, "response_data", None)
                 and isinstance(resp_model.response_data, type)
                 and issubclass(resp_model.response_data, BaseModel)
             ):
```

### Comparing `any_api-0.1.0.3/any_api/openapi/to/markdown.py` & `any_api-0.1.0.4/any_api/openapi/to/markdown.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/openapi/web_ui/elements.py` & `any_api-0.1.0.4/any_api/openapi/web_ui/elements.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/openapi/web_ui/rapidoc.py` & `any_api-0.1.0.4/any_api/openapi/web_ui/rapidoc.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/openapi/web_ui/redoc.py` & `any_api-0.1.0.4/any_api/openapi/web_ui/redoc.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/openapi/web_ui/swagger.py` & `any_api-0.1.0.4/any_api/openapi/web_ui/swagger.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/any_api/util/by_pydantic.py` & `any_api-0.1.0.4/any_api/util/by_pydantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         m_schema = get_schema_ref(model_name, ref_prefix, ref_template, False)  # pragma: no cover
     if m_definitions:
         m_schema.update({"definitions": m_definitions})
     return m_schema
 
 
 def create_pydantic_model(
-    annotation_dict: Dict[str, Tuple[Type, Any]],
+    annotation_dict: Optional[Dict[str, Tuple[Type, Any]]] = None,
     class_name: str = "DynamicModel",
     pydantic_config: Optional[Type["BaseConfig"]] = None,
     pydantic_base: Optional[Type["BaseModel"]] = None,
     pydantic_module: str = "pydantic.main",
     pydantic_validators: Optional[Dict[str, classmethod]] = None,
 ) -> Type["BaseModel"]:
     """pydantic self.pait_response_model helper
@@ -113,15 +113,15 @@
     """
     return create_model(
         class_name,
         __config__=pydantic_config,
         __base__=pydantic_base,
         __module__=pydantic_module,
         __validators__=pydantic_validators,
-        **annotation_dict,
+        **(annotation_dict or {}),
     )
 
 
 json_type_default_value_dict: Dict[str, Any] = {
     "null": None,
     "bool": True,
     "boolean": True,
```

### Comparing `any_api-0.1.0.3/any_api/util/i18n.py` & `any_api-0.1.0.4/any_api/util/i18n.py`

 * *Files identical despite different names*

### Comparing `any_api-0.1.0.3/pyproject.toml` & `any_api-0.1.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "any-api"
-version = "v0.1.0.3"
+version = "v0.1.0.4"
 description = "Quick and easy to create OpenAPI/AsyncAPI, and provide corresponding extensions"
 authors = ["so1n <qaz6803609@163.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pydantic = "^1.9.2"
```

### Comparing `any_api-0.1.0.3/setup.py` & `any_api-0.1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.9.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'any-api',
-    'version': '0.1.0.3',
+    'version': '0.1.0.4',
     'description': 'Quick and easy to create OpenAPI/AsyncAPI, and provide corresponding extensions',
     'long_description': 'None',
     'author': 'so1n',
     'author_email': 'qaz6803609@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `any_api-0.1.0.3/PKG-INFO` & `any_api-0.1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: any-api
-Version: 0.1.0.3
+Version: 0.1.0.4
 Summary: Quick and easy to create OpenAPI/AsyncAPI, and provide corresponding extensions
 License: Apache-2.0
 Author: so1n
 Author-email: qaz6803609@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

