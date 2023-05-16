# Comparing `tmp/frontegg-2.1.3.tar.gz` & `tmp/frontegg-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontegg-2.1.3.tar", max compression
+gzip compressed data, was "frontegg-2.1.4.tar", max compression
```

## Comparing `frontegg-2.1.3.tar` & `frontegg-2.1.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1065 2022-10-13 14:59:50.240636 frontegg-2.1.3/LICENSE
--rw-r--r--   0        0        0      406 2023-02-02 10:01:16.057919 frontegg-2.1.3/README-PYPI.rst
--rw-r--r--   0        0        0      213 2022-12-11 12:48:40.494240 frontegg-2.1.3/frontegg/__init__.py
--rw-r--r--   0        0        0      243 2022-12-11 12:48:40.494450 frontegg-2.1.3/frontegg/common/__init__.py
--rw-r--r--   0        0        0      489 2023-02-02 10:01:22.637222 frontegg-2.1.3/frontegg/common/cache/cache_manager.py
--rw-r--r--   0        0        0     1206 2023-02-02 10:01:22.637491 frontegg-2.1.3/frontegg/common/cache/local_cache_manager.py
--rw-r--r--   0        0        0     1147 2023-02-02 10:01:22.637710 frontegg-2.1.3/frontegg/common/cache/redis_cache_manager.py
--rw-r--r--   0        0        0      202 2022-12-11 12:48:40.494652 frontegg-2.1.3/frontegg/common/clients/__init__.py
--rw-r--r--   0        0        0     1738 2022-12-11 12:48:40.494799 frontegg-2.1.3/frontegg/common/clients/audits_client.py
--rw-r--r--   0        0        0     3232 2022-12-11 12:48:40.494939 frontegg-2.1.3/frontegg/common/clients/http_client.py
--rw-r--r--   0        0        0     4312 2023-02-02 10:01:22.638043 frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_resolver.py
--rw-r--r--   0        0        0      702 2023-02-02 10:01:22.638337 frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py
--rw-r--r--   0        0        0     2623 2023-02-02 10:01:22.638653 frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py
--rw-r--r--   0        0        0      985 2023-02-02 10:01:22.638891 frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py
--rw-r--r--   0        0        0      989 2023-02-02 10:01:22.639121 frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py
--rw-r--r--   0        0        0     1626 2023-02-02 10:01:22.639423 frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py
--rw-r--r--   0        0        0     1328 2023-02-02 10:01:22.639638 frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py
--rw-r--r--   0        0        0     1202 2023-02-02 10:01:22.639846 frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py
--rw-r--r--   0        0        0      968 2023-02-02 10:01:22.640079 frontegg-2.1.3/frontegg/common/clients/token_resolvers/authorization_header_resolver.py
--rw-r--r--   0        0        0     3563 2023-02-02 10:01:22.640311 frontegg-2.1.3/frontegg/common/clients/token_resolvers/token_resolver.py
--rw-r--r--   0        0        0     1352 2023-02-02 10:01:22.640525 frontegg-2.1.3/frontegg/common/clients/types.py
--rw-r--r--   0        0        0     1712 2022-12-11 12:48:40.495077 frontegg-2.1.3/frontegg/common/frontegg_authenticator.py
--rw-r--r--   0        0        0      351 2022-12-11 12:48:40.495204 frontegg-2.1.3/frontegg/common/frontegg_config.py
--rw-r--r--   0        0        0     1457 2023-02-02 10:01:22.640739 frontegg-2.1.3/frontegg/common/frontegg_context.py
--rw-r--r--   0        0        0     4225 2023-02-02 10:01:22.641738 frontegg-2.1.3/frontegg/common/identity_mixin.py
--rw-r--r--   0        0        0      250 2023-02-02 10:01:22.642005 frontegg-2.1.3/frontegg/common/package_utils.py
--rw-r--r--   0        0        0     4247 2023-03-22 13:04:42.099164 frontegg-2.1.3/frontegg/fastapi/README.md
--rw-r--r--   0        0        0       53 2022-10-13 14:59:50.242552 frontegg-2.1.3/frontegg/fastapi/__init__.py
--rw-r--r--   0        0        0     1620 2023-03-22 13:04:42.099816 frontegg-2.1.3/frontegg/fastapi/frontegg.py
--rw-r--r--   0        0        0      152 2022-12-11 12:48:40.497018 frontegg-2.1.3/frontegg/fastapi/secure_access/__init__.py
--rw-r--r--   0        0        0     4709 2023-03-22 13:04:42.100462 frontegg-2.1.3/frontegg/fastapi/secure_access/frontegg_security.py
--rw-r--r--   0        0        0     4164 2023-03-22 13:04:42.101047 frontegg-2.1.3/frontegg/flask/README.md
--rw-r--r--   0        0        0       53 2022-12-11 12:48:40.497924 frontegg-2.1.3/frontegg/flask/__init__.py
--rw-r--r--   0        0        0     1620 2023-03-22 13:04:42.101711 frontegg-2.1.3/frontegg/flask/frontegg.py
--rw-r--r--   0        0        0       86 2022-12-11 12:48:40.498654 frontegg-2.1.3/frontegg/flask/secure_access/__init__.py
--rw-r--r--   0        0        0     1820 2023-02-02 10:01:22.644681 frontegg-2.1.3/frontegg/flask/secure_access/with_authentication.py
--rw-r--r--   0        0        0      589 2022-12-11 12:48:40.499555 frontegg-2.1.3/frontegg/helpers/exceptions.py
--rw-r--r--   0        0        0     1669 2023-03-22 13:05:39.187041 frontegg-2.1.3/frontegg/helpers/frontegg_urls.py
--rw-r--r--   0        0        0      295 2022-10-13 14:59:50.243962 frontegg-2.1.3/frontegg/helpers/logger.py
--rw-r--r--   0        0        0      984 2022-12-11 12:48:40.500433 frontegg-2.1.3/frontegg/helpers/retry.py
--rw-r--r--   0        0        0     1582 2023-03-22 13:09:54.859746 frontegg-2.1.3/pyproject.toml
--rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 frontegg-2.1.3/setup.py
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 frontegg-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-10-13 14:59:50.240636 frontegg-2.1.4/LICENSE
+-rw-r--r--   0        0        0      406 2023-02-02 10:01:16.057919 frontegg-2.1.4/README-PYPI.rst
+-rw-r--r--   0        0        0      213 2022-12-11 12:48:40.494240 frontegg-2.1.4/frontegg/__init__.py
+-rw-r--r--   0        0        0      243 2022-12-11 12:48:40.494450 frontegg-2.1.4/frontegg/common/__init__.py
+-rw-r--r--   0        0        0      489 2023-02-02 10:01:22.637222 frontegg-2.1.4/frontegg/common/cache/cache_manager.py
+-rw-r--r--   0        0        0     1206 2023-02-02 10:01:22.637491 frontegg-2.1.4/frontegg/common/cache/local_cache_manager.py
+-rw-r--r--   0        0        0     1147 2023-02-02 10:01:22.637710 frontegg-2.1.4/frontegg/common/cache/redis_cache_manager.py
+-rw-r--r--   0        0        0      202 2022-12-11 12:48:40.494652 frontegg-2.1.4/frontegg/common/clients/__init__.py
+-rw-r--r--   0        0        0     1738 2022-12-11 12:48:40.494799 frontegg-2.1.4/frontegg/common/clients/audits_client.py
+-rw-r--r--   0        0        0     3232 2022-12-11 12:48:40.494939 frontegg-2.1.4/frontegg/common/clients/http_client.py
+-rw-r--r--   0        0        0     4338 2023-05-16 15:25:53.376931 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_resolver.py
+-rw-r--r--   0        0        0      702 2023-02-02 10:01:22.638337 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py
+-rw-r--r--   0        0        0     2658 2023-05-16 15:25:53.377590 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py
+-rw-r--r--   0        0        0      985 2023-02-02 10:01:22.638891 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py
+-rw-r--r--   0        0        0      989 2023-02-02 10:01:22.639121 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py
+-rw-r--r--   0        0        0     1626 2023-02-02 10:01:22.639423 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py
+-rw-r--r--   0        0        0     1328 2023-02-02 10:01:22.639638 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py
+-rw-r--r--   0        0        0     1202 2023-02-02 10:01:22.639846 frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py
+-rw-r--r--   0        0        0      968 2023-02-02 10:01:22.640079 frontegg-2.1.4/frontegg/common/clients/token_resolvers/authorization_header_resolver.py
+-rw-r--r--   0        0        0     3563 2023-02-02 10:01:22.640311 frontegg-2.1.4/frontegg/common/clients/token_resolvers/token_resolver.py
+-rw-r--r--   0        0        0     1352 2023-02-02 10:01:22.640525 frontegg-2.1.4/frontegg/common/clients/types.py
+-rw-r--r--   0        0        0     1712 2022-12-11 12:48:40.495077 frontegg-2.1.4/frontegg/common/frontegg_authenticator.py
+-rw-r--r--   0        0        0      351 2022-12-11 12:48:40.495204 frontegg-2.1.4/frontegg/common/frontegg_config.py
+-rw-r--r--   0        0        0     1518 2023-05-16 15:29:09.508464 frontegg-2.1.4/frontegg/common/frontegg_context.py
+-rw-r--r--   0        0        0     4225 2023-02-02 10:01:22.641738 frontegg-2.1.4/frontegg/common/identity_mixin.py
+-rw-r--r--   0        0        0      250 2023-02-02 10:01:22.642005 frontegg-2.1.4/frontegg/common/package_utils.py
+-rw-r--r--   0        0        0     4247 2023-03-22 13:04:42.099164 frontegg-2.1.4/frontegg/fastapi/README.md
+-rw-r--r--   0        0        0       53 2022-10-13 14:59:50.242552 frontegg-2.1.4/frontegg/fastapi/__init__.py
+-rw-r--r--   0        0        0     1620 2023-03-22 13:04:42.099816 frontegg-2.1.4/frontegg/fastapi/frontegg.py
+-rw-r--r--   0        0        0      152 2022-12-11 12:48:40.497018 frontegg-2.1.4/frontegg/fastapi/secure_access/__init__.py
+-rw-r--r--   0        0        0     4689 2023-05-16 15:29:09.509024 frontegg-2.1.4/frontegg/fastapi/secure_access/frontegg_security.py
+-rw-r--r--   0        0        0     4164 2023-03-22 13:04:42.101047 frontegg-2.1.4/frontegg/flask/README.md
+-rw-r--r--   0        0        0       53 2022-12-11 12:48:40.497924 frontegg-2.1.4/frontegg/flask/__init__.py
+-rw-r--r--   0        0        0     1620 2023-03-22 13:04:42.101711 frontegg-2.1.4/frontegg/flask/frontegg.py
+-rw-r--r--   0        0        0       86 2022-12-11 12:48:40.498654 frontegg-2.1.4/frontegg/flask/secure_access/__init__.py
+-rw-r--r--   0        0        0     1820 2023-02-02 10:01:22.644681 frontegg-2.1.4/frontegg/flask/secure_access/with_authentication.py
+-rw-r--r--   0        0        0      589 2022-12-11 12:48:40.499555 frontegg-2.1.4/frontegg/helpers/exceptions.py
+-rw-r--r--   0        0        0     1669 2023-03-22 13:05:39.187041 frontegg-2.1.4/frontegg/helpers/frontegg_urls.py
+-rw-r--r--   0        0        0      295 2022-10-13 14:59:50.243962 frontegg-2.1.4/frontegg/helpers/logger.py
+-rw-r--r--   0        0        0      984 2022-12-11 12:48:40.500433 frontegg-2.1.4/frontegg/helpers/retry.py
+-rw-r--r--   0        0        0     1582 2023-05-16 15:36:46.754671 frontegg-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 frontegg-2.1.4/setup.py
+-rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 frontegg-2.1.4/PKG-INFO
```

### Comparing `frontegg-2.1.3/LICENSE` & `frontegg-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/common/cache/local_cache_manager.py` & `frontegg-2.1.4/frontegg/common/cache/local_cache_manager.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/common/cache/redis_cache_manager.py` & `frontegg-2.1.4/frontegg/common/cache/redis_cache_manager.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/common/clients/audits_client.py` & `frontegg-2.1.4/frontegg/common/clients/audits_client.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/common/clients/http_client.py` & `frontegg-2.1.4/frontegg/common/clients/http_client.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_resolver.py` & `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
         if options is not None and ((options.get('permissions') is not None and len(options.get('permissions')) > 0) or
                                     (options.get('roles') is not None and len(options.get('roles')) > 0)):
             entity_with_roles = self.get_entity(entity)
             self.validate_roles_and_permissions(entity_with_roles, options)
         else:
             active_ids = self.__get_active_access_token_ids(entity)
