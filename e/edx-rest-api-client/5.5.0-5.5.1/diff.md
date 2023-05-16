# Comparing `tmp/edx-rest-api-client-5.5.0.tar.gz` & `tmp/edx-rest-api-client-5.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-rest-api-client-5.5.0.tar", last modified: Thu Jan 20 11:10:22 2022, max compression
+gzip compressed data, was "edx-rest-api-client-5.5.1.tar", last modified: Tue May 16 12:28:12 2023, max compression
```

## Comparing `edx-rest-api-client-5.5.0.tar` & `edx-rest-api-client-5.5.1.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 11:10:22.314582 edx-rest-api-client-5.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-01-20 11:10:19.000000 edx-rest-api-client-5.5.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-01-20 11:10:19.000000 edx-rest-api-client-5.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-01-20 11:10:19.000000 edx-rest-api-client-5.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4049 2022-01-20 11:10:22.314582 edx-rest-api-client-5.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3267 2022-01-20 11:10:19.000000 edx-rest-api-client-5.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 11:10:22.314582 edx-rest-api-client-5.5.0/edx_rest_api_client/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-01-20 11:10:19.000000 edx-rest-api-client-5.5.0/edx_rest_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-20 11:10:19.000000 edx-rest-api-client-5.5.0/edx_rest_api_client/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2694 2022-01-20 11:10:19.000000 edx-rest-api-client-5.5.0/edx_rest_api_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)    13349 2022-01-20 11:10:19.000000 edx-rest-api-client-5.5.0/edx_rest_api_client/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-01-20 11:10:19.000000 edx-rest-api-client-5.5.0/edx_rest_api_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 11:10:22.314582 edx-rest-api-client-5.5.0/edx_rest_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4049 2022-01-20 11:10:22.000000 edx-rest-api-client-5.5.0/edx_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-01-20 11:10:22.000000 edx-rest-api-client-5.5.0/edx_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-20 11:10:22.000000 edx-rest-api-client-5.5.0/edx_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-01-20 11:10:22.000000 edx-rest-api-client-5.5.0/edx_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-20 11:10:22.000000 edx-rest-api-client-5.5.0/edx_rest_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-20 11:10:22.314582 edx-rest-api-client-5.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-01-20 11:10:19.000000 edx-rest-api-client-5.5.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-01-20 11:10:19.000000 edx-rest-api-client-5.5.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-20 11:10:22.314582 edx-rest-api-client-5.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4420 2022-01-20 11:10:19.000000 edx-rest-api-client-5.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 12:28:12.198991 edx-rest-api-client-5.5.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5636 2023-05-16 12:28:12.198991 edx-rest-api-client-5.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4890 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 12:28:12.198991 edx-rest-api-client-5.5.1/edx_rest_api_client/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/edx_rest_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/edx_rest_api_client/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/edx_rest_api_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13817 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/edx_rest_api_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/edx_rest_api_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 12:28:12.198991 edx-rest-api-client-5.5.1/edx_rest_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5636 2023-05-16 12:28:12.000000 edx-rest-api-client-5.5.1/edx_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-05-16 12:28:12.000000 edx-rest-api-client-5.5.1/edx_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 12:28:12.000000 edx-rest-api-client-5.5.1/edx_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-16 12:28:12.000000 edx-rest-api-client-5.5.1/edx_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-16 12:28:12.000000 edx-rest-api-client-5.5.1/edx_rest_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 12:28:12.198991 edx-rest-api-client-5.5.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 12:28:12.198991 edx-rest-api-client-5.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4427 2023-05-16 12:28:07.000000 edx-rest-api-client-5.5.1/setup.py
```

### Comparing `edx-rest-api-client-5.5.0/LICENSE` & `edx-rest-api-client-5.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-rest-api-client-5.5.0/edx_rest_api_client/auth.py` & `edx-rest-api-client-5.5.1/edx_rest_api_client/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # pylint: disable=line-too-long
 class JwtAuth(AuthBase):
     """
     Attaches JWT Authentication to the given Request object.
 
     Deprecated:
-        See https://github.com/edx/edx-platform/blob/master/openedx/core/djangoapps/oauth_dispatch/docs/decisions/0008-use-asymmetric-jwts.rst
+        See https://github.com/openedx/edx-platform/blob/master/openedx/core/djangoapps/oauth_dispatch/docs/decisions/0008-use-asymmetric-jwts.rst
 
     Todos:
         * Remove pyjwt dependency from edx-rest-api-client when this class is
             removed.
         * This class is only used by ecomworker according to data supplied by
             the `deprecated_jwt_signing` custom attribute. This class should be
             moved to ecomworker and out of the shared library until it can be
@@ -54,30 +54,42 @@
 
         set_custom_attribute('deprecated_jwt_signing', 'JwtAuth')
         r.headers['Authorization'] = 'JWT {jwt}'.format(jwt=jwt.encode(data, self.signing_key))
         return r
 
 
 class SuppliedJwtAuth(AuthBase):
-    """Attaches a supplied JWT to the given Request object."""
+    """
+    Attaches a supplied JWT to the given Request object.
+    """
 
     def __init__(self, token):
-        """Instantiate the auth class."""
+        """
+        Instantiate the auth class.
+        """
         self.token = token
 
     def __call__(self, r):
-        """Update the request headers."""
+        """
+        Update the request headers.
+        """
         r.headers['Authorization'] = f'JWT {self.token}'
         return r
 
 
 class BearerAuth(AuthBase):
-    """ Attaches Bearer Authentication to the given Request object. """
+    """
+    Attaches Bearer Authentication to the given Request object.
+    """
 
     def __init__(self, token):
-        """ Instantiate the auth class. """
+        """
+        Instantiate the auth class.
+        """
         self.token = token
 
     def __call__(self, r):
-        """ Update the request headers. """
+        """
+        Update the request headers.
+        """
         r.headers['Authorization'] = f'Bearer {self.token}'
         return r
```

### Comparing `edx-rest-api-client-5.5.0/edx_rest_api_client/client.py` & `edx-rest-api-client-5.5.1/edx_rest_api_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import datetime
 import json
 import os
 import socket
 
+import crum
 import requests
 import requests.utils
 import slumber
-
 from edx_django_utils.cache import TieredCache
 from edx_django_utils.monitoring import set_custom_attribute
-from edx_rest_api_client.auth import BearerAuth, JwtAuth, SuppliedJwtAuth
-from edx_rest_api_client.__version__ import __version__
 
+from edx_rest_api_client.__version__ import __version__
+from edx_rest_api_client.auth import BearerAuth, JwtAuth, SuppliedJwtAuth
 
 # When caching tokens, use this value to err on expiring tokens a little early so they are
 # sure to be valid at the time they are used.
 ACCESS_TOKEN_EXPIRED_THRESHOLD_SECONDS = 5
 
 # How long should we wait to connect to the auth service.
 # https://requests.readthedocs.io/en/master/user/advanced/#timeouts
@@ -66,18 +66,27 @@
 
     if stripped_url.endswith('/oauth2'):
         return stripped_url + '/access_token'
 
     return stripped_url + '/oauth2/access_token'
 
 
+def get_request_id():
+    """
+    Helper to get the request id - usually set via an X-Request-ID header
+    """
+    request = crum.get_current_request()
+    return getattr(request, 'id', None)
+
+
 def get_oauth_access_token(url, client_id, client_secret, token_type='jwt', grant_type='client_credentials',
                            refresh_token=None,
                            timeout=(REQUEST_CONNECT_TIMEOUT, REQUEST_READ_TIMEOUT)):
-    """ Retrieves OAuth 2.0 access token using the given grant type.
+    """
+    Retrieves OAuth 2.0 access token using the given grant type.
 
     Args:
         url (str): Oauth2 access token endpoint, optionally including part of the path.
         client_id (str): client ID
         client_secret (str): client secret
     Kwargs:
         token_type (str): Type of token to return. Options include bearer and jwt.
@@ -124,15 +133,16 @@
 
     return access_token, expires_at
 
 
 def get_and_cache_oauth_access_token(url, client_id, client_secret, token_type='jwt', grant_type='client_credentials',
                                      refresh_token=None,
                                      timeout=(REQUEST_CONNECT_TIMEOUT, REQUEST_READ_TIMEOUT)):
-    """ Retrieves a possibly cached OAuth 2.0 access token using the given grant type.
+    """
+    Retrieves a possibly cached OAuth 2.0 access token using the given grant type.
 
     See ``get_oauth_access_token`` for usage details.
 
     First retrieves the access token from the cache and ensures it has not expired. If
     the access token either wasn't found in the cache, or was expired, retrieves a new
     access token and caches it for the lifetime of the token.
 
@@ -199,15 +209,15 @@
         response.raise_for_status()  # could be an error response
         response_data = response.json()
 
     For more usage details, see documentation of the :class:`requests.Session` object:
     - https://requests.readthedocs.io/en/master/user/advanced/#session-objects
 
     Note: Requires Django + Middleware for TieredCache, used for caching the access token.
-    See https://github.com/edx/edx-django-utils/blob/master/edx_django_utils/cache/README.rst#tieredcache
+    See https://github.com/openedx/edx-django-utils/blob/master/edx_django_utils/cache/README.rst#tieredcache
 
     """
 
     # If the oauth_uri is set, it will be appended to the base_url.
     # Also, if oauth_uri does not end with `/oauth2/access_token`, it will be adjusted as necessary to do so.
     # This was needed when using the client to connect with a third-party (rather than LMS).
     oauth_uri = None
