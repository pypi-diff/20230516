# Comparing `tmp/openimis-be-core-1.5.0.tar.gz` & `tmp/openimis-be-core-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-core-1.5.0.tar", last modified: Thu Nov 10 18:09:06 2022, max compression
+gzip compressed data, was "openimis-be-core-1.5.1.tar", last modified: Tue May 16 21:37:51 2023, max compression
```

## Comparing `openimis-be-core-1.5.0.tar` & `openimis-be-core-1.5.1.tar`

### file list

```diff
@@ -1,101 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:06.379299 openimis-be-core-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-11-10 18:09:06.379299 openimis-be-core-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    19127 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:06.375299 openimis-be-core-1.5.0/core/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6086 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/abs_calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     8096 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:06.375299 openimis-be-core-1.5.0/core/calendars/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/calendars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/calendars/ad_calendar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/calendars/ne_calendar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/calendars/test_ad_calendar.py
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/calendars/test_ne_calendar.py
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/custom_lookups.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:06.375299 openimis-be-core-1.5.0/core/datetimes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/datetimes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4652 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/datetimes/ad_datetime.py
--rw-r--r--   0 runner    (1001) docker     (121)    11952 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/datetimes/ne_datetime.py
--rw-r--r--   0 runner    (1001) docker     (121)     7203 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/datetimes/shared.py
--rw-r--r--   0 runner    (1001) docker     (121)    10516 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/datetimes/test_ad_datetime.py
--rw-r--r--   0 runner    (1001) docker     (121)    14463 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/datetimes/test_ne_datetime.py
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/datetimes/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:06.375299 openimis-be-core-1.5.0/core/gql/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/gql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:06.375299 openimis-be-core-1.5.0/core/gql/gql_mutations/
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/gql/gql_mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9327 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/gql/gql_mutations/base_mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/gql/gql_mutations/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/gql/gql_mutations/input_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    10209 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/gql/gql_mutations/mutation_by_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     6913 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/gql_queries.py
--rw-r--r--   0 runner    (1001) docker     (121)     3440 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/jwt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/jwt_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:06.379299 openimis-be-core-1.5.0/core/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     5044 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0002_auto_20190726_0701.py
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0003_control_mutationlog.py
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0004_auto_20190830_1625.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0005_group_usergroup.py
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0006_fieldcontrol.py
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0007_auto_20191008_0923.py
--rw-r--r--   0 runner    (1001) docker     (121)     3550 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0008_officer_role_roleright_userrole.py
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0009_mutationlog_client_mutation_details.py
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0010_rolemutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0011_auto_20210324_1528.py
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0012_users_officers_admins.py
--rw-r--r--   0 runner    (1001) docker     (121)     2686 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0013_users_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0014_users.py
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0015_missing_roles.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/0016_add_last_login_on_interactive_user.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    37544 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1677 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)    52900 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/security.py
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4005 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/service_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:06.379299 openimis-be-core-1.5.0/core/services/
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/services/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    10148 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/services/userServices.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:06.379299 openimis-be-core-1.5.0/core/services/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/services/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2319 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/services/utils/serviceUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4620 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:06.379299 openimis-be-core-1.5.0/core/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/templates/password_reset.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/test_security.py
--rw-r--r--   0 runner    (1001) docker     (121)    18987 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/test_services.py
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     7527 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:06.379299 openimis-be-core-1.5.0/core/validation/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/validation/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/validation/objectExistsValidationMixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3173 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/validation/obligatoryFieldValidation.py
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/validation/uniqueCodeValidationMixin.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:06.379299 openimis-be-core-1.5.0/core/websocket/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4502 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/websocket/abstract_websocket_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/websocket/async_websocket_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-11-10 18:08:55.000000 openimis-be-core-1.5.0/core/websocket/base_websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:06.379299 openimis-be-core-1.5.0/openimis_be_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-11-10 18:09:06.000000 openimis-be-core-1.5.0/openimis_be_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2541 2022-11-10 18:09:06.000000 openimis-be-core-1.5.0/openimis_be_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 18:09:06.000000 openimis-be-core-1.5.0/openimis_be_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-10 18:09:06.000000 openimis-be-core-1.5.0/openimis_be_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-10 18:09:06.000000 openimis-be-core-1.5.0/openimis_be_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 18:09:06.379299 openimis-be-core-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-11-10 18:09:04.000000 openimis-be-core-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:51.815735 openimis-be-core-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-16 21:37:51.815735 openimis-be-core-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19127 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:51.807735 openimis-be-core-1.5.1/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/abs_calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:51.807735 openimis-be-core-1.5.1/core/calendars/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/calendars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/calendars/ad_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/calendars/ne_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/calendars/test_ad_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/calendars/test_ne_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/custom_lookups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:51.807735 openimis-be-core-1.5.1/core/datetimes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/datetimes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/datetimes/ad_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/datetimes/ne_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/datetimes/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/datetimes/test_ad_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/datetimes/test_ne_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/datetimes/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:51.807735 openimis-be-core-1.5.1/core/gql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/gql/custom_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/gql/export_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:51.811735 openimis-be-core-1.5.1/core/gql/gql_mutations/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/gql/gql_mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/gql/gql_mutations/base_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/gql/gql_mutations/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/gql/gql_mutations/input_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/gql/gql_mutations/mutation_by_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/gql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/jwt_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:51.811735 openimis-be-core-1.5.1/core/migration_to_history_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migration_to_history_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migration_to_history_model/create_temp_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migration_to_history_model/patch_table_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:51.811735 openimis-be-core-1.5.1/core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0002_auto_20190726_0701.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0003_control_mutationlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0004_auto_20190830_1625.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0005_group_usergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0006_fieldcontrol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0007_auto_20191008_0923.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0008_officer_role_roleright_userrole.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0009_mutationlog_client_mutation_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0010_rolemutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0011_auto_20210324_1528.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0012_users_officers_admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0013_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0014_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0015_missing_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0016_add_last_login_on_interactive_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0017_exportablequerymodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0018_auto_20230318_1551.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0019_extended_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0020_add_missing_fields_to_django_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/0021_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40316 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59586 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/service_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:51.815735 openimis-be-core-1.5.1/core/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/services/roleServices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/services/userServices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:51.815735 openimis-be-core-1.5.1/core/services/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/services/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/services/utils/serviceUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:51.815735 openimis-be-core-1.5.1/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/templates/password_reset.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18987 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:51.815735 openimis-be-core-1.5.1/core/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/validation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/validation/objectExistsValidationMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/validation/obligatoryFieldValidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/validation/uniqueCodeValidationMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:51.815735 openimis-be-core-1.5.1/core/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/websocket/abstract_websocket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/websocket/async_websocket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-16 21:37:34.000000 openimis-be-core-1.5.1/core/websocket/base_websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:51.815735 openimis-be-core-1.5.1/openimis_be_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-16 21:37:51.000000 openimis-be-core-1.5.1/openimis_be_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-16 21:37:51.000000 openimis-be-core-1.5.1/openimis_be_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:37:51.000000 openimis-be-core-1.5.1/openimis_be_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-16 21:37:51.000000 openimis-be-core-1.5.1/openimis_be_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-16 21:37:51.000000 openimis-be-core-1.5.1/openimis_be_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:37:51.815735 openimis-be-core-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-16 21:37:49.000000 openimis-be-core-1.5.1/setup.py
```

### Comparing `openimis-be-core-1.5.0/LICENSE.md` & `openimis-be-core-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/PKG-INFO` & `openimis-be-core-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-core
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Core reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-core-1.5.0/README.md` & `openimis-be-core-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/abs_calculation_rule.py` & `openimis-be-core-1.5.1/core/abs_calculation_rule.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/apps.py` & `openimis-be-core-1.5.1/core/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 logger = logging.getLogger(__name__)
 
 MODULE_NAME = "core"
 
 this = sys.modules[MODULE_NAME]
 
 DEFAULT_CFG = {
+    "username_code_length": "8",  # cannot be bigger than 50 unless modified length limit
+    "user_username_and_code_length_limit": "50",
     "auto_provisioning_user_group": "user",
     "calendar_package": "core",
     "calendar_module": ".calendars.ad_calendar",
     "datetime_package": "core",
     "datetime_module": ".datetimes.ad_datetime",
     "shortstrfdate": "%d/%m/%Y",
     "longstrfdate": "%a %d %B %Y",
@@ -49,14 +51,16 @@
     "fields_controls_eo": {},
 }
 
 
 class CoreConfig(AppConfig):
     default_auto_field = 'django.db.models.AutoField'  # Django 3.1+
     name = MODULE_NAME