-            if entity.get('sub') not in active_ids:
+            if active_ids is None or entity.get('sub') not in active_ids:
                 raise UnauthenticatedException()
 
         return {**entity_with_roles, **entity}
 
     def get_entity(self, entity: IEntityWithRoles) -> List[str]:
         service = self.__get_active_access_token_service(entity.get('type'))
 
@@ -51,15 +51,15 @@
 
     def __get_active_access_token_service(self, type: TokenTypes):
         resolver = None
         for _resolver in self.__access_token_services:
             if _resolver.should_handle(type):
                 resolver = _resolver
                 break
-        if not resolver:
+        if resolver is None:
             logger.error("Failed to find token resolver")
             raise UnauthenticatedException()
 
         return resolver
 
     def __init_access_token_services(self, authenticator: FronteggAuthenticator):
         http_client = HttpClient(authenticator.client_id, authenticator.api_key, '')
```

### Comparing `frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py` & `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py` & `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,23 +40,25 @@
         except UnauthenticatedException:
             self.entity_cache_manager.set(cache_key, {'empty': True}, {'expires_in_seconds': 10})
 
     def get_active_access_token_ids(self) -> List[str]:
         cache_key = self.get_cache_prefix() + '_ids'
         cached_data = self.active_access_tokens_cache_manager.get(cache_key)
 
