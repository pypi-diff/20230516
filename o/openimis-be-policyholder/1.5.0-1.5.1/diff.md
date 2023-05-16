# Comparing `tmp/openimis-be-policyholder-1.5.0.tar.gz` & `tmp/openimis-be-policyholder-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-policyholder-1.5.0.tar", last modified: Fri Nov 11 08:12:08 2022, max compression
+gzip compressed data, was "openimis-be-policyholder-1.5.1.tar", last modified: Tue May 16 21:38:38 2023, max compression
```

## Comparing `openimis-be-policyholder-1.5.0.tar` & `openimis-be-policyholder-1.5.1.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:08.149729 openimis-be-policyholder-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5583 2022-11-11 08:12:08.149729 openimis-be-policyholder-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4843 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:08.141728 openimis-be-policyholder-1.5.0/openimis_be_policyholder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5583 2022-11-11 08:12:08.000000 openimis-be-policyholder-1.5.0/openimis_be_policyholder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2044 2022-11-11 08:12:08.000000 openimis-be-policyholder-1.5.0/openimis_be_policyholder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 08:12:08.000000 openimis-be-policyholder-1.5.0/openimis_be_policyholder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-11-11 08:12:08.000000 openimis-be-policyholder-1.5.0/openimis_be_policyholder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-11 08:12:08.000000 openimis-be-policyholder-1.5.0/openimis_be_policyholder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:08.141728 openimis-be-policyholder-1.5.0/policyholder/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)    11346 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:08.141728 openimis-be-policyholder-1.5.0/policyholder/gql/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/gql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:08.145729 openimis-be-policyholder-1.5.0/policyholder/gql/gql_mutations/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/gql/gql_mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2295 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/gql/gql_mutations/create_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/gql/gql_mutations/delete_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     5741 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/gql/gql_mutations/input_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/gql/gql_mutations/replace_mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/gql/gql_mutations/update_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     4268 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/gql/gql_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:08.145729 openimis-be-policyholder-1.5.0/policyholder/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    21878 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0002_auto_20201214_1237.py
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0003_auto_20201214_1239.py
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0004_auto_20201214_1302.py
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0005_auto_20210111_1254.py
--rw-r--r--   0 runner    (1001) docker     (121)     3235 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0006_policyholdercontributionplanmutation_policyholderinsureemutation_policyholdermutation_policyholderus.py
--rw-r--r--   0 runner    (1001) docker     (121)     7267 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0007_auto_20210118_0927.py
--rw-r--r--   0 runner    (1001) docker     (121)     7014 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0008_auto_20210118_1109.py
--rw-r--r--   0 runner    (1001) docker     (121)     6921 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0009_auto_20210118_1127.py
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0010_auto_20210126_1040.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0011_auto_20210408_0937.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0012_auto_20210408_0949.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0013_auto_20210408_0951.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0014_auto_20210408_1007.py
--rw-r--r--   0 runner    (1001) docker     (121)      932 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0015_auto_20210624_1243.py
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/0016_policyholder_roles_for_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8381 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     9714 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    15473 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:08.145729 openimis-be-policyholder-1.5.0/policyholder/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3313 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4671 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/tests/helpers_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:08.145729 openimis-be-policyholder-1.5.0/policyholder/tests/services/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20660 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/tests/services/services_ph_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:08.149729 openimis-be-policyholder-1.5.0/policyholder/validation/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/validation/policyholder_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:11:51.000000 openimis-be-policyholder-1.5.0/policyholder/views.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 08:12:08.149729 openimis-be-policyholder-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-11-11 08:12:06.000000 openimis-be-policyholder-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:38.832294 openimis-be-policyholder-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-16 21:38:38.832294 openimis-be-policyholder-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:38.828294 openimis-be-policyholder-1.5.1/openimis_be_policyholder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-16 21:38:38.000000 openimis-be-policyholder-1.5.1/openimis_be_policyholder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-16 21:38:38.000000 openimis-be-policyholder-1.5.1/openimis_be_policyholder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:38:38.000000 openimis-be-policyholder-1.5.1/openimis_be_policyholder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-16 21:38:38.000000 openimis-be-policyholder-1.5.1/openimis_be_policyholder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 21:38:38.000000 openimis-be-policyholder-1.5.1/openimis_be_policyholder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:38.828294 openimis-be-policyholder-1.5.1/policyholder/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:38.828294 openimis-be-policyholder-1.5.1/policyholder/gql/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/gql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:38.828294 openimis-be-policyholder-1.5.1/policyholder/gql/gql_mutations/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/gql/gql_mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/gql/gql_mutations/create_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/gql/gql_mutations/delete_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/gql/gql_mutations/input_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/gql/gql_mutations/replace_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/gql/gql_mutations/update_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/gql/gql_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:38.828294 openimis-be-policyholder-1.5.1/policyholder/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    21878 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0002_auto_20201214_1237.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0003_auto_20201214_1239.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0004_auto_20201214_1302.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0005_auto_20210111_1254.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0006_policyholdercontributionplanmutation_policyholderinsureemutation_policyholdermutation_policyholderus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0007_auto_20210118_0927.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0008_auto_20210118_1109.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0009_auto_20210118_1127.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0010_auto_20210126_1040.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0011_auto_20210408_0937.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0012_auto_20210408_0949.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0013_auto_20210408_0951.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0014_auto_20210408_1007.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0015_auto_20210624_1243.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0016_policyholder_roles_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/0017_auto_20230126_0903.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:38.832294 openimis-be-policyholder-1.5.1/policyholder/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/tests/helpers_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:38.832294 openimis-be-policyholder-1.5.1/policyholder/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/tests/services/services_ph_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:38.832294 openimis-be-policyholder-1.5.1/policyholder/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/validation/permission_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/validation/policyholder_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:28.000000 openimis-be-policyholder-1.5.1/policyholder/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:38:38.832294 openimis-be-policyholder-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-16 21:38:37.000000 openimis-be-policyholder-1.5.1/setup.py
```

### Comparing `openimis-be-policyholder-1.5.0/LICENSE.md` & `openimis-be-policyholder-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/PKG-INFO` & `openimis-be-policyholder-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-policyholder
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend PolicyHolder reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-policyholder-1.5.0/README.md` & `openimis-be-policyholder-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/openimis_be_policyholder.egg-info/PKG-INFO` & `openimis-be-policyholder-1.5.1/openimis_be_policyholder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-policyholder
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend PolicyHolder reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-policyholder-1.5.0/openimis_be_policyholder.egg-info/SOURCES.txt` & `openimis-be-policyholder-1.5.1/openimis_be_policyholder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,17 @@
 policyholder/migrations/0010_auto_20210126_1040.py
 policyholder/migrations/0011_auto_20210408_0937.py
 policyholder/migrations/0012_auto_20210408_0949.py
 policyholder/migrations/0013_auto_20210408_0951.py
 policyholder/migrations/0014_auto_20210408_1007.py
 policyholder/migrations/0015_auto_20210624_1243.py
 policyholder/migrations/0016_policyholder_roles_for_admin.py