+    username_code_length = 8
+    user_username_and_code_length_limit = 50
     age_of_majority = 18
     password_reset_template = "password_reset.txt"
     gql_query_roles_perms = []
     gql_mutation_create_roles_perms = []
     gql_mutation_update_roles_perms = []
     gql_mutation_replace_roles_perms = []
     gql_mutation_duplicate_roles_perms = []
@@ -96,14 +100,20 @@
             this.datetime = self._import_module(cfg, "datetime")
         except Exception:
             logger.error('Failed to configure calendar, using default!\n%s: %s' % (
                 sys.exc_info()[0].__name__, sys.exc_info()[1]))
             this.calendar = self._import_module(DEFAULT_CFG, "calendar")
             this.datetime = self._import_module(DEFAULT_CFG, "datetime")
 
+    def _configure_username_code_length(self, cfg):
+        this.username_code_length = int(cfg["username_code_length"])
+
+    def _configure_user_username_and_code_length_limit(self, cfg):
+        this.user_username_and_code_length_limit = int(cfg["user_username_and_code_length_limit"])
+
     def _configure_majority(self, cfg):
         this.age_of_majority = int(cfg["age_of_majority"])
 
     def _configure_currency(self, cfg):
         this.currency = str(cfg["currency"])
 
     def _configure_auto_provisioning(self, cfg):
@@ -119,15 +129,15 @@
             g = Group(name=group)
             g.save()
             from django.contrib.auth.models import Permission
             p = Permission.objects.get(codename="view_user")
             g.permissions.add(p)
             g.save()
         except Exception as e:
-            logger.warning('Failed set auto_provisioning_user_group '+str(e))
+            logger.warning('Failed set auto_provisioning_user_group ' + str(e))
 
     def _configure_graphql(self, cfg):
         this.async_mutations = True if cfg["async_mutations"] is None else cfg["async_mutations"].lower() == "true"
 
     def _configure_permissions(self, cfg):
         CoreConfig.gql_query_roles_perms = cfg["gql_query_roles_perms"]
         CoreConfig.gql_mutation_create_roles_perms = cfg["gql_mutation_create_roles_perms"]
@@ -152,14 +162,16 @@
         CoreConfig.fields_controls_user = cfg["fields_controls_user"]
         CoreConfig.fields_controls_eo = cfg["fields_controls_eo"]
 
     def ready(self):
         from .models import ModuleConfiguration
         cfg = ModuleConfiguration.get_or_default(MODULE_NAME, DEFAULT_CFG)
         self._configure_calendar(cfg)
+        self._configure_username_code_length(cfg)
+        self._configure_user_username_and_code_length_limit(cfg)
         self._configure_majority(cfg)
         self._configure_auto_provisioning(cfg)
         self._configure_graphql(cfg)
         self._configure_currency(cfg)
         self._configure_permissions(cfg)
 
         self.password_reset_template = cfg["password_reset_template"]
```

### Comparing `openimis-be-core-1.5.0/core/calendars/ad_calendar.py` & `openimis-be-core-1.5.1/core/calendars/ad_calendar.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/calendars/ne_calendar.py` & `openimis-be-core-1.5.1/core/calendars/ne_calendar.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/calendars/test_ad_calendar.py` & `openimis-be-core-1.5.1/core/calendars/test_ad_calendar.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/calendars/test_ne_calendar.py` & `openimis-be-core-1.5.1/core/calendars/test_ne_calendar.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/custom_lookups.py` & `openimis-be-core-1.5.1/core/custom_lookups.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/datetimes/ad_datetime.py` & `openimis-be-core-1.5.1/core/datetimes/ad_datetime.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/datetimes/ne_datetime.py` & `openimis-be-core-1.5.1/core/datetimes/ne_datetime.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/datetimes/shared.py` & `openimis-be-core-1.5.1/core/datetimes/shared.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/datetimes/test_ad_datetime.py` & `openimis-be-core-1.5.1/core/datetimes/test_ad_datetime.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/datetimes/test_ne_datetime.py` & `openimis-be-core-1.5.1/core/datetimes/test_ne_datetime.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/datetimes/test_shared.py` & `openimis-be-core-1.5.1/core/datetimes/test_shared.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/fields.py` & `openimis-be-core-1.5.1/core/fields.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/forms.py` & `openimis-be-core-1.5.1/core/forms.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/gql/gql_mutations/base_mutation.py` & `openimis-be-core-1.5.1/core/gql/gql_mutations/base_mutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/gql/gql_mutations/exceptions.py` & `openimis-be-core-1.5.1/core/gql/gql_mutations/exceptions.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/gql/gql_mutations/mutation_by_filter.py` & `openimis-be-core-1.5.1/core/gql/gql_mutations/mutation_by_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                     .filter(q_filter) \
 
                 if return_objects:
                     data['filtered_objects'] = base_query
                 else:
                     uuids = base_query.values_list('uuid', flat=True).distinct()
                     data['uuids'] = uuids
-            async_mutate(cls, user, **data)
+            return async_mutate(cls, user, **data)
         return wrapper
     return inner_function
 
 
 def map_gql_to_django_filter(filters: dict, qgl_type_filters, explicit_handlers=None):
     if explicit_handlers is None:
         explicit_handlers = {}
@@ -178,15 +178,15 @@
                         base_query = base_query.filter(_append_filter_amount(amount_from, amount_to))
 
                 if return_objects:
                     data['filtered_objects'] = base_query
                 else:
                     uuids = base_query.values_list('id', flat=True).distinct()
                     data['uuids'] = uuids
-            async_mutate(cls, user, **data)
+            return async_mutate(cls, user, **data)
         return wrapper
     return inner_function
 
 
 def _append_filter_amount(amount_from, amount_to):
     # TODO make a signal to contract module to not break modular approach and
     #  not repeat the same code from contract module
```

### Comparing `openimis-be-core-1.5.0/core/gql_queries.py` & `openimis-be-core-1.5.1/core/gql_queries.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import graphene
 import location.gql_queries
 from core import ExtendedConnection, filter_validity
 from core.models import Officer, Role, RoleRight, UserRole, User, InteractiveUser, UserMutation, Language
 from graphene_django import DjangoObjectType
 from location.models import HealthFacility