-        if cached_data:
+        if cached_data is not None:
             return cached_data
 
         try:
             data = self.access_token_service.get_active_access_token_ids()
             self.active_access_tokens_cache_manager.set(cache_key, data, {'expires_in_seconds': 10})
 
             return data
         except UnauthenticatedException:
             self.active_access_tokens_cache_manager.set(cache_key, [], {'expires_in_seconds': 10})
 
+            return []
+
     def __is_empty_access_token(self, access_token) -> bool:
         return 'empty' in access_token and access_token['empty'] is True
     @abc.abstractmethod
     def get_cache_prefix(self, access_token) -> str:
         pass
```

### Comparing `frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py` & `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py` & `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py` & `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py` & `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py` & `frontegg-2.1.4/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/common/clients/token_resolvers/authorization_header_resolver.py` & `frontegg-2.1.4/frontegg/common/clients/token_resolvers/authorization_header_resolver.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/common/clients/token_resolvers/token_resolver.py` & `frontegg-2.1.4/frontegg/common/clients/token_resolvers/token_resolver.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/common/clients/types.py` & `frontegg-2.1.4/frontegg/common/clients/types.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/common/frontegg_authenticator.py` & `frontegg-2.1.4/frontegg/common/frontegg_authenticator.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/common/frontegg_context.py` & `frontegg-2.1.4/frontegg/common/frontegg_context.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from frontegg.common.package_utils import PackageUtils
-
+from frontegg.helpers.logger import logger
 
 class FronteggContext(object):
     _instance = None
     options = {}
 
     def __new__(cls):
         if cls._instance is None:
-            print('Creating the object')
+            logger.debug('Creating a new frontegg context')
             cls._instance = super(FronteggContext, cls).__new__(cls)
             # Put any initialization here.
         return cls._instance
 
     @staticmethod
     def init(options={}):
         FronteggContext().__validate_options(options)
```

### Comparing `frontegg-2.1.3/frontegg/common/identity_mixin.py` & `frontegg-2.1.4/frontegg/common/identity_mixin.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/fastapi/README.md` & `frontegg-2.1.4/frontegg/fastapi/README.md`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/fastapi/frontegg.py` & `frontegg-2.1.4/frontegg/fastapi/frontegg.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/fastapi/secure_access/frontegg_security.py` & `frontegg-2.1.4/frontegg/fastapi/secure_access/frontegg_security.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,15 @@
             return User(**decoded_user, access_token=auth_header.get('token'))
 
         except UnauthorizedException:
             logger.info('entity does not have required role and permissions')
             raise HTTPException(status_code=403, detail='You do not have permission to perform this action.')
 
         except Exception as e:
-            print(e)
-            logger.info('something went wrong while validating JWT, ' + str(e))
+            logger.error('something went wrong while validating JWT, ' + str(e))
             return self.handle_authentication_failure()
 
 
 def FronteggSecurity(permissions: List[str] = None, auto_error: bool = True, roles: List[str] = None):  # noqa
     """
     This factory function will create authentication dependency for FastAPI,
     and will ensure the user has the right permissions if specified.
```

