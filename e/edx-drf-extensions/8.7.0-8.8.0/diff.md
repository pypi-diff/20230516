# Comparing `tmp/edx-drf-extensions-8.7.0.tar.gz` & `tmp/edx-drf-extensions-8.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-drf-extensions-8.7.0.tar", last modified: Tue Apr 18 20:28:33 2023, max compression
+gzip compressed data, was "edx-drf-extensions-8.8.0.tar", last modified: Tue May 16 16:18:20 2023, max compression
```

## Comparing `edx-drf-extensions-8.7.0.tar` & `edx-drf-extensions-8.8.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.995486 edx-drf-extensions-8.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)     6622 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10058 2023-04-18 20:28:32.995486 edx-drf-extensions-8.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2758 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.983485 edx-drf-extensions-8.7.0/csrf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.983485 edx-drf-extensions-8.7.0/csrf/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.987486 edx-drf-extensions-8.7.0/csrf/api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.987486 edx-drf-extensions-8.7.0/csrf/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      907 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/csrf/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.987486 edx-drf-extensions-8.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8975 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.987486 edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10058 2023-04-18 20:28:32.000000 edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-04-18 20:28:32.000000 edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 20:28:32.000000 edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-04-18 20:28:32.000000 edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-18 20:28:32.000000 edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.991485 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.991485 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.991485 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.991485 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6965 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.991485 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8299 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/cookies.py
--rw-r--r--   0 runner    (1001) docker     (122)    13117 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/decoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    14306 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.995486 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10681 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py
--rw-r--r--   0 runner    (1001) docker     (122)    13147 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    19881 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.995486 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1842 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.995486 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9944 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     4241 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/paginators.py
--rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.995486 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)    10793 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_paginators.py
--rw-r--r--   0 runner    (1001) docker     (122)    17320 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/edx_rest_framework_extensions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:28:32.995486 edx-drf-extensions-8.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      233 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-18 20:28:32.999486 edx-drf-extensions-8.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5114 2023-04-18 20:28:29.000000 edx-drf-extensions-8.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.900800 edx-drf-extensions-8.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10017 2023-05-16 16:18:20.900800 edx-drf-extensions-8.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.892800 edx-drf-extensions-8.8.0/csrf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/csrf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.892800 edx-drf-extensions-8.8.0/csrf/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/csrf/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/csrf/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.892800 edx-drf-extensions-8.8.0/csrf/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/csrf/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/csrf/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/csrf/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/csrf/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.892800 edx-drf-extensions-8.8.0/csrf/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/csrf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/csrf/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/csrf/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.892800 edx-drf-extensions-8.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8975 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.892800 edx-drf-extensions-8.8.0/edx_drf_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10017 2023-05-16 16:18:20.000000 edx-drf-extensions-8.8.0/edx_drf_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-05-16 16:18:20.000000 edx-drf-extensions-8.8.0/edx_drf_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 16:18:20.000000 edx-drf-extensions-8.8.0/edx_drf_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-16 16:18:20.000000 edx-drf-extensions-8.8.0/edx_drf_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-16 16:18:20.000000 edx-drf-extensions-8.8.0/edx_drf_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.896800 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.896800 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.896800 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/bearer/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/bearer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/bearer/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.896800 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/bearer/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/bearer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6965 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.896800 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8299 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13970 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14306 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.896800 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10681 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13147 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19881 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2322 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.896800 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/session/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1842 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/session/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.900800 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/session/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/session/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/session/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9944 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4241 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/paginators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.900800 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10793 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6384 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/tests/test_paginators.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17320 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/edx_rest_framework_extensions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 16:18:20.900800 edx-drf-extensions-8.8.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-05-16 16:18:20.900800 edx-drf-extensions-8.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5114 2023-05-16 16:18:15.000000 edx-drf-extensions-8.8.0/setup.py
```

### Comparing `edx-drf-extensions-8.7.0/CHANGELOG.rst` & `edx-drf-extensions-8.8.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.8.0] - 2023-05-16
+--------------------
+
+Removed
+~~~~~~~
+
+* Removed dependency on ``pyjwkest``. Uses existing PyJWT dependency instead.
+
 [8.7.0] - 2023-04-14
 --------------------
 
 Added
 ~~~~~
 
 * Add ``edx_drf_extensions_version`` to help with rollout of changes in this library across services.