+from .apps import CoreConfig
+from django.utils.translation import gettext as _
+from django.core.exceptions import PermissionDenied
 
 from .utils import prefix_filterset
 
 
 class OfficerGQLType(DjangoObjectType):
     """
     This type corresponds to the Enrolment Officer but is a bit more generic than just Enrolment.
@@ -108,28 +111,34 @@
             "email": ["iexact"],
             "is_associated": ["exact"],
             "language_id": ["exact"],
         }
         connection_class = ExtendedConnection
 
     def resolve_health_facility(self, info, **kwargs):
+        if not info.context.user.has_perms(CoreConfig.gql_query_users_perms):
+            raise PermissionDenied(_("unauthorized"))
         if self.health_facility_id:
             return HealthFacility.get_queryset(None, info).filter(pk=self.health_facility_id).first()
         else:
             return None
 
     def resolve_roles(self, info, **kwargs):
+        if not info.context.user.is_authenticated:
+            raise PermissionDenied(_("unauthorized"))
         if self.user_roles:
             return Role.objects\
                 .filter(validity_to__isnull=True)\
                 .filter(user_roles__user_id=self.id, user_roles__validity_to__isnull=True)
         else:
             return None
 
     def resolve_userdistrict_set(self, info, **kwargs):
+        if not info.context.user.is_authenticated:
+            raise PermissionDenied(_("unauthorized"))
         if self.userdistrict_set:
             return self.userdistrict_set.filter(*filter_validity())
         else:
             return None
 
     @classmethod
     def get_queryset(cls, queryset, info):
@@ -162,14 +171,16 @@
         connection_class = ExtendedConnection
 
     @classmethod
     def get_queryset(cls, queryset, info):
         return User.get_queryset(queryset, info)
 
     def resolve_client_mutation_id(self, info):
+        if not info.context.user.has_perms(CoreConfig.gql_query_users_perms):
+            raise PermissionDenied(_("unauthorized"))
         user_mutation = self.mutations.select_related('mutation').filter(mutation__status=0).first()
         return user_mutation.mutation.client_mutation_id if user_mutation else None
 
 
 class PermissionOpenImisGQLType(graphene.ObjectType):
     perms_name = graphene.String()
     perms_value = graphene.Int()
@@ -201,7 +212,17 @@
             "name": ["exact"],
             "sort_order": ["exact"]
         }
 
     @classmethod
     def get_queryset(cls, queryset, info):
         return queryset
+
+
+class ValidationMessageGQLType(graphene.ObjectType):
+    """
+    This object is used for validation of user's input in forms (e.g. insuree code).
+    """
+    is_valid = graphene.Boolean()
+    error_code = graphene.Int()
+    error_message = graphene.String()
+
```

### Comparing `openimis-be-core-1.5.0/core/jwt.py` & `openimis-be-core-1.5.1/core/jwt.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/jwt_authentication.py` & `openimis-be-core-1.5.1/core/jwt_authentication.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/migrations/0001_initial.py` & `openimis-be-core-1.5.1/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/migrations/0002_auto_20190726_0701.py` & `openimis-be-core-1.5.1/core/migrations/0002_auto_20190726_0701.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/migrations/0003_control_mutationlog.py` & `openimis-be-core-1.5.1/core/migrations/0003_control_mutationlog.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/migrations/0004_auto_20190830_1625.py` & `openimis-be-core-1.5.1/core/migrations/0004_auto_20190830_1625.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/migrations/0005_group_usergroup.py` & `openimis-be-core-1.5.1/core/migrations/0005_group_usergroup.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/migrations/0006_fieldcontrol.py` & `openimis-be-core-1.5.1/core/migrations/0006_fieldcontrol.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/migrations/0008_officer_role_roleright_userrole.py` & `openimis-be-core-1.5.1/core/migrations/0008_officer_role_roleright_userrole.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/migrations/0010_rolemutation.py` & `openimis-be-core-1.5.1/core/migrations/0010_rolemutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/migrations/0011_auto_20210324_1528.py` & `openimis-be-core-1.5.1/core/migrations/0011_auto_20210324_1528.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/migrations/0012_users_officers_admins.py` & `openimis-be-core-1.5.1/core/migrations/0012_users_officers_admins.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/migrations/0013_users_api.py` & `openimis-be-core-1.5.1/core/migrations/0013_users_api.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/migrations/0014_users.py` & `openimis-be-core-1.5.1/core/migrations/0014_users.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/migrations/0015_missing_roles.py` & `openimis-be-core-1.5.1/core/migrations/0015_missing_roles.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/migrations/0016_add_last_login_on_interactive_user.py` & `openimis-be-core-1.5.1/core/migrations/0016_add_last_login_on_interactive_user.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/models.py` & `openimis-be-core-1.5.1/core/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import json
 import logging
 import os
 import sys
 import uuid
 from copy import copy
-from datetime import datetime as py_datetime
+from datetime import datetime as py_datetime, timedelta
 
 from cached_property import cached_property
 from dirtyfields import DirtyFieldsMixin
 from django.apps import apps
 from django.conf import settings
 from django.contrib.auth.models import AbstractBaseUser, BaseUserManager, PermissionsMixin, Group
 from django.core.exceptions import ObjectDoesNotExist, PermissionDenied, ValidationError
+from django.core.files.base import ContentFile
 from django.db import models
 from django.db.models import Q, DO_NOTHING, F, JSONField
 from django.utils.crypto import salted_hmac
 from graphql import ResolveInfo
+from pandas import DataFrame
 from simple_history.models import HistoricalRecords
 
 import core
+from django.conf import settings
+
+from .apps import CoreConfig
 from .fields import DateTimeField
 from .utils import filter_validity
 
 logger = logging.getLogger(__name__)
 
 
 class UUIDModel(models.Model):
@@ -170,15 +175,15 @@
     code = models.CharField(db_column='LanguageCode',
                             primary_key=True, max_length=5)
     name = models.CharField(db_column='LanguageName', max_length=50)
     sort_order = models.IntegerField(
         db_column='SortOrder', blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblLanguages'
 
 
 class UserManager(BaseUserManager):
 
     def _create_core_user(self, **fields):
         user = User(**fields)
@@ -225,15 +230,15 @@
             return user, False
         except User.DoesNotExist:
             return self.auto_provision_user(**kwargs)
 
 
 class TechnicalUser(AbstractBaseUser):
     id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
-    username = models.CharField(max_length=150, unique=True)
+    username = models.CharField(max_length=CoreConfig.user_username_and_code_length_limit, unique=True)
     email = models.EmailField(blank=True, null=True)
     language = 'en'
     is_staff = models.BooleanField(default=False)
     is_superuser = models.BooleanField(default=False)
     validity_from = models.DateTimeField(blank=True, null=True)
     validity_to = models.DateTimeField(blank=True, null=True)
 
@@ -285,15 +290,15 @@
         if settings.ROW_SECURITY and user.is_anonymous:
             return queryset.filter(id=-1)
         if settings.ROW_SECURITY:
             pass
         return queryset
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblRole'
 
 
 class RoleRight(VersionedModel):
     id = models.AutoField(db_column='RoleRightID', primary_key=True)
     role = models.ForeignKey(Role, models.DO_NOTHING,
                              db_column='RoleID', related_name="rights")
@@ -308,26 +313,26 @@
         if settings.ROW_SECURITY and user.is_anonymous:
             return queryset.filter(id=-1)
         if settings.ROW_SECURITY:
             pass
         return queryset
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblRoleRight'
 
 
 class InteractiveUser(VersionedModel):
     id = models.AutoField(db_column="UserID", primary_key=True)
     uuid = models.CharField(db_column="UserUUID", max_length=36, default=uuid.uuid4, unique=True)
     language = models.ForeignKey(Language, models.DO_NOTHING, db_column="LanguageID")
     last_name = models.CharField(db_column="LastName", max_length=100)
     other_names = models.CharField(db_column="OtherNames", max_length=100)
     phone = models.CharField(db_column="Phone", max_length=50, blank=True, null=True)
-    login_name = models.CharField(db_column="LoginName", max_length=25)
+    login_name = models.CharField(db_column="LoginName", max_length=CoreConfig.user_username_and_code_length_limit)
     last_login = models.DateTimeField(db_column="LastLogin", null=True)
     health_facility_id = models.IntegerField(db_column="HFID", blank=True, null=True)
 
     audit_user_id = models.IntegerField(db_column="AuditUserID")
     # dummy_pwd is always blank. It is actually a transient field used in the Legacy to pass the clear text password in
     # a User object from the ASPX to the DAL where it is processed into/against password and private key/salt)
     # dummy_pwd = models.CharField(db_column='DummyPwd', max_length=25, blank=True, null=True)
@@ -368,27 +373,33 @@
     def get_username(self):
         return self.login_name
 
     @property
     def stored_password(self):
         return self.password
 
+    @property
+    def user(self):
+        return self.user_set.first()
+
     @stored_password.setter
     def stored_password(self, value):
         logger.warn(
             "You should not use this property to set a password. Use 'password' instead."
         )
         self.password = value
 
     @property
     def is_staff(self):
         return False
 
     @property
     def is_superuser(self):
+        if self.user and self.user.t_user:
+            return self.user.t_user.is_superuser
         return False
 
     @cached_property
     def rights(self):
         return [rr.right_id for rr in RoleRight.filter_queryset().filter(
             role_id__in=[r.role_id for r in UserRole.filter_queryset().filter(
                 user_id=self.id)]).distinct()]
@@ -406,14 +417,25 @@
         return None
 
     @property
     def is_officer(self):
         return Officer.objects.filter(
             code=self.username, has_login=True, validity_to__isnull=True).exists()
 
+    @property
+    def is_claim_admin(self):
+        # Unlike Officer ClaimAdmin model was moved to the claim module,
+        # and it's not granted that the module is installed.
+        if 'claim' in sys.modules:
+            from claim.models import ClaimAdmin
+            return ClaimAdmin.objects.filter(
+                code=self.username, has_login=True, validity_to__isnull=True).exists()
+        else:
+            return False
+
     def set_password(self, raw_password):
         from hashlib import sha256
         from secrets import token_hex
 
         self.private_key = token_hex(128)
         pwd_hash = sha256()
         pwd_hash.update(f"{raw_password.rstrip()}{self.private_key}".encode())
@@ -449,34 +471,34 @@
         if isinstance(user, ResolveInfo):
             user = user.context.user
         if settings.ROW_SECURITY and user.is_anonymous:
             return queryset.filter(id=-1)
         return queryset
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblUsers'
 
 
 class UserRole(VersionedModel):
     id = models.AutoField(db_column='UserRoleID', primary_key=True)
     user = models.ForeignKey(
         InteractiveUser, models.DO_NOTHING, db_column='UserID', related_name="user_roles")
     role = models.ForeignKey(Role, models.DO_NOTHING,
                              db_column='RoleID', related_name="user_roles")
     audit_user_id = models.IntegerField(
         db_column='AudituserID', blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblUserRole'
 
 
 class User(UUIDModel, PermissionsMixin):
-    username = models.CharField(unique=True, max_length=25)
+    username = models.CharField(unique=True, max_length=CoreConfig.user_username_and_code_length_limit)
     t_user = models.ForeignKey(TechnicalUser, on_delete=models.CASCADE, blank=True, null=True)
     i_user = models.ForeignKey(InteractiveUser, on_delete=models.CASCADE, blank=True, null=True)
     officer = models.ForeignKey("Officer", on_delete=models.CASCADE, blank=True, null=True)
     claim_admin = models.ForeignKey("claim.ClaimAdmin", on_delete=models.CASCADE, blank=True, null=True)
 
     USERNAME_FIELD = 'username'
     REQUIRED_FIELDS = []
@@ -509,15 +531,17 @@
 
     @property
     def is_staff(self):
         return self._u.is_staff
 
     @property
     def is_superuser(self):
-        return self._u.is_superuser
+        if self.user and self.user.t_user:
+            return self.user.t_user.is_superuser
+        return False
 
     @property
     def is_active(self):
         if self._u.validity_from is None and self._u.validity_to is None:
             return True
         from core import datetime
         now = datetime.datetime.now()
@@ -525,19 +549,18 @@
             return False
         if not self._u.validity_to is None and self._u.validity_to < now:
             return False
         return True
 
     def has_perm(self, perm, obj=None):
         i_user = self.i_user if obj is None else obj.i_user
-        return (
-            True
-            if i_user is not None and perm in i_user.rights_str
-            else super(User, self).has_perm(perm, obj)
-        )
+        if i_user is not None and (i_user.is_superuser or perm in i_user.rights_str):
+            return True
+        else:
+            return super(User, self).has_perm(perm, obj)
 
     @property
     def rights(self):
         if self.i_user:
             return self.i_user.rights
         return []
 
@@ -622,33 +645,34 @@
 
 
 class UserGroup(models.Model):
     user = models.ForeignKey(User, models.DO_NOTHING)
     group = models.ForeignKey(Group, models.DO_NOTHING)
 
     class Meta:
-        managed = False
-        db_table = 'core_User_groups'
+        managed = True
+        db_table = 'Core_User_groups'
         unique_together = (('user', 'group'),)
 
 
-class Officer(VersionedModel):
+class Officer(VersionedModel, ExtendableModel):
     id = models.AutoField(db_column='OfficerID', primary_key=True)
     uuid = models.CharField(db_column='OfficerUUID',
                             max_length=36, default=uuid.uuid4, unique=True)
-    code = models.CharField(db_column='Code', max_length=8)
+    code = models.CharField(db_column='Code', max_length=CoreConfig.user_username_and_code_length_limit)
     last_name = models.CharField(db_column='LastName', max_length=100)
     other_names = models.CharField(db_column='OtherNames', max_length=100)
     dob = models.DateField(db_column='DOB', blank=True, null=True)
     phone = models.CharField(db_column='Phone', max_length=50, blank=True, null=True)
     location = models.ForeignKey('location.Location', models.DO_NOTHING, db_column='LocationId', blank=True, null=True)
     substitution_officer = models.ForeignKey('self', models.DO_NOTHING, db_column='OfficerIDSubst', blank=True,
                                              null=True)
     works_to = models.DateTimeField(db_column='WorksTo', blank=True, null=True)
-    veo_code = models.CharField(db_column='VEOCode', max_length=8, blank=True, null=True)
+    veo_code = models.CharField(db_column='VEOCode', max_length=CoreConfig.user_username_and_code_length_limit,
+                                blank=True, null=True)
     veo_last_name = models.CharField(db_column='VEOLastName', max_length=100, blank=True, null=True)
     veo_other_names = models.CharField(db_column='VEOOtherNames', max_length=100, blank=True, null=True)
     veo_dob = models.DateField(db_column='VEODOB', blank=True, null=True)
     veo_phone = models.CharField(db_column='VEOPhone', max_length=25, blank=True, null=True)
     audit_user_id = models.IntegerField(db_column='AuditUserID')
     # rowid = models.TextField(db_column='RowID', blank=True, null=True)   This field type is a guess.
     email = models.CharField(db_column='EmailId', max_length=200, blank=True, null=True)
@@ -698,37 +722,37 @@
         return False
 
     @property
     def officer_allowed_locations(self):
         """
         Returns uuid of all locations allowed for given officer
         """
-        from location.models import OfficerVillage
+        from location.models import OfficerVillage, Location
         villages = OfficerVillage.objects\
             .filter(officer=self, validity_to__isnull=True)
         all_allowed_uuids = []
         for village in villages:
             allowed_uuids = [village.location.uuid]
             parent = village.location.parent
             while parent is not None:
                 allowed_uuids.append(parent.uuid)
                 parent = parent.parent
             all_allowed_uuids.extend(allowed_uuids)
-        return all_allowed_uuids
+        return Location.objects.filter(uuid__in=all_allowed_uuids)
 
     @classmethod
     def get_queryset(cls, queryset, user):
         if isinstance(user, ResolveInfo):
             user = user.context.user
         if settings.ROW_SECURITY and user.is_anonymous:
             return queryset.filter(id=-1)
         return queryset
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblOfficer'
 
 
 class MutationLog(UUIDModel):
     """
     Maintains a log of every mutation requested along with its status. It is used to reply
     immediately to the client and have longer processing in the various backend modules.