+policyholder/migrations/0017_auto_20230126_0903.py
 policyholder/migrations/__init__.py
 policyholder/tests/__init__.py
 policyholder/tests/helpers.py
 policyholder/tests/helpers_tests.py
 policyholder/tests/services/__init__.py
 policyholder/tests/services/services_ph_tests.py
 policyholder/validation/__init__.py
+policyholder/validation/permission_validation.py
 policyholder/validation/policyholder_validation.py
```

### Comparing `openimis-be-policyholder-1.5.0/policyholder/apps.py` & `openimis-be-policyholder-1.5.1/policyholder/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/gql/gql_mutations/create_mutations.py` & `openimis-be-policyholder-1.5.1/policyholder/gql/gql_mutations/update_mutations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,82 @@
-from core.gql.gql_mutations.base_mutation import BaseMutation, BaseHistoryModelCreateMutationMixin
+from core.gql.gql_mutations.base_mutation import BaseMutation, BaseHistoryModelUpdateMutationMixin
 from core.models import InteractiveUser
+from policyholder.apps import PolicyholderConfig
 from policyholder.models import PolicyHolder, PolicyHolderInsuree, PolicyHolderContributionPlan, PolicyHolderUser
-from policyholder.gql.gql_mutations import PolicyHolderInputType, PolicyHolderInsureeInputType, \
-    PolicyHolderContributionPlanInputType, PolicyHolderUserInputType
+from policyholder.gql.gql_mutations import PolicyHolderInsureeUpdateInputType, \
+    PolicyHolderContributionPlanUpdateInputType, PolicyHolderUserUpdateInputType, PolicyHolderUpdateInputType
 from policyholder.validation import PolicyHolderValidation