@@ -261,30 +271,35 @@
         Returns the JWT access token that will be used to make authenticated calls.
 
         The intention of this method is only to allow you to decode the JWT if you require
         any of its details, like the username. You should not use the JWT to make calls by
         another client.
 
         Here is example code that properly uses the configured JWT decoder:
-        https://github.com/edx/edx-drf-extensions/blob/master/edx_rest_framework_extensions/auth/jwt/authentication.py#L180-L190
+        https://github.com/openedx/edx-drf-extensions/blob/master/edx_rest_framework_extensions/auth/jwt/authentication.py#L180-L190
         """
         self._ensure_authentication()
         return self.auth.token
 
-    def request(self, method, url, **kwargs):  # pylint: disable=arguments-differ
+    def request(self, method, url, headers=None, **kwargs):  # pylint: disable=arguments-differ
         """
         Overrides Session.request to ensure that the session is authenticated.
 
         Note: Typically, users of the client won't call this directly, but will
         instead use Session.get or Session.post.
 
         """
+        request_id = get_request_id()
+        if headers is None:
+            headers = {}
+        if headers.get('X-Request-ID') is None and request_id is not None:
+            headers['X-Request-ID'] = request_id
         set_custom_attribute('api_client', 'OAuthAPIClient')
         self._ensure_authentication()
-        return super().request(method, url, **kwargs)
+        return super().request(method, url, headers=headers, **kwargs)
 
 
 class EdxRestApiClient(slumber.API):
     """
     API client for edX REST API.
 
     (deprecated)  See docs/decisions/0002-oauth-api-client-replacement.rst.