@@ -1019,7 +1043,55 @@
 class UserMutation(UUIDModel, ObjectMutation):
     core_user = models.ForeignKey(User, models.CASCADE, related_name='mutations')
     mutation = models.ForeignKey(MutationLog, models.DO_NOTHING, related_name='users')
 
     class Meta:
         managed = True
         db_table = "core_UserMutation"
+
+
+def _get_default_expire_date():
+    return py_datetime.now() + timedelta(days=1)
+
+
+def _query_export_path(instance, filename):
+    # file will be uploaded to MEDIA_ROOT/user_<id>/<filename>
+    return F'query_exports/user_{instance.user.uuid}/{filename}'
+
+
+class ExportableQueryModel(models.Model):
+    name = models.CharField(max_length=255)
+    model = models.CharField(max_length=255)
+    content = models.FileField(upload_to=_query_export_path)
+
+    user = models.ForeignKey(
+        User, db_column="User", related_name='data_exports',
+        on_delete=models.deletion.DO_NOTHING, null=False)
+
+    sql_query = models.TextField()
+    create_date = DateTimeField(db_column='DateCreated', default=py_datetime.now)
+    expire_date = DateTimeField(db_column='DateExpiring', default=_get_default_expire_date)
+    is_deleted = models.BooleanField(default=False)
+
+    @staticmethod
+    def create_csv_export(qs, values, user, column_names=None,
+                          patches=None):
+        if patches is None:
+            patches = []
+        sql = qs.query.sql_with_params()
+        content = DataFrame.from_records(qs.values_list(*values))
+        content.columns = values
+        for patch in patches:
+            content = patch(content)
+
+        content.columns = column_names or values
+        filename = F"{uuid.uuid4()}.csv"
+        content = ContentFile(content.to_csv(), filename)
+        export = ExportableQueryModel(
+            name=filename,
+            model=qs.model,
+            content=content,
+            user=user,
+            sql_query=sql,
+        )
+        export.save()
+        return export
```

### Comparing `openimis-be-core-1.5.0/core/scheduler.py` & `openimis-be-core-1.5.1/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/schema.py` & `openimis-be-core-1.5.1/core/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import decimal
 import json
 import logging
 import re
 import sys
 import uuid