+from policyholder.validation.permission_validation import PermissionValidation
 
 
-class CreatePolicyHolderMutation(BaseHistoryModelCreateMutationMixin, BaseMutation):
+class UpdatePolicyHolderMutation(BaseHistoryModelUpdateMutationMixin, BaseMutation):
     _mutation_class = "PolicyHolderMutation"
     _mutation_module = "policyholder"
     _model = PolicyHolder
 
-    class Input(PolicyHolderInputType):
+    class Input(PolicyHolderUpdateInputType):
         pass
 
     @classmethod
     def _validate_mutation(cls, user, **data):
         super()._validate_mutation(user, **data)
-        PolicyHolderValidation.validate_create(user, **data)
+        PermissionValidation.validate_perms(user, PolicyholderConfig.gql_mutation_update_policyholder_perms)
+        PolicyHolderValidation.validate_update(user, **data)
 
 
-class CreatePolicyHolderInsureeMutation(BaseHistoryModelCreateMutationMixin, BaseMutation):
+class UpdatePolicyHolderInsureeMutation(BaseHistoryModelUpdateMutationMixin, BaseMutation):
     _mutation_class = "PolicyHolderInsureeMutation"
     _mutation_module = "policyholder"
     _model = PolicyHolderInsuree
 
-    class Input(PolicyHolderInsureeInputType):
+    class Input(PolicyHolderInsureeUpdateInputType):
         pass
 
+    @classmethod
+    def _validate_mutation(cls, user, **data):
+        super()._validate_mutation(user, **data)
+        PermissionValidation.validate_perms(user, PolicyholderConfig.gql_mutation_update_policyholderinsuree_perms)
+
 
-class CreatePolicyHolderContributionPlanMutation(BaseHistoryModelCreateMutationMixin, BaseMutation):
+class UpdatePolicyHolderContributionPlanMutation(BaseHistoryModelUpdateMutationMixin, BaseMutation):
     _mutation_class = "PolicyHolderContributionPlanMutation"
     _mutation_module = "policyholder"
     _model = PolicyHolderContributionPlan
 
-    class Input(PolicyHolderContributionPlanInputType):
+    class Input(PolicyHolderContributionPlanUpdateInputType):
         pass
 
+    @classmethod
+    def _validate_mutation(cls, user, **data):
+        super()._validate_mutation(user, **data)
+        PermissionValidation.validate_perms(user, PolicyholderConfig.gql_mutation_update_policyholdercontributionplan_perms)
 
-class CreatePolicyHolderUserMutation(BaseHistoryModelCreateMutationMixin, BaseMutation):
+
+class UpdatePolicyHolderUserMutation(BaseHistoryModelUpdateMutationMixin, BaseMutation):
     _mutation_class = "PolicyHolderUserMutation"
     _mutation_module = "policyholder"
     _model = PolicyHolderUser
 
     @classmethod
     def _mutate(cls, user, **data):
-        client_mutation_id = data.get("client_mutation_id")
         if "client_mutation_id" in data:
             data.pop('client_mutation_id')
         if "client_mutation_label" in data:
             data.pop('client_mutation_label')
