# Comparing `tmp/skip-django-auth-token-0.2.15.2.tar.gz` & `tmp/skip-django-auth-token-0.2.15.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-auth-token-0.2.15.2.tar", last modified: Mon Mar  6 14:59:53 2023, max compression
+gzip compressed data, was "skip-django-auth-token-0.2.15.3.tar", last modified: Tue May 16 11:54:38 2023, max compression
```

## Comparing `skip-django-auth-token-0.2.15.2.tar` & `skip-django-auth-token-0.2.15.3.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.936814 skip-django-auth-token-0.2.15.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-06 14:59:53.936814 skip-django-auth-token-0.2.15.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.924814 skip-django-auth-token-0.2.15.2/auth_token/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.924814 skip-django-auth-token-0.2.15.2/auth_token/authorization_request/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/authorization_request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/authorization_request/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.924814 skip-django-auth-token-0.2.15.2/auth_token/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.924814 skip-django-auth-token-0.2.15.2/auth_token/contrib/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/admin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.928814 skip-django-auth-token-0.2.15.2/auth_token/contrib/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.928814 skip-django-auth-token-0.2.15.2/auth_token/contrib/common/auth_security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/common/auth_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/common/auth_security/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/common/auth_security/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.928814 skip-django-auth-token-0.2.15.2/auth_token/contrib/common/default/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/common/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/common/default/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/common/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/common/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.928814 skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.928814 skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/auth_security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/auth_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/auth_security/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.928814 skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/default/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/default/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.928814 skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/tests/auth_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.928814 skip-django-auth-token-0.2.15.2/auth_token/contrib/ms_sso/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/ms_sso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/ms_sso/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/ms_sso/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/ms_sso/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/ms_sso/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.928814 skip-django-auth-token-0.2.15.2/auth_token/contrib/rest_framework_auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/rest_framework_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/rest_framework_auth/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/rest_framework_auth/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.924814 skip-django-auth-token-0.2.15.2/auth_token/contrib/rest_framework_auth/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.928814 skip-django-auth-token-0.2.15.2/auth_token/contrib/rest_framework_auth/templates/rest_framework_auth/
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/rest_framework_auth/templates/rest_framework_auth/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/contrib/rest_framework_auth/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.924814 skip-django-auth-token-0.2.15.2/auth_token/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.924814 skip-django-auth-token-0.2.15.2/auth_token/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.928814 skip-django-auth-token-0.2.15.2/auth_token/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.928814 skip-django-auth-token-0.2.15.2/auth_token/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.928814 skip-django-auth-token-0.2.15.2/auth_token/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/management/commands/clean_authorization_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/management/commands/clean_authorization_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/management/commands/clean_one_time_passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.932814 skip-django-auth-token-0.2.15.2/auth_token/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0002_tokenrelatedobject.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0003_usertokentakeover.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0004_token_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0005_auto_20180626_1724.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0006_auto_20190312_0846.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0007_auto_20190313_1528.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0008_auto_20190509_1401.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0009_auto_20190622_1920.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0010_auto_20190723_1410.py
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0011_auto_20210119_1308.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0012_auto_20210119_1308.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0013_auto_20210119_1547.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0014_auto_20210308_0918.py
--rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0015_auto_20210308_0919.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/0016_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13691 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    23518 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/auth_token/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.932814 skip-django-auth-token-0.2.15.2/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.932814 skip-django-auth-token-0.2.15.2/example/dj/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.932814 skip-django-auth-token-0.2.15.2/example/dj/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.932814 skip-django-auth-token-0.2.15.2/example/dj/apps/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/apps/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/apps/app/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/apps/app/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.932814 skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/is_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/ms_sso.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)    38170 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.932814 skip-django-auth-token-0.2.15.2/example/dj/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/dj/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      385 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/example/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 14:59:53.936814 skip-django-auth-token-0.2.15.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-03-06 14:59:44.000000 skip-django-auth-token-0.2.15.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:59:53.936814 skip-django-auth-token-0.2.15.2/skip_django_auth_token.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-06 14:59:53.000000 skip-django-auth-token-0.2.15.2/skip_django_auth_token.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-03-06 14:59:53.000000 skip-django-auth-token-0.2.15.2/skip_django_auth_token.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:59:53.000000 skip-django-auth-token-0.2.15.2/skip_django_auth_token.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:59:53.000000 skip-django-auth-token-0.2.15.2/skip_django_auth_token.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-06 14:59:53.000000 skip-django-auth-token-0.2.15.2/skip_django_auth_token.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-06 14:59:53.000000 skip-django-auth-token-0.2.15.2/skip_django_auth_token.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.309946 skip-django-auth-token-0.2.15.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-16 11:54:38.309946 skip-django-auth-token-0.2.15.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.297946 skip-django-auth-token-0.2.15.3/auth_token/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.297946 skip-django-auth-token-0.2.15.3/auth_token/authorization_request/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/authorization_request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/authorization_request/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.297946 skip-django-auth-token-0.2.15.3/auth_token/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.297946 skip-django-auth-token-0.2.15.3/auth_token/contrib/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/admin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.297946 skip-django-auth-token-0.2.15.3/auth_token/contrib/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.297946 skip-django-auth-token-0.2.15.3/auth_token/contrib/common/auth_security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/common/auth_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/common/auth_security/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/common/auth_security/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.297946 skip-django-auth-token-0.2.15.3/auth_token/contrib/common/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/common/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/common/default/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/common/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/common/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.301946 skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.301946 skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/auth_security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/auth_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/auth_security/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.301946 skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/default/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.301946 skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/tests/auth_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.301946 skip-django-auth-token-0.2.15.3/auth_token/contrib/ms_sso/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/ms_sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/ms_sso/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/ms_sso/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/ms_sso/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/ms_sso/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.301946 skip-django-auth-token-0.2.15.3/auth_token/contrib/rest_framework_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/rest_framework_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/rest_framework_auth/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/rest_framework_auth/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.293945 skip-django-auth-token-0.2.15.3/auth_token/contrib/rest_framework_auth/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.301946 skip-django-auth-token-0.2.15.3/auth_token/contrib/rest_framework_auth/templates/rest_framework_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/rest_framework_auth/templates/rest_framework_auth/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/contrib/rest_framework_auth/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.293945 skip-django-auth-token-0.2.15.3/auth_token/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.293945 skip-django-auth-token-0.2.15.3/auth_token/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.301946 skip-django-auth-token-0.2.15.3/auth_token/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.301946 skip-django-auth-token-0.2.15.3/auth_token/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.301946 skip-django-auth-token-0.2.15.3/auth_token/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/management/commands/clean_authorization_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/management/commands/clean_authorization_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/management/commands/clean_one_time_passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.305945 skip-django-auth-token-0.2.15.3/auth_token/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0002_tokenrelatedobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0003_usertokentakeover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0004_token_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0005_auto_20180626_1724.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0006_auto_20190312_0846.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0007_auto_20190313_1528.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0008_auto_20190509_1401.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0009_auto_20190622_1920.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0010_auto_20190723_1410.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0011_auto_20210119_1308.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0012_auto_20210119_1308.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0013_auto_20210119_1547.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0014_auto_20210308_0918.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0015_auto_20210308_0919.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/0016_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13691 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23518 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/auth_token/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.305945 skip-django-auth-token-0.2.15.3/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.305945 skip-django-auth-token-0.2.15.3/example/dj/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.305945 skip-django-auth-token-0.2.15.3/example/dj/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.305945 skip-django-auth-token-0.2.15.3/example/dj/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/apps/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/apps/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/apps/app/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.309946 skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/is_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/ms_sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38170 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.309946 skip-django-auth-token-0.2.15.3/example/dj/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/dj/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      385 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/example/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 11:54:38.309946 skip-django-auth-token-0.2.15.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-16 11:54:28.000000 skip-django-auth-token-0.2.15.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:54:38.309946 skip-django-auth-token-0.2.15.3/skip_django_auth_token.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-16 11:54:38.000000 skip-django-auth-token-0.2.15.3/skip_django_auth_token.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-16 11:54:38.000000 skip-django-auth-token-0.2.15.3/skip_django_auth_token.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:54:38.000000 skip-django-auth-token-0.2.15.3/skip_django_auth_token.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:54:38.000000 skip-django-auth-token-0.2.15.3/skip_django_auth_token.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-16 11:54:38.000000 skip-django-auth-token-0.2.15.3/skip_django_auth_token.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 11:54:38.000000 skip-django-auth-token-0.2.15.3/skip_django_auth_token.egg-info/top_level.txt
```

### Comparing `skip-django-auth-token-0.2.15.2/LICENSE` & `skip-django-auth-token-0.2.15.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/PKG-INFO` & `skip-django-auth-token-0.2.15.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-auth-token
-Version: 0.2.15.2
+Version: 0.2.15.3
 Summary: Django authorization via tokens.
 Home-page: https://github.com/skip-pay/django-auth-token
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Keywords: django,authorization
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `skip-django-auth-token-0.2.15.2/README.rst` & `skip-django-auth-token-0.2.15.3/README.rst`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/authorization_request/backends.py` & `skip-django-auth-token-0.2.15.3/auth_token/authorization_request/backends.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/backends.py` & `skip-django-auth-token-0.2.15.3/auth_token/backends.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/config.py` & `skip-django-auth-token-0.2.15.3/auth_token/config.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/common/auth_security/validators.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/common/auth_security/validators.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/common/auth_security/views.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/common/auth_security/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/common/default/views.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/common/default/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from urllib.parse import quote_plus
+
 from django.contrib.auth.views import LoginView, LogoutView
 from django.utils.decorators import method_decorator
 from django.urls import reverse, NoReverseMatch
 from django.utils.translation import gettext
 from django.http import HttpResponseRedirect
 from django.views.decorators.cache import never_cache
 