+
+import graphene
+from django.utils.translation import gettext as _
 from copy import copy
 from datetime import datetime as py_datetime
 from functools import reduce
 from django.utils.translation import gettext_lazy
 from graphene.types.generic import GenericScalar
 from graphql_jwt.mutations import JSONWebTokenMutation, mixins
 import graphene_django_optimizer as gql_optimizer
@@ -23,26 +26,29 @@
 from core.tasks import openimis_mutation_async
 from django import dispatch
 from django.conf import settings
 from django.contrib.auth.models import AnonymousUser
 from django.core.exceptions import ValidationError, PermissionDenied
 from django.core.serializers.json import DjangoJSONEncoder
 from django.db import transaction
-from django.db.models import Q
+from django.db.models import Q, Count
 from django.db.models.expressions import RawSQL
 from django.http import HttpRequest
 from django.utils import translation
 from graphene.utils.str_converters import to_snake_case, to_camel_case
 from graphene_django.filter import DjangoFilterConnectionField
 import graphql_jwt
-from typing import Optional
+from typing import Optional, List, Dict, Any
 
 from .apps import CoreConfig
 from .gql_queries import *
+from .utils import flatten_dict
 from .models import ModuleConfiguration, FieldControl, MutationLog, Language, RoleMutation, UserMutation
+from .services.roleServices import check_role_unique_name
+from .services.userServices import check_user_unique_email
 from .validation.obligatoryFieldValidation import validate_payload_for_obligatory_fields
 
 MAX_SMALLINT = 32767
 MIN_SMALLINT = -32768
 
 core = sys.modules["core"]
 
@@ -168,15 +174,15 @@
     class Input:
         client_mutation_label = graphene.String(max_length=255, required=False)
         client_mutation_details = graphene.List(graphene.String)
         mutation_extensions = ParsedJSONString(
             description="Extension data to be used by signals. Will not be pushed to mutation implementation.")
 
     @classmethod
-    def async_mutate(cls, user, **data) -> Optional[str]:
+    def async_mutate(cls, user, **data) -> List[Dict[str, Any]]:
         """
         This method has to be overridden in the subclasses to implement the actual mutation.
         The response should contain a boolean for success and an error message that will be saved into the DB
         :param user: contains the logged user or None
         :param data: all parameters passed to the mutation
         :return: error_message if None is returned, the response is considered to be a success
         """
@@ -259,16 +265,19 @@
                     error_messages = cls.async_mutate(
                         info.context.user if info.context and info.context.user else None,
                         **mutation_data)
                     if not error_messages:
                         logger.debug("[OpenIMISMutation %s] marked as successful", mutation_log.id)
                         mutation_log.mark_as_successful()
                     else:
+                        exceptions = [message.pop("exc") for message in error_messages if "exc" in message]
                         errors_json = json.dumps(error_messages)
                         logger.error("[OpenIMISMutation %s] marked as failed: %s", mutation_log.id, errors_json)
+                        for exc in exceptions:
+                            logger.error("[OpenIMISMutation %s] Exception:", mutation_log.id, exc_info=exc)
                         mutation_log.mark_as_failed(errors_json)
                 except BaseException as exc:
                     error_messages = exc
                     logger.error("async_mutate threw an exception. It should have gotten this far.", exc_info=exc)
                     # Record the failure of the mutation but don't include details for security reasons
                     mutation_log.mark_as_failed(f"The mutation threw a {type(exc)}, check logs for details")
                 logger.debug("[OpenIMISMutation %s] send post mutation signal", mutation_log.id)
@@ -336,14 +345,16 @@
             qs = qs.order_by(*snake_order)
         return qs
 
     @classmethod
     def resolve_queryset(
             cls, connection, iterable, info, args, filtering_args, filterset_class
     ):
+        if not info.context.user.is_authenticated:
+            raise PermissionDenied(_("unauthorized"))
         qs = super(DjangoFilterConnectionField, cls).resolve_queryset(
             connection, iterable, info, args
         )
         filter_kwargs = {k: v for k, v in args.items() if k in filtering_args}
         qs = filterset_class(data=filter_kwargs, queryset=qs, request=info.context).qs
 
         return OrderedDjangoFilterConnectionField.orderBy(qs, args)
@@ -437,21 +448,23 @@
         other_names=graphene.String(description="partial match, case insensitive"),
         phone=graphene.String(description="exact match on phone number"),
         email=graphene.String(description="exact match on email address"),
         role_id=graphene.Int(),
         roles=graphene.List(of_type=graphene.Int),
         health_facility_id=graphene.Int(description="Base health facility ID (not UUID!)"),
         region_id=graphene.Int(),
+        region_ids=graphene.List(of_type=graphene.Int),
         district_id=graphene.Int(),
         municipality_id=graphene.Int(),
         village_id=graphene.Int(),
         birth_date_from=graphene.Date(),
         birth_date_to=graphene.Date(),
         user_types=graphene.List(of_type=UserTypeEnum),
         language=graphene.String(),
+        showHistory=graphene.Boolean(),
         str=graphene.String(description="text search that will check username, last name, other names and email"),
         description="This interface provides access to the various types of users in openIMIS. The main resource"
                     "is limited to a username and refers either to a TechnicalUser or InteractiveUser. Only the latter"
                     "is exposed in GraphQL. There are also optional links to ClaimAdministrator and Officer depending"
                     "on the setup. BEWARE, fetching these links is costly as there is no direct database link between"
                     "these entities and there are retrieved one by one. Do not fetch them for large lists if you can"
                     "avoid it. The showHistory is acting on the InteractiveUser, avoid mixing with Officer or "
@@ -463,20 +476,79 @@
     enrolment_officers = OrderedDjangoFilterConnectionField(
         OfficerGQLType,
         str=graphene.String(
             description="text search that will check username, last name, other names and email"
         ),
     )
 
+    substitution_enrolment_officers = OrderedDjangoFilterConnectionField(
+        OfficerGQLType,
+        villages_uuids=graphene.List(
+            graphene.NonNull(graphene.String),
+            description="List of villages to be required for substituion officers"),
+        officer_uuid=graphene.String(
+            required=False,
+            description="Current officer uuid to be excluded from substitution list."),
+        str=graphene.String(
+            required=False,
+            description="Query that will return possible EO replacements."
+        ),
+    )
+
     modules_permissions = graphene.Field(
         ModulePermissionsListGQLType,
     )
 
     languages = graphene.List(LanguageGQLType)
 