-        cls.create_policy_holder_user(user=user, object_data=data)
+        updated_object = cls._model.objects.filter(id=data['id']).first()
+        [setattr(updated_object, key, data[key]) for key in data]
+        cls.update_policy_holder_user(user=user, object_to_update=updated_object)
 
     @classmethod
-    def create_policy_holder_user(cls, user, object_data):
-        obj = cls._model(**object_data)
-        obj.save(username=user.username)
-        return obj
+    def update_policy_holder_user(cls, user, object_to_update):
+        object_to_update.save(username=user.username)
+        return object_to_update
 
-    class Input(PolicyHolderUserInputType):
+    class Input(PolicyHolderUserUpdateInputType):
         pass
 
+    @classmethod
+    def _validate_mutation(cls, user, **data):
+        super()._validate_mutation(user, **data)
+        PermissionValidation.validate_perms(user, PolicyholderConfig.gql_mutation_update_policyholderuser_perms)
+
+
```

### Comparing `openimis-be-policyholder-1.5.0/policyholder/gql/gql_mutations/delete_mutations.py` & `openimis-be-policyholder-1.5.1/policyholder/gql/gql_mutations/delete_mutations.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,61 @@
 from core.gql.gql_mutations import DeleteInputType
 from core.gql.gql_mutations.base_mutation import BaseDeleteMutation, BaseHistoryModelDeleteMutationMixin
+from policyholder.apps import PolicyholderConfig
 from policyholder.models import PolicyHolder, PolicyHolderInsuree, PolicyHolderContributionPlan, PolicyHolderUser
+from policyholder.validation.permission_validation import PermissionValidation
 
 
 class DeletePolicyHolderMutation(BaseHistoryModelDeleteMutationMixin, BaseDeleteMutation):
     _mutation_class = "PolicyHolderMutation"
     _mutation_module = "policyholder"
     _model = PolicyHolder
 
     class Input(DeleteInputType):
         pass
 
+    @classmethod
+    def _validate_mutation(cls, user, **data):
+        super()._validate_mutation(user, **data)
+        PermissionValidation.validate_perms(user, PolicyholderConfig.gql_mutation_delete_policyholder_perms)
+
 
 class DeletePolicyHolderInsureeMutation(BaseHistoryModelDeleteMutationMixin, BaseDeleteMutation):
     _mutation_class = "PolicyHolderInsureeMutation"
     _mutation_module = "policyholder"
     _model = PolicyHolderInsuree
 
     class Input(DeleteInputType):
         pass
 
+    @classmethod
+    def _validate_mutation(cls, user, **data):
+        super()._validate_mutation(user, **data)
+        PermissionValidation.validate_perms(user, PolicyholderConfig.gql_mutation_delete_policyholderinsuree_perms)
+
 
 class DeletePolicyHolderContributionPlanMutation(BaseHistoryModelDeleteMutationMixin, BaseDeleteMutation):
     _mutation_class = "PolicyHolderContributionPlanMutation"
     _mutation_module = "policyholder"
     _model = PolicyHolderContributionPlan
 
     class Input(DeleteInputType):
         pass
 
+    @classmethod
+    def _validate_mutation(cls, user, **data):
+        super()._validate_mutation(user, **data)
+        PermissionValidation.validate_perms(user, PolicyholderConfig.gql_mutation_delete_policyholdercontributionplan_perms)
+
 
 class DeletePolicyHolderUserMutation(BaseHistoryModelDeleteMutationMixin, BaseDeleteMutation):
     _mutation_class = "PolicyHolderUserMutation"
     _mutation_module = "policyholder"
     _model = PolicyHolderUser
 
     class Input(DeleteInputType):
         pass
 