```

### Comparing `edx-rest-api-client-5.5.0/requirements/constraints.txt` & `edx-rest-api-client-5.5.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-rest-api-client-5.5.0/setup.py` & `edx-rest-api-client-5.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #!/usr/bin/env python
-""" Setup to allow pip installs of edx-rest-api-client module """
+"""
+Setup to allow pip installs of edx-rest-api-client module.
+"""
 
 import os
 import re
 
 from setuptools import find_packages, setup
 
 from edx_rest_api_client import __version__
@@ -77,29 +79,29 @@
 
     return line and line.strip() and not line.startswith(('-r', '#', '-e', 'git+', '-c'))
 
 
 setup(
     name='edx-rest-api-client',
     version=__version__,
-    description='Slumber client used to access various edX Platform REST APIs.',
+    description='Client utilities to access various Open edX Platform REST APIs.',
     long_description=long_description,
     long_description_content_type="text/x-rst",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Topic :: Internet',
         'Intended Audience :: Developers',
         'Environment :: Web Environment',
     ],
     keywords='edx rest api client',
-    url='https://github.com/edx/edx-rest-api-client',
+    url='https://github.com/openedx/edx-rest-api-client',
     author='edX',
     author_email='oscm@edx.org',
     license='Apache',
     packages=find_packages(exclude=['*.tests']),
     install_requires=load_requirements('requirements/base.in'),
 )
```