+    validate_username = graphene.Field(
+        graphene.Boolean,
+        username=graphene.String(required=True),
+        description="Checks that the specified username is unique."
+    )
+
+    validate_user_email = graphene.Field(
+        graphene.Boolean,
+        user_email=graphene.String(required=True),
+        description="Checks that the specified user email is unique."
+    )
+
+    validate_role_name = graphene.Field(
+        graphene.Boolean,
+        role_name=graphene.String(required=True),
+        description="Checks that the specified role name is unique."
+    )
+
+    username_length = graphene.Int()
+
+    def resolve_username_length(self, info, **kwargs):
+        if not info.context.user.has_perms(CoreConfig.gql_query_users_perms):
+            raise PermissionDenied(_("unauthorized"))
+        return CoreConfig.username_code_length
+
+    def resolve_validate_role_name(self, info, **kwargs):
+        if not info.context.user.has_perms(CoreConfig.gql_query_roles_perms):
+            raise PermissionDenied(_("unauthorized"))
+        errors = check_role_unique_name(name=kwargs['role_name'])
+        return False if errors else True
+
+    def resolve_validate_username(self, info, **kwargs):
+        if not info.context.user.has_perms(CoreConfig.gql_query_users_perms):
+            raise PermissionDenied(_("unauthorized"))
+        if User.objects.filter(username=kwargs['username']).exists():
+            return False
+        else:
+            return True
+
+    def resolve_validate_user_email(self, info, **kwargs):
+        if not info.context.user.has_perms(CoreConfig.gql_query_users_perms):
+            raise PermissionDenied(_("unauthorized"))
+        errors = check_user_unique_email(user_email=kwargs['user_email'])
+        return False if errors else True
+
     def resolve_enrolment_officers(self, info, **kwargs):
         from .models import Officer
 
         if not info.context.user.has_perms(
                 CoreConfig.gql_query_enrolment_officers_perms
         ):
             raise PermissionError("Unauthorized")
@@ -489,14 +561,46 @@
                     Q(code__icontains=search)
                     | Q(last_name__icontains=search)
                     | Q(other_names__icontains=search)
                 ),
                 info,
             )
 
+    def resolve_substitution_enrolment_officers(self, info, **kwargs):
+        from .models import Officer
+
+        if not info.context.user.has_perms(
+                CoreConfig.gql_query_enrolment_officers_perms):
+            raise PermissionError("Unauthorized")
+
+        queryset = Officer.objects
+
+        villages_uuids = kwargs.get('villages_uuids', None)
+        if not villages_uuids:
+            return []
+
+        officer_uuid = kwargs.get('officer_uuid', None)
+        if officer_uuid:
+            queryset = queryset.exclude(uuid=officer_uuid)
+
+        query_str = kwargs.get('str', None)
+        if query_str:
+            queryset = queryset.filter(Q(code__istartswith=query_str)
+                                       | Q(last_name__istartswith=query_str)
+                                       | Q(other_names__istartswith=query_str)
+                                       | Q(email__istartswith=query_str))
+
+        return queryset.prefetch_related('officer_villages') \
+            .annotate(nb_village=Count('officer_villages')) \
+            .filter(nb_village__gte=len(villages_uuids),
+                    officer_villages__location__uuid__in=villages_uuids,
+                    validity_to__isnull=True,
+                    officer_villages__validity_to__isnull=True,
+                    officer_villages__location__validity_to__isnull=True)
+
     def resolve_interactive_users(self, info, **kwargs):
         if not info.context.user.has_perms(CoreConfig.gql_query_users_perms):
             raise PermissionError("Unauthorized")
         filters = []
         query = InteractiveUser.objects
 
         client_mutation_id = kwargs.get("client_mutation_id", None)
@@ -521,22 +625,28 @@
 
     def resolve_eo_obligatory_fields(self, info):
         if info.context.user.is_authenticated:
             return CoreConfig.fields_controls_eo
         return None
 
     def resolve_users(self, info, email=None, last_name=None, other_names=None, phone=None,
-                      role_id=None, roles=None, health_facility_id=None, region_id=None, district_id=None,
-                      municipality_id=None, birth_date_from=None, birth_date_to=None, user_types=None, language=None,
-                      village_id=None, **kwargs):
+                      role_id=None, roles=None, health_facility_id=None, region_id=None,
+                      district_id=None, municipality_id=None, birth_date_from=None, birth_date_to=None,
+                      user_types=None, language=None, village_id=None, region_ids=None, **kwargs):
         if not info.context.user.has_perms(CoreConfig.gql_query_users_perms):
             raise PermissionError("Unauthorized")
 
         user_filters = []
         user_query = User.objects.exclude(t_user__isnull=False)
+
+        show_history = kwargs.get('showHistory', False)
+        if not show_history and not kwargs.get('uuid', None):
+            active_users_ids = [user.id for user in user_query if user.is_active]
+            user_filters.append(Q(id__in=active_users_ids))
+
         text_search = kwargs.get("str")  # Poorly chosen name, avoid of shadowing "str"
         if text_search:
             user_filters.append(Q(username__icontains=text_search) |
                                 Q(i_user__last_name__icontains=text_search) |
                                 Q(officer__last_name__icontains=text_search) |
                                 Q(claim_admin__last_name__icontains=text_search) |
                                 Q(i_user__other_names__icontains=text_search) |
@@ -584,16 +694,20 @@
                                 Q(claim_admin__dob__lte=birth_date_to))
         if role_id:
             user_filters.append(Q(i_user__user_roles__role_id=role_id) &
                                 Q(i_user__user_roles__validity_to__isnull=True))
         if roles:
             user_filters.append(Q(i_user__user_roles__role_id__in=roles) &
                                 Q(i_user__user_roles__validity_to__isnull=True))
+
         if region_id:
             user_filters.append(Q(i_user__userdistrict__location__parent_id=region_id))
+        elif region_ids:
+            user_filters.append(Q(i_user__userdistrict__location__parent_id__in=region_ids))
+
         if district_id:
             user_filters.append(Q(i_user__userdistrict__location_id=district_id))
         if municipality_id:
             user_filters.append(Q(officer__officer_villages__location__parent_id=municipality_id))
         if village_id:
             user_filters.append(Q(officer__officer_villages__location_id=village_id))
 
@@ -604,15 +718,15 @@
                 UT_TECHNICAL: Q(t_user__isnull=False),
                 UT_CLAIM_ADMIN: Q(claim_admin__isnull=False),
             }
             user_filters.append(reduce(lambda a, b: a | b, [ut_conditions[x] for x in user_types]))
 
         # Do NOT use the query optimizer here ! It would make the t_user, officer etc as deferred fields if they are not
         # explicitly requested in the GraphQL response. However, this prevents the dynamic remapping of the User object.
-        return user_query.filter(*user_filters)
+        return user_query.filter(*user_filters).distinct()
 
     def resolve_role(self, info, **kwargs):
         if not info.context.user.has_perms(CoreConfig.gql_query_roles_perms):
             raise PermissionError("Unauthorized")
         filters = []
         query = Role.objects
 
@@ -657,29 +771,30 @@
 
     def resolve_modules_permissions(self, info, **kwargs):
         if not info.context.user.has_perms(CoreConfig.gql_query_roles_perms):
             raise PermissionError("Unauthorized")
         excluded_app = [
             "health_check.cache", "health_check", "health_check.db",
             "test_without_migrations", "test_without_migrations",
-            "rules", "graphene_django", "rest_framework", "rest_framework_rules",
+            "rules", "graphene_django", "rest_framework",
             "health_check.storage", "channels", "graphql_jwt.refresh_token.apps.RefreshTokenConfig"
         ]
         all_apps = [app for app in settings.INSTALLED_APPS if not app.startswith("django") and app not in excluded_app]
         config = []
         for app in all_apps:
             apps = __import__(f"{app}.apps")
             is_default_cfg = hasattr(apps.apps, 'DEFAULT_CFG')
             is_defaulf_config = hasattr(apps.apps, 'DEFAULT_CONFIG')
             if is_default_cfg or is_defaulf_config:
                 if is_defaulf_config:
                     config_dict = ModuleConfiguration.get_or_default(f"{app}", apps.apps.DEFAULT_CONFIG)
                 else:
                     config_dict = ModuleConfiguration.get_or_default(f"{app}", apps.apps.DEFAULT_CFG)
                 permission = []