+    @classmethod
+    def _validate_mutation(cls, user, **data):
+        super()._validate_mutation(user, **data)
+        PermissionValidation.validate_perms(user, PolicyholderConfig.gql_mutation_delete_policyholderuser_perms)
```

### Comparing `openimis-be-policyholder-1.5.0/policyholder/gql/gql_mutations/input_types.py` & `openimis-be-policyholder-1.5.1/policyholder/gql/gql_mutations/input_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     date_valid_to = graphene.Date(required=False)
     json_ext = graphene.types.json.JSONString(required=False)
 
 
 class PolicyHolderInsureeReplaceInputType(ReplaceInputType):
     insuree_id = graphene.Int(required=True, name="insureeId")
     contribution_plan_bundle_id = graphene.UUID(requried=True, name="contributionPlanBundleId")
+    json_ext = graphene.types.json.JSONString(required=False)
     date_valid_from = graphene.Date(required=True)
     date_valid_to = graphene.Date(required=False)
 
 
 class PolicyHolderContributionPlanInputType(OpenIMISMutation.Input):
     id = graphene.UUID(required=False)
     policy_holder_id = graphene.UUID(required=False)
```

### Comparing `openimis-be-policyholder-1.5.0/policyholder/gql/gql_types.py` & `openimis-be-policyholder-1.5.1/policyholder/gql/gql_types.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/migrations/0001_initial.py` & `openimis-be-policyholder-1.5.1/policyholder/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/migrations/0002_auto_20201214_1237.py` & `openimis-be-policyholder-1.5.1/policyholder/migrations/0002_auto_20201214_1237.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/migrations/0003_auto_20201214_1239.py` & `openimis-be-policyholder-1.5.1/policyholder/migrations/0003_auto_20201214_1239.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/migrations/0004_auto_20201214_1302.py` & `openimis-be-policyholder-1.5.1/policyholder/migrations/0004_auto_20201214_1302.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/migrations/0005_auto_20210111_1254.py` & `openimis-be-policyholder-1.5.1/policyholder/migrations/0005_auto_20210111_1254.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/migrations/0006_policyholdercontributionplanmutation_policyholderinsureemutation_policyholdermutation_policyholderus.py` & `openimis-be-policyholder-1.5.1/policyholder/migrations/0006_policyholdercontributionplanmutation_policyholderinsureemutation_policyholdermutation_policyholderus.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/migrations/0007_auto_20210118_0927.py` & `openimis-be-policyholder-1.5.1/policyholder/migrations/0007_auto_20210118_0927.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/migrations/0008_auto_20210118_1109.py` & `openimis-be-policyholder-1.5.1/policyholder/migrations/0008_auto_20210118_1109.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/migrations/0009_auto_20210118_1127.py` & `openimis-be-policyholder-1.5.1/policyholder/migrations/0009_auto_20210118_1127.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/migrations/0010_auto_20210126_1040.py` & `openimis-be-policyholder-1.5.1/policyholder/migrations/0010_auto_20210126_1040.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/migrations/0015_auto_20210624_1243.py` & `openimis-be-policyholder-1.5.1/policyholder/migrations/0015_auto_20210624_1243.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/migrations/0016_policyholder_roles_for_admin.py` & `openimis-be-policyholder-1.5.1/policyholder/migrations/0016_policyholder_roles_for_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/models.py` & `openimis-be-policyholder-1.5.1/policyholder/models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/schema.py` & `openimis-be-policyholder-1.5.1/policyholder/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,17 +14,21 @@
     DeletePolicyHolderInsureeMutation, DeletePolicyHolderUserMutation, DeletePolicyHolderContributionPlanMutation
 from policyholder.gql.gql_mutations.update_mutations import UpdatePolicyHolderMutation, \
     UpdatePolicyHolderInsureeMutation, UpdatePolicyHolderUserMutation, UpdatePolicyHolderContributionPlanMutation
 from policyholder.gql.gql_mutations.replace_mutation import ReplacePolicyHolderInsureeMutation, \
     ReplacePolicyHolderContributionPlanMutation, ReplacePolicyHolderUserMutation
 
 from policyholder.apps import PolicyholderConfig
+from policyholder.services import PolicyHolder as PolicyHolderServices
 from policyholder.gql.gql_types import PolicyHolderUserGQLType, PolicyHolderGQLType, PolicyHolderInsureeGQLType, \
     PolicyHolderContributionPlanGQLType
 