@@ -36,15 +38,15 @@
         return HttpResponseRedirect(self.get_success_url())
 
     def _get_sso_login_methods(self):
         try:
             return [
                 {
                     'name': 'microsoft',
-                    'url': f'{reverse("ms-sso-login")}?next={self.request.GET.get("next", "/")}',
+                    'url': f'{reverse("ms-sso-login")}?next={quote_plus(self.request.GET.get("next", "/"), safe="/")}',
                     'label': gettext('Continue with Microsoft account')
                 }
             ]
         except NoReverseMatch:
             return []
 
     def get_context_data(self, **kwargs):
```

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/common/forms.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/common/forms.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/common/views.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/common/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/auth_security/resource.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/auth_security/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/default/resource.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/default/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/forms.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/forms.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/tests/auth_test_cases.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/tests/auth_test_cases.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/is_core_auth/views.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/is_core_auth/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/ms_sso/backends.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/ms_sso/backends.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/ms_sso/helpers.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/ms_sso/helpers.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/ms_sso/views.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/ms_sso/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/rest_framework_auth/authentication.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/rest_framework_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/rest_framework_auth/serializers.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/rest_framework_auth/serializers.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/rest_framework_auth/templates/rest_framework_auth/login.html` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/rest_framework_auth/templates/rest_framework_auth/login.html`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/contrib/rest_framework_auth/views.py` & `skip-django-auth-token-0.2.15.3/auth_token/contrib/rest_framework_auth/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/enums.py` & `skip-django-auth-token-0.2.15.3/auth_token/enums.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/locale/cs/LC_MESSAGES/django.mo` & `skip-django-auth-token-0.2.15.3/auth_token/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/locale/cs/LC_MESSAGES/django.po` & `skip-django-auth-token-0.2.15.3/auth_token/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/management/commands/clean_authorization_requests.py` & `skip-django-auth-token-0.2.15.3/auth_token/management/commands/clean_authorization_requests.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/management/commands/clean_authorization_tokens.py` & `skip-django-auth-token-0.2.15.3/auth_token/management/commands/clean_authorization_tokens.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/management/commands/clean_one_time_passwords.py` & `skip-django-auth-token-0.2.15.3/auth_token/management/commands/clean_one_time_passwords.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/middleware.py` & `skip-django-auth-token-0.2.15.3/auth_token/middleware.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/migrations/0001_initial.py` & `skip-django-auth-token-0.2.15.3/auth_token/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/migrations/0002_tokenrelatedobject.py` & `skip-django-auth-token-0.2.15.3/auth_token/migrations/0002_tokenrelatedobject.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/migrations/0003_usertokentakeover.py` & `skip-django-auth-token-0.2.15.3/auth_token/migrations/0003_usertokentakeover.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/migrations/0005_auto_20180626_1724.py` & `skip-django-auth-token-0.2.15.3/auth_token/migrations/0005_auto_20180626_1724.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/migrations/0006_auto_20190312_0846.py` & `skip-django-auth-token-0.2.15.3/auth_token/migrations/0006_auto_20190312_0846.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/migrations/0007_auto_20190313_1528.py` & `skip-django-auth-token-0.2.15.3/auth_token/migrations/0007_auto_20190313_1528.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/migrations/0008_auto_20190509_1401.py` & `skip-django-auth-token-0.2.15.3/auth_token/migrations/0008_auto_20190509_1401.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/migrations/0009_auto_20190622_1920.py` & `skip-django-auth-token-0.2.15.3/auth_token/migrations/0009_auto_20190622_1920.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/migrations/0010_auto_20190723_1410.py` & `skip-django-auth-token-0.2.15.3/auth_token/migrations/0010_auto_20190723_1410.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/migrations/0011_auto_20210119_1308.py` & `skip-django-auth-token-0.2.15.3/auth_token/migrations/0011_auto_20210119_1308.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/migrations/0012_auto_20210119_1308.py` & `skip-django-auth-token-0.2.15.3/auth_token/migrations/0012_auto_20210119_1308.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/migrations/0013_auto_20210119_1547.py` & `skip-django-auth-token-0.2.15.3/auth_token/migrations/0013_auto_20210119_1547.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/migrations/0014_auto_20210308_0918.py` & `skip-django-auth-token-0.2.15.3/auth_token/migrations/0014_auto_20210308_0918.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/migrations/0015_auto_20210308_0919.py` & `skip-django-auth-token-0.2.15.3/auth_token/migrations/0015_auto_20210308_0919.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/models.py` & `skip-django-auth-token-0.2.15.3/auth_token/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/signals.py` & `skip-django-auth-token-0.2.15.3/auth_token/signals.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/auth_token/utils.py` & `skip-django-auth-token-0.2.15.3/auth_token/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/admin.py` & `skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/admin.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/commands.py` & `skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/commands.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/is_core.py` & `skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/is_core.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/middleware.py` & `skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/middleware.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/models.py` & `skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/ms_sso.py` & `skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/ms_sso.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/rest_framework.py` & `skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/rest_framework.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/example/dj/apps/app/tests/utils.py` & `skip-django-auth-token-0.2.15.3/example/dj/apps/app/tests/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/example/dj/settings/base.py` & `skip-django-auth-token-0.2.15.3/example/dj/settings/base.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/example/dj/settings/settings.py` & `skip-django-auth-token-0.2.15.3/example/dj/settings/settings.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/example/dj/urls.py` & `skip-django-auth-token-0.2.15.3/example/dj/urls.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/example/dj/wsgi.py` & `skip-django-auth-token-0.2.15.3/example/dj/wsgi.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/setup.py` & `skip-django-auth-token-0.2.15.3/setup.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.2.15.2/skip_django_auth_token.egg-info/PKG-INFO` & `skip-django-auth-token-0.2.15.3/skip_django_auth_token.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-auth-token
-Version: 0.2.15.2
+Version: 0.2.15.3
 Summary: Django authorization via tokens.
 Home-page: https://github.com/skip-pay/django-auth-token
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Keywords: django,authorization
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `skip-django-auth-token-0.2.15.2/skip_django_auth_token.egg-info/SOURCES.txt` & `skip-django-auth-token-0.2.15.3/skip_django_auth_token.egg-info/SOURCES.txt`

 * *Files identical despite different names*

