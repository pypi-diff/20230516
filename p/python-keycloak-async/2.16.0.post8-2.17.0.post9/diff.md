# Comparing `tmp/python_keycloak_async-2.16.0.post8.tar.gz` & `tmp/python_keycloak_async-2.17.0.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_keycloak_async-2.16.0.post8.tar", max compression
+gzip compressed data, was "python_keycloak_async-2.17.0.post9.tar", max compression
```

## Comparing `python_keycloak_async-2.16.0.post8.tar` & `python_keycloak_async-2.17.0.post9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     5559 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/CHANGELOG.md
--rw-r--r--   0        0        0     3192 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/CONTRIBUTING.md
--rw-r--r--   0        0        0     1111 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/LICENSE
--rw-r--r--   0        0        0    15646 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/README.md
--rw-r--r--   0        0        0     2428 2023-04-20 06:50:28.320121 python_keycloak_async-2.16.0.post8/pyproject.toml
--rw-r--r--   0        0        0     2381 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/__init__.py
--rw-r--r--   0        0        0     1197 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/_version.py
--rw-r--r--   0        0        0     3748 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/authorization/__init__.py
--rw-r--r--   0        0        0     4421 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/authorization/permission.py
--rw-r--r--   0        0        0     5252 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/authorization/policy.py
--rw-r--r--   0        0        0     2306 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/authorization/role.py
--rw-r--r--   0        0        0     9292 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/connection.py
--rw-r--r--   0        0        0     5469 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/exceptions.py
--rw-r--r--   0        0        0   150157 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/keycloak_admin.py
--rw-r--r--   0        0        0    25578 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/keycloak_openid.py
--rw-r--r--   0        0        0    15826 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/keycloak_uma.py
--rw-r--r--   0        0        0    12915 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/openid_connection.py
--rw-r--r--   0        0        0     8755 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/uma_permissions.py
--rw-r--r--   0        0        0    11715 2023-04-20 06:50:07.131828 python_keycloak_async-2.16.0.post8/src/keycloak/urls_patterns.py
--rw-r--r--   0        0        0    17449 1970-01-01 00:00:00.000000 python_keycloak_async-2.16.0.post8/PKG-INFO
+-rw-r--r--   0        0        0     5911 2023-05-16 02:57:49.557041 python_keycloak_async-2.17.0.post9/CHANGELOG.md
+-rw-r--r--   0        0        0     3192 2023-05-16 02:57:49.557041 python_keycloak_async-2.17.0.post9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1111 2023-05-16 02:57:49.557041 python_keycloak_async-2.17.0.post9/LICENSE
+-rw-r--r--   0        0        0    15646 2023-05-16 02:57:49.557041 python_keycloak_async-2.17.0.post9/README.md
+-rw-r--r--   0        0        0     2427 2023-05-16 02:58:12.850563 python_keycloak_async-2.17.0.post9/pyproject.toml
+-rw-r--r--   0        0        0     2381 2023-05-16 02:57:49.561041 python_keycloak_async-2.17.0.post9/src/keycloak/__init__.py
+-rw-r--r--   0        0        0     1197 2023-05-16 02:57:49.561041 python_keycloak_async-2.17.0.post9/src/keycloak/_version.py
+-rw-r--r--   0        0        0     3823 2023-05-16 02:57:49.561041 python_keycloak_async-2.17.0.post9/src/keycloak/authorization/__init__.py
+-rw-r--r--   0        0        0     4421 2023-05-16 02:57:49.561041 python_keycloak_async-2.17.0.post9/src/keycloak/authorization/permission.py
+-rw-r--r--   0        0        0     5252 2023-05-16 02:57:49.561041 python_keycloak_async-2.17.0.post9/src/keycloak/authorization/policy.py
+-rw-r--r--   0        0        0     2306 2023-05-16 02:57:49.561041 python_keycloak_async-2.17.0.post9/src/keycloak/authorization/role.py
+-rw-r--r--   0        0        0     9292 2023-05-16 02:57:49.561041 python_keycloak_async-2.17.0.post9/src/keycloak/connection.py
+-rw-r--r--   0        0        0     5469 2023-05-16 02:57:49.561041 python_keycloak_async-2.17.0.post9/src/keycloak/exceptions.py
+-rw-r--r--   0        0        0   152050 2023-05-16 02:57:49.561041 python_keycloak_async-2.17.0.post9/src/keycloak/keycloak_admin.py
+-rw-r--r--   0        0        0    25578 2023-05-16 02:57:49.561041 python_keycloak_async-2.17.0.post9/src/keycloak/keycloak_openid.py
+-rw-r--r--   0        0        0    15826 2023-05-16 02:57:49.561041 python_keycloak_async-2.17.0.post9/src/keycloak/keycloak_uma.py
+-rw-r--r--   0        0        0    12915 2023-05-16 02:57:49.561041 python_keycloak_async-2.17.0.post9/src/keycloak/openid_connection.py
+-rw-r--r--   0        0        0     8755 2023-05-16 02:57:49.561041 python_keycloak_async-2.17.0.post9/src/keycloak/uma_permissions.py
+-rw-r--r--   0        0        0    11800 2023-05-16 02:57:49.561041 python_keycloak_async-2.17.0.post9/src/keycloak/urls_patterns.py
+-rw-r--r--   0        0        0    17447 1970-01-01 00:00:00.000000 python_keycloak_async-2.17.0.post9/PKG-INFO
```

### Comparing `python_keycloak_async-2.16.0.post8/CHANGELOG.md` & `python_keycloak_async-2.17.0.post9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,24 @@
+## v2.17.0 (2023-05-16)
+
+### Fix
+
+- Fixes `Authorization.load_config` breaking if a scope based permission is linked with anything other than a role based policy. Fixes #445 (#446)
+- issue with app engine reported in #440 (#442)
+
+### Feat
+
+- Add get and delete methods for client authz resources (#435)
+
 ## v2.16.0 (2023-04-20)
 
 ### Refactor
 
 - Migrate to asyncio
+- Initializing KeycloakAdmin without server_url
 
 ## v2.15.3 (2023-04-06)
 
 ### Fix
 
 - Check if _s exists in ConnectionManager before deleting it (#429)
```

### Comparing `python_keycloak_async-2.16.0.post8/CONTRIBUTING.md` & `python_keycloak_async-2.17.0.post9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post8/LICENSE` & `python_keycloak_async-2.17.0.post9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post8/README.md` & `python_keycloak_async-2.17.0.post9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 # Get Certs
 certs = await keycloak_openid.certs()
 
 # Get RPT (Entitlement)
 token = await keycloak_openid.token("user", "password")
 rpt = await keycloak_openid.entitlement(token['access_token'], "resource_id")
 
-# Instropect RPT
+# Introspect RPT
 token_rpt_info = await keycloak_openid.introspect(token['access_token'],
                                                   rpt=rpt['rpt'],
                                                   token_type_hint="requesting_party_token")
 
 # Introspect Token
 token_info = await keycloak_openid.introspect(token['access_token'])
```

### Comparing `python_keycloak_async-2.16.0.post8/pyproject.toml` & `python_keycloak_async-2.17.0.post9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-keycloak-async"
-version = "v2.16.0-8"
+version = "v2.17.0-9"
 description = "python-keycloak-async is a Python package providing access to the Keycloak API."
 license = "MIT"
 readme = "README.md"
 keywords = [ "keycloak", "asyncio", "openid", "oidc" ]
 authors = [
     "Quang Phan <quangpq.uit@gmail.com>",
     "Marcos Pereira <marcospereira.mpj@gmail.com>",
@@ -39,15 +39,15 @@
 commonmark = {version = "^0.9.1", optional = true}
 recommonmark = {version = "^0.7.1", optional = true}
 Sphinx = {version = "^5.3.0", optional = true}
 sphinx-rtd-theme = {version = "^1.0.0", optional = true}
 readthedocs-sphinx-ext = {version = "^2.1.9", optional = true}
 m2r2 = {version = "^0.3.2", optional = true}
 sphinx-autoapi = {version = "^2.0.0", optional = true}
-requests-toolbelt = "^0.10.1"
+requests-toolbelt = "^1.0.0"
 deprecation = "^2.1.0"
 
 [tool.poetry.extras]
 docs = [
     "mock",
     "alabaster",
     "commonmark",
```

### Comparing `python_keycloak_async-2.16.0.post8/src/keycloak/__init__.py` & `python_keycloak_async-2.17.0.post9/src/keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post8/src/keycloak/_version.py` & `python_keycloak_async-2.17.0.post9/src/keycloak/_version.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post8/src/keycloak/authorization/__init__.py` & `python_keycloak_async-2.17.0.post9/src/keycloak/authorization/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,15 +84,16 @@
                     decision_strategy=pol["decisionStrategy"],
                 )
 
                 permission.scopes = ast.literal_eval(pol["config"]["scopes"])
 
                 if "applyPolicies" in pol["config"]:
                     for policy_name in ast.literal_eval(pol["config"]["applyPolicies"]):
-                        self.policies[policy_name].add_permission(permission)
+                        if self.policies.get(policy_name) is not None:
+                            self.policies[policy_name].add_permission(permission)
 
             if pol["type"] == "resource":
                 permission = Permission(
                     name=pol["name"],
                     type=pol["type"],
                     logic=pol["logic"],
                     decision_strategy=pol["decisionStrategy"],
```

### Comparing `python_keycloak_async-2.16.0.post8/src/keycloak/authorization/permission.py` & `python_keycloak_async-2.17.0.post9/src/keycloak/authorization/permission.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post8/src/keycloak/authorization/policy.py` & `python_keycloak_async-2.17.0.post9/src/keycloak/authorization/policy.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post8/src/keycloak/authorization/role.py` & `python_keycloak_async-2.17.0.post9/src/keycloak/authorization/role.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post8/src/keycloak/connection.py` & `python_keycloak_async-2.17.0.post9/src/keycloak/connection.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post8/src/keycloak/exceptions.py` & `python_keycloak_async-2.17.0.post9/src/keycloak/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post8/src/keycloak/keycloak_admin.py` & `python_keycloak_async-2.17.0.post9/src/keycloak/keycloak_admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,18 +25,15 @@
 # internal Keycloak server ID, usually a uuid string
 
 """The keycloak admin module."""
 
 from builtins import isinstance
 from typing import Optional
 
-import deprecation
-
 from . import urls_patterns
-from ._version import __version__
 from .exceptions import (
     KeycloakDeleteError,
     KeycloakError,
     KeycloakGetError,
     KeycloakPostError,
     KeycloakPutError,
     raise_error_from_response,
@@ -151,15 +148,15 @@
             custom_headers=custom_headers,
             timeout=timeout,
         )
         if auto_refresh_token is not None:
             self.auto_refresh_token = auto_refresh_token
         if token is not None:
             self.connection.headers = {
-                "Authorization": "Bearer " + self.token.get("access_token"),
+                "Authorization": "Bearer " + token.get("access_token"),
                 "Content-Type": "application/json",
             }
 
     async def __aenter__(self):
         await self.init_token()
         return self
 
@@ -1025,15 +1022,15 @@
 
         :param path: group path
         :type path: str
         :return: Keycloak server response (GroupRepresentation)
         :rtype: dict
         """
         params_path = {"realm-name": self.connection.realm_name, "path": path}
-        data_raw = await self.raw_get(urls_patterns.URL_ADMIN_GROUP_BY_PATH.format(**params_path))
+        data_raw = await self.connection.raw_get(urls_patterns.URL_ADMIN_GROUP_BY_PATH.format(**params_path))
         return raise_error_from_response(data_raw, KeycloakGetError)
 
     async def create_group(self, payload, parent=None, skip_exists=False):
         """Create a group in the Realm.
 
         GroupRepresentation
         https://www.keycloak.org/docs-api/18.0/rest-api/#_grouprepresentation
@@ -1244,29 +1241,75 @@
             urls_patterns.URL_ADMIN_CLIENT_AUTHZ_RESOURCES.format(**params_path),
             json=payload,
         )
         return raise_error_from_response(
             data_raw, KeycloakPostError, expected_codes=[201], skip_exists=skip_exists
         )
 
+    async def delete_client_authz_resource(self, client_id: str, resource_id: str):
+        """Delete a client resource.
+
+        :param client_id: id in ClientRepresentation
+            https://www.keycloak.org/docs-api/18.0/rest-api/index.html#_clientrepresentation
+        :type client_id: str
+        :param resource_id: id in ResourceRepresentation
+            https://www.keycloak.org/docs-api/18.0/rest-api/index.html#_resourcerepresentation
+        :type resource_id: str
+
+        :return: Keycloak server response
+        :rtype: bytes
+        """
+        params_path = {
+            "realm-name": self.connection.realm_name,
+            "id": client_id,
+            "resource-id": resource_id,
+        }
+        data_raw = await self.connection.raw_delete(
+            urls_patterns.URL_ADMIN_CLIENT_AUTHZ_RESOURCE.format(**params_path)
+        )
+        return raise_error_from_response(data_raw, KeycloakDeleteError, expected_codes=[204])
+
     async def get_client_authz_resources(self, client_id):
         """Get resources from client.
 
         :param client_id: id in ClientRepresentation
             https://www.keycloak.org/docs-api/18.0/rest-api/index.html#_clientrepresentation
         :type client_id: str
-        :return: Keycloak server response
-        :rtype: dict
+        :return: Keycloak server response (ResourceRepresentation)
+        :rtype: list
         """
         params_path = {"realm-name": self.connection.realm_name, "id": client_id}
         data_raw = await self.connection.raw_get(
             urls_patterns.URL_ADMIN_CLIENT_AUTHZ_RESOURCES.format(**params_path)
         )
         return raise_error_from_response(data_raw, KeycloakGetError)
 
+    async def get_client_authz_resource(self, client_id: str, resource_id: str):
+        """Get a client resource.
+
+        :param client_id: id in ClientRepresentation
+            https://www.keycloak.org/docs-api/18.0/rest-api/index.html#_clientrepresentation
+        :type client_id: str
+        :param resource_id: id in ResourceRepresentation
+            https://www.keycloak.org/docs-api/18.0/rest-api/index.html#_resourcerepresentation
+        :type resource_id: str
+
+        :return: Keycloak server response (ResourceRepresentation)
+        :rtype: dict
+        """
+        params_path = {
+            "realm-name": self.connection.realm_name,
+            "id": client_id,
+            "resource-id": resource_id,
+        }
+        data_raw = await self.connection.raw_get(
+            urls_patterns.URL_ADMIN_CLIENT_AUTHZ_RESOURCE.format(**params_path)
+        )
+        return raise_error_from_response(data_raw, KeycloakGetError, expected_codes=[200])
+
     async def create_client_authz_role_based_policy(self, client_id, payload, skip_exists=False):
         """Create role-based policy of client.
 
         Payload example::
 
             payload={
                 "type": "role",
```

### Comparing `python_keycloak_async-2.16.0.post8/src/keycloak/keycloak_openid.py` & `python_keycloak_async-2.17.0.post9/src/keycloak/keycloak_openid.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post8/src/keycloak/keycloak_uma.py` & `python_keycloak_async-2.17.0.post9/src/keycloak/keycloak_uma.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post8/src/keycloak/openid_connection.py` & `python_keycloak_async-2.17.0.post9/src/keycloak/openid_connection.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post8/src/keycloak/uma_permissions.py` & `python_keycloak_async-2.17.0.post9/src/keycloak/uma_permissions.py`

 * *Files identical despite different names*

### Comparing `python_keycloak_async-2.16.0.post8/src/keycloak/urls_patterns.py` & `python_keycloak_async-2.17.0.post9/src/keycloak/urls_patterns.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 URL_ADMIN_CLIENT_DEFAULT_CLIENT_SCOPES = URL_ADMIN_CLIENT + "/default-client-scopes"
 URL_ADMIN_CLIENT_DEFAULT_CLIENT_SCOPE = (
     URL_ADMIN_CLIENT_DEFAULT_CLIENT_SCOPES + "/{client_scope_id}"
 )
 
 URL_ADMIN_CLIENT_AUTHZ = URL_ADMIN_CLIENT + "/authz/resource-server"
 URL_ADMIN_CLIENT_AUTHZ_SETTINGS = URL_ADMIN_CLIENT_AUTHZ + "/settings"
+URL_ADMIN_CLIENT_AUTHZ_RESOURCE = URL_ADMIN_CLIENT_AUTHZ + "/resource/{resource-id}"
 URL_ADMIN_CLIENT_AUTHZ_RESOURCES = URL_ADMIN_CLIENT_AUTHZ + "/resource?max=-1"
 URL_ADMIN_CLIENT_AUTHZ_SCOPES = URL_ADMIN_CLIENT_AUTHZ + "/scope?max=-1"
 URL_ADMIN_CLIENT_AUTHZ_PERMISSIONS = URL_ADMIN_CLIENT_AUTHZ + "/permission?max=-1"
 URL_ADMIN_CLIENT_AUTHZ_POLICIES = URL_ADMIN_CLIENT_AUTHZ + "/policy?max=-1&permission=false"
 URL_ADMIN_CLIENT_AUTHZ_ROLE_BASED_POLICY = URL_ADMIN_CLIENT_AUTHZ + "/policy/role?max=-1"
 URL_ADMIN_CLIENT_AUTHZ_RESOURCE_BASED_PERMISSION = (
     URL_ADMIN_CLIENT_AUTHZ + "/permission/resource?max=-1"
```

### Comparing `python_keycloak_async-2.16.0.post8/PKG-INFO` & `python_keycloak_async-2.17.0.post9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-keycloak-async
-Version: 2.16.0.post8
+Version: 2.17.0.post9
 Summary: python-keycloak-async is a Python package providing access to the Keycloak API.
 License: MIT
 Keywords: keycloak,asyncio,openid,oidc
 Author: Quang Phan
 Author-email: quangpq.uit@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -26,15 +26,15 @@
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: m2r2 (>=0.3.2,<0.4.0) ; extra == "docs"
 Requires-Dist: mock (>=4.0.3,<5.0.0) ; extra == "docs"
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: readthedocs-sphinx-ext (>=2.1.9,<3.0.0) ; extra == "docs"
 Requires-Dist: recommonmark (>=0.7.1,<0.8.0) ; extra == "docs"
-Requires-Dist: requests-toolbelt (>=0.10.1,<0.11.0)
+Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: sphinx-autoapi (>=2.0.0,<3.0.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0) ; extra == "docs"
 Project-URL: Documentation, https://github.com/quangpq/python-keycloak-async
 Project-URL: Issue tracker, https://github.com/quangpq/python-keycloak-async/issues
 Description-Content-Type: text/markdown
 
 # Python Keycloak Async
@@ -146,15 +146,15 @@
 # Get Certs
 certs = await keycloak_openid.certs()
 
 # Get RPT (Entitlement)
 token = await keycloak_openid.token("user", "password")
 rpt = await keycloak_openid.entitlement(token['access_token'], "resource_id")
 
-# Instropect RPT
+# Introspect RPT
 token_rpt_info = await keycloak_openid.introspect(token['access_token'],
                                                   rpt=rpt['rpt'],
                                                   token_type_hint="requesting_party_token")
 
 # Introspect Token
 token_info = await keycloak_openid.introspect(token['access_token'])
```