+from django.core.exceptions import PermissionDenied
+from django.utils.translation import gettext as _
+
 from payment.signals import signal_before_payment_query
 from .signals import append_policy_holder_filter
 
 
 class Query(graphene.ObjectType):
     policy_holder = OrderedDjangoFilterConnectionField(
         PolicyHolderGQLType,
@@ -55,17 +59,30 @@
     policy_holder_contribution_plan_bundle = OrderedDjangoFilterConnectionField(
         PolicyHolderContributionPlanGQLType,
         orderBy=graphene.List(of_type=graphene.String),
         dateValidFrom__Gte=graphene.DateTime(),
         dateValidTo__Lte=graphene.DateTime(),
         applyDefaultValidityFilter=graphene.Boolean()
     )
+    validate_policy_holder_code = graphene.Field(
+        graphene.Boolean,
+        policy_holder_code=graphene.String(required=True),
+        description="Checks that the specified policy holder code is unique."
+    )
 
-    def resolve_policy_holder(self, info, **kwargs):
+    def resolve_validate_policy_holder_code(self, info, **kwargs):
+        if not info.context.user.has_perms(PolicyholderConfig.gql_query_policyholder_perms):
+            raise PermissionDenied(_("unauthorized"))
+        errors = PolicyHolderServices.check_unique_code_policy_holder(code=kwargs['policy_holder_code'])
+        return False if errors else True
 
+
+    def resolve_policy_holder(self, info, **kwargs):
+        if not info.context.user.has_perms(PolicyholderConfig.gql_query_policyholder_perms):
+            raise PermissionDenied(_("unauthorized"))
         filters = []
         additional_filter = kwargs.get('additional_filter', None)
         # go to process additional filter only when this arg of filter was passed into query
         if not info.context.user.has_perms(PolicyholderConfig.gql_query_policyholder_perms):
             # then check perms
             if info.context.user.has_perms(PolicyholderConfig.gql_query_policyholder_portal_perms):
                 # check if user is linked to ph in policy holder user table
```

### Comparing `openimis-be-policyholder-1.5.0/policyholder/services.py` & `openimis-be-policyholder-1.5.1/policyholder/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,20 @@
             uuid_string = str(phm.id)
             dict_representation = model_to_dict(phm)
             dict_representation["id"], dict_representation["uuid"] = (str(uuid_string), str(uuid_string))
         except Exception as exc:
             return _output_exception(model_name="PolicyHolder", method="create", exception=exc)
         return _output_result_success(dict_representation=dict_representation)
 
+    @staticmethod
+    def check_unique_code_policy_holder(code):
+        if PolicyHolderModel.objects.filter(code=code, is_deleted=False).exists():
+            return [{"message": "Policy holder code %s already exists" % code}]
+        return []
+
     @check_authentication
     def update(self, policy_holder):
         try:
             PolicyHolderValidation.validate_update(self.user, **policy_holder)
             updated_phm = PolicyHolderModel.objects.filter(id=policy_holder['id']).first()
             [setattr(updated_phm, key, policy_holder[key]) for key in policy_holder]
             updated_phm.save(username=self.user.username)
```

### Comparing `openimis-be-policyholder-1.5.0/policyholder/signals.py` & `openimis-be-policyholder-1.5.1/policyholder/signals.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/tests/helpers.py` & `openimis-be-policyholder-1.5.1/policyholder/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/tests/helpers_tests.py` & `openimis-be-policyholder-1.5.1/policyholder/tests/helpers_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/tests/services/services_ph_tests.py` & `openimis-be-policyholder-1.5.1/policyholder/tests/services/services_ph_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/policyholder/validation/policyholder_validation.py` & `openimis-be-policyholder-1.5.1/policyholder/validation/policyholder_validation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policyholder-1.5.0/setup.py` & `openimis-be-policyholder-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-policyholder',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend PolicyHolder reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