+                config_dict = flatten_dict(config_dict)
                 for key, value in config_dict.items():
                     if key.endswith("_perms"):
                         if isinstance(value, list):
                             for val in value:
                                 permission.append(PermissionOpenImisGQLType(
                                     perms_name=key,
                                     perms_value=val,
@@ -709,14 +824,16 @@
         )
         layer = kwargs.get('layer')
         if layer is not None:
             crits = (*crits, Q(layer=layer))
         return ModuleConfiguration.objects.prefetch_related('controls').filter(*crits)
 
     def resolve_languages(self, info, **kwargs):
+        if not info.context.user.is_authenticated:
+            raise PermissionDenied(_("unauthorized"))
         return Language.objects.order_by('sort_order').all()
 
 
 class RoleBase:
     id = graphene.Int(required=False, read_only=True)
     uuid = graphene.String(required=False)
     name = graphene.String(required=True, max_length=50)
@@ -852,14 +969,16 @@
     @classmethod
     def async_mutate(cls, user, **data):
         try:
             if type(user) is AnonymousUser or not user.id:
                 raise ValidationError("mutation.authentication_required")
             if not user.has_perms(CoreConfig.gql_mutation_create_roles_perms):
                 raise PermissionDenied("unauthorized")
+            if check_role_unique_name(data.get('name', None)):
+                raise ValidationError("mutation.duplicate_of_role_name")
             from core.utils import TimeUtils
             data['validity_from'] = TimeUtils.now()
             data['audit_user_id'] = user.id_for_audit
             update_or_create_role(data, user)
             return None
         except Exception as exc:
             return [
@@ -884,14 +1003,16 @@
         try:
             if type(user) is AnonymousUser or not user.id:
                 raise ValidationError("mutation.authentication_required")
             if not user.has_perms(CoreConfig.gql_mutation_update_roles_perms):
                 raise PermissionDenied("unauthorized")
             if 'uuid' not in data:
                 raise ValidationError("There is no uuid in updateMutation input!")
+            if check_role_unique_name(data.get('name', None), data['uuid']):
+                raise ValidationError("mutation.duplicate_of_role_name")
             data['audit_user_id'] = user.id_for_audit
             update_or_create_role(data, user)
             return None
         except Exception as exc:
             return [
                 {
                     'message': "core.mutation.failed_to_update_role",
@@ -931,15 +1052,15 @@
             role = Role.objects \
                 .filter(uuid=role_uuid) \
                 .first()
             if role is None:
                 errors.append({
                     'title': role,
                     'list': [{'message':
-                                  "role.validation.id_does_not_exist" % {'id': role_uuid}}]
+                              "role.validation.id_does_not_exist" % {'id': role_uuid}}]
                 })
                 continue
             errors += set_role_deleted(role)
         if len(errors) == 1:
             errors = errors[0]['list']
         return errors
 
@@ -1027,14 +1148,16 @@
         pass
 
     @classmethod
     def async_mutate(cls, user, **data):
         try:
             if type(user) is AnonymousUser or not user.id:
                 raise ValidationError("mutation.authentication_required")
+            if User.objects.filter(username=data['username']).exists():
+                raise ValidationError("User with this user name already exists.")
             if not user.has_perms(CoreConfig.gql_mutation_create_users_perms):
                 raise PermissionDenied("unauthorized")
             from core.utils import TimeUtils
             data['validity_from'] = TimeUtils.now()
             data['audit_user_id'] = user.id_for_audit
             update_or_create_user(data, user)
             return None
@@ -1095,29 +1218,48 @@
             user = User.objects \
                 .filter(id=user_uuid) \
                 .first()
             if user is None:
                 errors.append({
                     'title': user,
                     'list': [{'message':
-                                  "user.validation.id_does_not_exist" % {'id': user_uuid}}]
+                              "user.validation.id_does_not_exist" % {'id': user_uuid}}]
                 })
                 continue
             errors += set_user_deleted(user)
         if len(errors) == 1:
             errors = errors[0]['list']
         return errors
 
 
 @transaction.atomic
 @validate_payload_for_obligatory_fields(CoreConfig.fields_controls_user, 'data')
 def update_or_create_user(data, user):
     client_mutation_id = data.get("client_mutation_id", None)
     # client_mutation_label = data.get("client_mutation_label", None)
 
+    incoming_email = data.get('email')
+    current_user = InteractiveUser.objects.filter(user__id=data['uuid']).first()
+
+    current_email = current_user.email if current_user else None
+
+    if incoming_email:
+        if not check_email_validity(incoming_email):
+            raise ValidationError(_("mutation.user_email_invalid"))
+        if current_email != incoming_email:
+            if check_user_unique_email(user_email=data['email']):
+                raise ValidationError(_("mutation.user_email_duplicated"))
+    else:
+        raise ValidationError(_("mutation.user_no_email_provided"))
+
+    username = data.get('username')
+
+    if len(username) > CoreConfig.username_code_length:
+        raise ValidationError(_("mutation.user_username_too_long"))
+
     if "client_mutation_id" in data:
         data.pop('client_mutation_id')
     if "client_mutation_label" in data:
         data.pop('client_mutation_label')
     user_uuid = data.pop('uuid') if 'uuid' in data else None
 
     if UT_INTERACTIVE in data["user_types"]:
@@ -1132,21 +1274,35 @@
         officer, officer_created = None, False
     if UT_CLAIM_ADMIN in data["user_types"]:
         claim_admin, claim_admin_created = create_or_update_claim_admin(
             user_uuid, data, user.id_for_audit, UT_INTERACTIVE in data["user_types"])
     else:
         claim_admin, claim_admin_created = None, False
     core_user, core_user_created = create_or_update_core_user(
-        user_uuid=user_uuid, username=data["username"], i_user=i_user, officer=officer, claim_admin=claim_admin)
+        user_uuid=user_uuid, username=username, i_user=i_user, officer=officer, claim_admin=claim_admin)
 
     if client_mutation_id:
         UserMutation.object_mutated(user, core_user=core_user, client_mutation_id=client_mutation_id)
     return core_user
 
 
+def check_email_validity(email):
+    # checks if string is a valid email address
+    # using regex provided in the HTML5 standard
+    # it omits some RFC recommendations by design
+    # https://html.spec.whatwg.org/multipage/input.html#valid-e-mail-address
+    import re
+    regex = re.compile(
+        r"^[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+@[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9]"
+        r"(?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)*$")
+    if not re.fullmatch(regex, email):
+        return False
+    return True
+
+
 def set_user_deleted(user):
     try:
         if user.i_user:
             user.i_user.delete_history()
         if user.t_user:
             user.t_user.delete_history()
         if user.officer:
```

### Comparing `openimis-be-core-1.5.0/core/security.py` & `openimis-be-core-1.5.1/core/security.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/serializers.py` & `openimis-be-core-1.5.1/core/serializers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/service_signals.py` & `openimis-be-core-1.5.1/core/service_signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 
 class RegisteredServiceSignal:
 
     def __init__(self, providing_args=None):
         """
         Due to how python manage class prototypes, there's a chance that class definition using register_service_signal
-        will not be loaded until first import of given class. Therefore it's likely that binding function responsible
+        will not be loaded until first import of given class. Therefore, it's likely that binding function responsible
         for loading functions called before/after signal will be invoked before signal register. In this case functions
-        are queued and connected to actual signal after the registration. Whether or not registration took place
+        are queued and connected to actual signal after the registration. Whether registration took place
         is defined by providing_args. If argument is None, signal is considered not registered.
         """
         self.__signal_results = {'before': None, 'after': None}
         self.__connection_queue = {type_: queue.Queue() for type_ in ServiceSignalBindType}
         self.__signals_before = []
         self.__signals_after = []
```

### Comparing `openimis-be-core-1.5.0/core/services/base.py` & `openimis-be-core-1.5.1/core/services/base.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/services/userServices.py` & `openimis-be-core-1.5.1/core/services/userServices.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,29 +188,27 @@
 
 
 def create_or_update_core_user(user_uuid, username, i_user=None, t_user=None, officer=None, claim_admin=None):
     if user_uuid:
         # This intentionally fails if the provided uuid doesn't exist as we don't want clients to set it
         user = User.objects.get(id=user_uuid)
         # There is no history to save for User
-        if user.username != username:
-            logger.warning("Ignored attempt to change the username of %s from %s to %s. This is not supported",
-                           user_uuid, user.username, username)
         created = False
     elif username:
         user = User.objects.filter(username=username).first()
         created = False
     else:
         user = None
         created = False
 
     if not user:
         user = User(username=username)
         created = True
-
+    if username:
+        user.username = username
     if i_user:
         user.i_user = i_user
     if t_user:
         user.t_user = t_user
     if officer:
         user.officer = officer
     if claim_admin:
@@ -239,14 +237,20 @@
     if default_token_generator.check_token(user, token):
         user.set_password(password)
         user.save()
     else:
         raise ValidationError("Invalid Token")
 
 
+def check_user_unique_email(user_email):
+    if InteractiveUser.objects.filter(email=user_email, validity_to__isnull=True).exists():
+        return [{"message": "User email %s already exists" % user_email}]
+    return []
+
+
 def reset_user_password(request, username):
     user = User.objects.get(username=username)
     user.clear_refresh_tokens()
 
     if not user.email:
         raise ValidationError(
             f"User {username} cannot reset password because he has no email address"
```

### Comparing `openimis-be-core-1.5.0/core/services/utils/serviceUtils.py` & `openimis-be-core-1.5.1/core/services/utils/serviceUtils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/signals.py` & `openimis-be-core-1.5.1/core/signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     Decorator for registering signals for service. Two signals will be created: one before service and one after.
     Signals are stored in core.signals.REGISTERED_SERVICE_SIGNALS as RegisteredServiceSignal.
     See RegisteredServiceSignal class definition for more information regarding when signals are registered
     and connected. Signal receivers output is stored in RegisteredServiceSignal.signal_results. Results are
     overridden after very call.
 
     Example use:
-        @register_service_signal('create_policy', PolicyServiceClass):
+        @register_service_signal('create_policy'):
         def create_policy(self, *args, **kwargs)
             ...
 
         Will create new RegisteredServiceSignal instance available from  REGISTERED_SERVICE_SIGNALS['create_policy'].
         Signal name has to be unique.
 
     """
@@ -81,15 +81,15 @@
 
     return decorator
 
 
 def bind_service_signal(signal_name: str, func: Callable,
                         bind_type: ServiceSignalBindType = ServiceSignalBindType.BEFORE_AND_AFTER):
     """
-    By default binding is done after modules are loaded, with same similar approach as for graphql.
+    By default, binding is done after modules are loaded, with same similar approach as for graphql.
     Main OpenIMIS backend is crawling through modules searching for bind_service_signals function
     in module_name.signals path. In most cases function connected to signal will be loaded before signals are
     registered. They're queued and connected after signal definition is provided.
 
     Example:
         Content of openimis-be-invoice_py/invoice/signals.py:
         from core.signals import bind_service_signal
```

### Comparing `openimis-be-core-1.5.0/core/tasks.py` & `openimis-be-core-1.5.1/core/tasks.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/test_helpers.py` & `openimis-be-core-1.5.1/core/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/test_models.py` & `openimis-be-core-1.5.1/core/test_models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/test_security.py` & `openimis-be-core-1.5.1/core/test_security.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/test_services.py` & `openimis-be-core-1.5.1/core/test_services.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/test_utils.py` & `openimis-be-core-1.5.1/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/utils.py` & `openimis-be-core-1.5.1/core/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import core
 import graphene
 from django.db.models import Q
 from django.utils.translation import gettext as _
 import logging
 from django.apps import apps
+from django.core.exceptions import PermissionDenied
 
 
 logger = logging.getLogger(__file__)
 
 __all__ = [
     "TimeUtils",
     "full_class_name",
@@ -122,14 +123,25 @@
         else:
             filters = []
     else:
         filters = [*filter_validity_business_model(**kwargs)]
     return filters
 
 
+def flatten_dict(d, parent_key='', sep='_'):
+    items = []
+    for k, v in d.items():
+        new_key = parent_key + sep + k if parent_key else k
+        if isinstance(v, dict):
+            items.extend(flatten_dict(v, new_key, sep=sep).items())
+        else:
+            items.append((new_key, v))
+    return dict(items)
+
+
 def filter_is_deleted(arg='is_deleted', **kwargs):
     is_deleted = kwargs.get(arg)
     if is_deleted is None:
         is_deleted = False
     return (
         Q(is_deleted=is_deleted)
     )
@@ -189,17 +201,21 @@
     class Meta:
         abstract = True
 
     total_count = graphene.Int()
     edge_count = graphene.Int()
 
     def resolve_total_count(self, info, **kwargs):
+        if not info.context.user.is_authenticated:
+            raise PermissionDenied(_("unauthorized"))
         return self.length
 
     def resolve_edge_count(self, info, **kwargs):
+        if not info.context.user.is_authenticated:
+            raise PermissionDenied(_("unauthorized"))
         return len(self.edges)
 
 
 def get_scheduler_method_ref(name):
     """
     Use to retrieve the method reference from a str name. This is necessary when the module cannot be imported from
     that location.
```

### Comparing `openimis-be-core-1.5.0/core/validation/base.py` & `openimis-be-core-1.5.1/core/validation/base.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/validation/obligatoryFieldValidation.py` & `openimis-be-core-1.5.1/core/validation/obligatoryFieldValidation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/validation/uniqueCodeValidationMixin.py` & `openimis-be-core-1.5.1/core/validation/uniqueCodeValidationMixin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/websocket/abstract_websocket_client.py` & `openimis-be-core-1.5.1/core/websocket/abstract_websocket_client.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/websocket/async_websocket_client.py` & `openimis-be-core-1.5.1/core/websocket/async_websocket_client.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/core/websocket/base_websocket_client.py` & `openimis-be-core-1.5.1/core/websocket/base_websocket_client.py`

 * *Files identical despite different names*

### Comparing `openimis-be-core-1.5.0/openimis_be_core.egg-info/PKG-INFO` & `openimis-be-core-1.5.1/openimis_be_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-core
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Core reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-core-1.5.0/openimis_be_core.egg-info/SOURCES.txt` & `openimis-be-core-1.5.1/openimis_be_core.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -38,19 +38,24 @@
 core/datetimes/ad_datetime.py
 core/datetimes/ne_datetime.py
 core/datetimes/shared.py
 core/datetimes/test_ad_datetime.py
 core/datetimes/test_ne_datetime.py
 core/datetimes/test_shared.py
 core/gql/__init__.py
+core/gql/custom_lookup.py
+core/gql/export_mixin.py
 core/gql/gql_mutations/__init__.py
 core/gql/gql_mutations/base_mutation.py
 core/gql/gql_mutations/exceptions.py
 core/gql/gql_mutations/input_types.py
 core/gql/gql_mutations/mutation_by_filter.py
+core/migration_to_history_model/__init__.py
+core/migration_to_history_model/create_temp_tables.py
+core/migration_to_history_model/patch_table_data.py
 core/migrations/0001_initial.py
 core/migrations/0002_auto_20190726_0701.py
 core/migrations/0003_control_mutationlog.py
 core/migrations/0004_auto_20190830_1625.py
 core/migrations/0005_group_usergroup.py
 core/migrations/0006_fieldcontrol.py
 core/migrations/0007_auto_20191008_0923.py
@@ -59,17 +64,23 @@
 core/migrations/0010_rolemutation.py
 core/migrations/0011_auto_20210324_1528.py
 core/migrations/0012_users_officers_admins.py
 core/migrations/0013_users_api.py
 core/migrations/0014_users.py
 core/migrations/0015_missing_roles.py
 core/migrations/0016_add_last_login_on_interactive_user.py
+core/migrations/0017_exportablequerymodel.py
+core/migrations/0018_auto_20230318_1551.py
+core/migrations/0019_extended_field.py
+core/migrations/0020_add_missing_fields_to_django_scheme.py
+core/migrations/0021_set_managed_to_true.py
 core/migrations/__init__.py
 core/services/__init__.py
 core/services/base.py
+core/services/roleServices.py
 core/services/userServices.py
 core/services/utils/__init__.py
 core/services/utils/serviceUtils.py
 core/templates/password_reset.txt
 core/validation/__init__.py
 core/validation/base.py
 core/validation/objectExistsValidationMixin.py
```

### Comparing `openimis-be-core-1.5.0/setup.py` & `openimis-be-core-1.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,25 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-core',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Core reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
     author_email='xgillmann@bluesquarehub.com',
     install_requires=[
+        'isodate',
         'django',
         'django-db-signals',
         'djangorestframework',
         'cached-property',
         'nepalicalendar',
         'django-simple-history',
         'django-dirtyfields',
```