```

### Comparing `edx-drf-extensions-8.7.0/LICENSE.txt` & `edx-drf-extensions-8.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/PKG-INFO` & `edx-drf-extensions-8.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-drf-extensions
-Version: 8.7.0
+Version: 8.8.0
 Summary: edX extensions of Django REST Framework
 Home-page: https://github.com/openedx/edx-drf-extensions
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -13,18 +13,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 License-File: LICENSE.txt
 
-Part of `edX code`__.
-
-__ https://code.edx.org/
-
 edX Django REST Framework Extensions  |CI|_ |Codecov|_
 ==========================================================
 .. |CI| image:: https://github.com/openedx/edx-drf-extensions/workflows/Python%20CI/badge.svg?branch=master
 .. _CI: https://github.com/openedx/edx-drf-extensions/actions?query=workflow%3A%22Python+CI%22
 
 .. |Codecov| image:: https://codecov.io/github/edx/edx-drf-extensions/coverage.svg?branch=master
 .. _Codecov: https://codecov.io/github/edx/edx-drf-extensions?branch=master
@@ -70,17 +66,16 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines should be followed for Open edX code in general.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 
@@ -94,14 +89,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.8.0] - 2023-05-16
+--------------------
+
+Removed
+~~~~~~~
+
+* Removed dependency on ``pyjwkest``. Uses existing PyJWT dependency instead.
+
 [8.7.0] - 2023-04-14
 --------------------
 
 Added
 ~~~~~
 
 * Add ``edx_drf_extensions_version`` to help with rollout of changes in this library across services.
```

### Comparing `edx-drf-extensions-8.7.0/README.rst` & `edx-drf-extensions-8.8.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-Part of `edX code`__.
-
-__ https://code.edx.org/
-
 edX Django REST Framework Extensions  |CI|_ |Codecov|_
 ==========================================================
 .. |CI| image:: https://github.com/openedx/edx-drf-extensions/workflows/Python%20CI/badge.svg?branch=master
 .. _CI: https://github.com/openedx/edx-drf-extensions/actions?query=workflow%3A%22Python+CI%22
 
 .. |Codecov| image:: https://codecov.io/github/edx/edx-drf-extensions/coverage.svg?branch=master
 .. _Codecov: https://codecov.io/github/edx/edx-drf-extensions?branch=master
@@ -51,15 +47,14 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines should be followed for Open edX code in general.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
```

### Comparing `edx-drf-extensions-8.7.0/csrf/api/v1/views.py` & `edx-drf-extensions-8.8.0/csrf/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/csrf/tests/test_api.py` & `edx-drf-extensions-8.8.0/csrf/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/docs/conf.py` & `edx-drf-extensions-8.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/PKG-INFO` & `edx-drf-extensions-8.8.0/edx_drf_extensions.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-drf-extensions
-Version: 8.7.0
+Version: 8.8.0
 Summary: edX extensions of Django REST Framework
 Home-page: https://github.com/openedx/edx-drf-extensions
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -13,18 +13,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 License-File: LICENSE.txt
 
-Part of `edX code`__.
-
-__ https://code.edx.org/
-
 edX Django REST Framework Extensions  |CI|_ |Codecov|_
 ==========================================================
 .. |CI| image:: https://github.com/openedx/edx-drf-extensions/workflows/Python%20CI/badge.svg?branch=master
 .. _CI: https://github.com/openedx/edx-drf-extensions/actions?query=workflow%3A%22Python+CI%22
 
 .. |Codecov| image:: https://codecov.io/github/edx/edx-drf-extensions/coverage.svg?branch=master
 .. _Codecov: https://codecov.io/github/edx/edx-drf-extensions?branch=master