### Comparing `frontegg-2.1.3/frontegg/flask/README.md` & `frontegg-2.1.4/frontegg/flask/README.md`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/flask/frontegg.py` & `frontegg-2.1.4/frontegg/flask/frontegg.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/flask/secure_access/with_authentication.py` & `frontegg-2.1.4/frontegg/flask/secure_access/with_authentication.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/helpers/exceptions.py` & `frontegg-2.1.4/frontegg/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/helpers/frontegg_urls.py` & `frontegg-2.1.4/frontegg/helpers/frontegg_urls.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/frontegg/helpers/retry.py` & `frontegg-2.1.4/frontegg/helpers/retry.py`

 * *Files identical despite different names*

### Comparing `frontegg-2.1.3/pyproject.toml` & `frontegg-2.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frontegg"
-version = "2.1.3"
+version = "2.1.4"
 description = "Frontegg is a web platform where SaaS companies can set up their fully managed, scalable and brand aware - SaaS features and integrate them into their SaaS portals in up to 5 lines of code."
 homepage = "https://frontegg.com/"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `frontegg-2.1.3/setup.py` & `frontegg-2.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'typing-extensions>=4.4.0,<5.0.0']
 
 extras_require = \
 {'fastapi': ['fastapi'], 'flask': ['flask>=1.0,<2.0']}
 
 setup_kwargs = {
     'name': 'frontegg',
-    'version': '2.1.3',
+    'version': '2.1.4',
     'description': 'Frontegg is a web platform where SaaS companies can set up their fully managed, scalable and brand aware - SaaS features and integrate them into their SaaS portals in up to 5 lines of code.',
     'long_description': '.. image:: https://fronteggstuff.blob.core.windows.net/frongegg-logos/logo-transparent.png\n   :alt: Frontegg\n\nFrontegg is a web platform where SaaS companies can set up their fully managed, scalable and brand aware - SaaS features and integrate them into their SaaS portals in up to 5 lines of code.\n\nFor more information and usage you can visit the `github repo <https://github.com/frontegg/python-sdk>`_.',
     'author': 'Frontegg LTD',
     'author_email': 'hello@frontegg.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://frontegg.com/',
```

### Comparing `frontegg-2.1.3/PKG-INFO` & `frontegg-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontegg
-Version: 2.1.3
+Version: 2.1.4
 Summary: Frontegg is a web platform where SaaS companies can set up their fully managed, scalable and brand aware - SaaS features and integrate them into their SaaS portals in up to 5 lines of code.
 Home-page: https://frontegg.com/
 Author: Frontegg LTD
 Author-email: hello@frontegg.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