@@ -70,17 +66,16 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines should be followed for Open edX code in general.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 
@@ -94,14 +89,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.8.0] - 2023-05-16
+--------------------
+
+Removed
+~~~~~~~
+
+* Removed dependency on ``pyjwkest``. Uses existing PyJWT dependency instead.
+
 [8.7.0] - 2023-04-14
 --------------------
 
 Added
 ~~~~~
 
 * Add ``edx_drf_extensions_version`` to help with rollout of changes in this library across services.
```

### Comparing `edx-drf-extensions-8.7.0/edx_drf_extensions.egg-info/SOURCES.txt` & `edx-drf-extensions-8.8.0/edx_drf_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/authentication.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/bearer/authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/bearer/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/authentication.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/cookies.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/cookies.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/decoder.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/decoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 """
 import logging
 import sys
 
 import jwt
 from django.conf import settings
 from edx_django_utils.monitoring import set_custom_attribute
-from jwkest.jwk import KEYS
-from jwkest.jws import JWS
+from jwt.api_jwk import PyJWK, PyJWKSet
+from jwt.utils import base64url_encode
 from rest_framework_jwt.settings import api_settings
 from semantic_version import Version
 
 from edx_rest_framework_extensions.settings import get_first_jwt_issuer, get_jwt_issuers
 
 
 logger = logging.getLogger(__name__)
@@ -199,15 +199,15 @@
     # .. custom_attribute_description: Number of JWT verification keys in use for this
     #   verification. Should be same as number of asymmetric public keys. This is
     #   intended to aid in key rotations; once the average count stabilizes at a
     #   higher number after adding a public key, it should be safe to change the secret key.
     set_custom_attribute('jwt_auth_verify_asymmetric_keys_count', len(key_set))
 
     try:
-        _ = JWS().verify_compact(token, key_set)
+        _verify_jwk_signature_using_keyset(token, key_set, jwt_issuer)
         # .. custom_attribute_name: jwt_auth_asymmetric_verified
         # .. custom_attribute_description: Whether the JWT was successfully verified
         #   using an asymmetric key.
         set_custom_attribute('jwt_auth_asymmetric_verified', True)
         return
     except Exception:  # pylint: disable=broad-except
         # Continue to the old code path of trying all keys
@@ -224,15 +224,15 @@
     #   verification. Should be same as number of asymmetric public keys, plus one if
     #   a symmetric key secret is set. This is intended to aid in key rotations; once
     #   the average count stabilizes at a higher number after adding a public key, it
     #   should be safe to change the secret key.
     set_custom_attribute('jwt_auth_verify_all_keys_count', len(key_set))
 
     try:
-        _ = JWS().verify_compact(token, key_set)
+        _verify_jwk_signature_using_keyset(token, key_set, jwt_issuer)
         # .. custom_attribute_name: jwt_auth_symmetric_verified
         # .. custom_attribute_description: Whether the JWT was successfully verified
         #   using a symmetric key.
         # Note: Rather than using a single custom attribute like ``jwt_auth_verified``
         #   with values of 'symmetric' or 'asymmetric', we use two separate custom
         #   attribute names (e.g. jwt_auth_symmetric_verified and jwt_auth_asymmetric_verified),
         #   so that if each of these were set separately in the same request, they
@@ -244,14 +244,35 @@
         # .. custom_attribute_description: True if the JWT token verification failed.
         set_custom_attribute('jwt_auth_verification_failed', True)
         logger.exception('Token verification failed.')
         exc_info = sys.exc_info()
         raise jwt.InvalidTokenError(exc_info[2]) from token_error
 
 
+def _verify_jwk_signature_using_keyset(token, key_set, jwt_issuer):
+    for i in range(0, len(key_set)):
+        try:
+            algorithms = None
+            if key_set[i].key_type == 'RSA':
+                algorithms = ['RS256', 'RS512',]
+            elif key_set[i].key_type == 'oct':
+                algorithms = ['HS256',]
+
+            _ = jwt.decode(
+                    token,
+                    key=key_set[i].key,
+                    algorithms=algorithms,
+                    audience=jwt_issuer['AUDIENCE'],
+                )
+            break
+        except Exception:  # pylint: disable=broad-except
+            if i == len(key_set) - 1:
+                raise
+
+
 def _decode_and_verify_token(token, jwt_issuer):
     """
     Part of the verification implementation; must not be used in isolation,
     as the signature is actually checked in a different function.
     """
     options = {
         'require': ["exp", "iat"],
@@ -295,19 +316,20 @@
 
 
 def _get_signing_jwk_key_set(jwt_issuer, add_symmetric_keys=True):
     """
     Returns a JWK Keyset containing all active keys that are configured
     for verifying signatures.
     """
-    key_set = KEYS()
+    key_set = []
 
     # asymmetric keys
     signing_jwk_set = settings.JWT_AUTH.get('JWT_PUBLIC_SIGNING_JWK_SET')
     if signing_jwk_set:
-        key_set.load_jwks(signing_jwk_set)
+        key_set.extend(PyJWKSet.from_json(signing_jwk_set).keys)
 
     if add_symmetric_keys:
         # symmetric key
-        key_set.add({'key': jwt_issuer['SECRET_KEY'], 'kty': 'oct'})
+        encoded_secret_key = base64url_encode(jwt_issuer['SECRET_KEY'].encode('utf-8'))
+        key_set.append(PyJWK({'k': encoded_secret_key, 'kty': 'oct'}))
 
     return key_set
```

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/middleware.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/jwt/tests/utils.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/jwt/tests/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """ Utility functions for tests. """
-import json
 from time import time
 
 import jwt
 from django.conf import settings
-from jwkest import jwk
-from jwkest.jws import JWS
+from jwt.api_jwk import PyJWK
 
 
 def generate_jwt(user, scopes=None, filters=None, is_restricted=None):
     """
     Generate a valid JWT for authenticated requests.
     """
     access_token = generate_latest_version_payload(
@@ -29,22 +27,17 @@
     return jwt.encode(payload, signing_key)
 
 
 def generate_asymmetric_jwt_token(payload):
     """
     Generate a valid asymmetric JWT token for authenticated requests.
     """
-    keys = jwk.KEYS()
-    serialized_keypair = json.loads(settings.JWT_AUTH['JWT_PRIVATE_SIGNING_JWK'])
-    keys.add(serialized_keypair)
+    private_key = PyJWK.from_json(settings.JWT_AUTH['JWT_PRIVATE_SIGNING_JWK'])
     algorithm = settings.JWT_AUTH['JWT_SIGNING_ALGORITHM']
-
-    data = json.dumps(payload)
-    jws = JWS(data, alg=algorithm)
-    return jws.sign_compact(keys=keys)
+    return jwt.encode(payload, key=private_key.key, algorithm=algorithm)
 
 
 def generate_latest_version_payload(user, scopes=None, filters=None, version=None,
                                     is_restricted=None):
     """
     Generate a valid JWT payload given a user and optionally scopes and filters.
     """
```

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/authentication.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/session/authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/auth/session/tests/test_authentication.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/auth/session/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/config.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/config.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/middleware.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/paginators.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/paginators.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/permissions.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/permissions.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/settings.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/settings.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_middleware.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_paginators.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/tests/test_paginators.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_permissions.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/edx_rest_framework_extensions/tests/test_settings.py` & `edx-drf-extensions-8.8.0/edx_rest_framework_extensions/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/requirements/constraints.txt` & `edx-drf-extensions-8.8.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-drf-extensions-8.7.0/setup.py` & `edx-drf-extensions-8.8.0/setup.py`

 * *Files identical despite different names*

