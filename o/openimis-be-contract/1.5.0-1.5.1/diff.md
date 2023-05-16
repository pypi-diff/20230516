# Comparing `tmp/openimis-be-contract-1.5.0.tar.gz` & `tmp/openimis-be-contract-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-contract-1.5.0.tar", last modified: Fri Nov 11 08:12:05 2022, max compression
+gzip compressed data, was "openimis-be-contract-1.5.1.tar", last modified: Tue May 16 21:38:40 2023, max compression
```

## Comparing `openimis-be-contract-1.5.0.tar` & `openimis-be-contract-1.5.1.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:05.716985 openimis-be-contract-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     5024 2022-11-11 08:12:05.716985 openimis-be-contract-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4293 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:05.712985 openimis-be-contract-1.5.0/contract/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     5157 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     3946 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:05.712985 openimis-be-contract-1.5.0/contract/gql/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/gql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:05.712985 openimis-be-contract-1.5.0/contract/gql/gql_mutations/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/gql/gql_mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2157 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/gql/gql_mutations/contract_details_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     6410 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/gql/gql_mutations/contract_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     4225 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/gql/gql_mutations/input_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    11658 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/gql/gql_mutations/mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3685 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/gql/gql_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:05.716985 openimis-be-contract-1.5.0/contract/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    15534 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     3988 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0002_auto_20201221_1547.py
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0003_auto_20201222_1044.py
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0004_auto_20201222_1424.py
--rw-r--r--   0 runner    (1001) docker     (121)     1576 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0005_auto_20201228_1151.py
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0006_auto_20201228_1218.py
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0007_auto_20201228_1310.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0008_auto_20201230_1052.py
--rw-r--r--   0 runner    (1001) docker     (121)     3593 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0009_auto_20210118_1427.py
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0010_auto_20210119_1204.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0011_contractmutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0012_contractdetailsmutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0013_auto_20210202_0815.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0014_auto_20210208_1236.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0015_auto_20210208_1506.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0016_auto_20210208_1508.py
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0017_contract_roles_for_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0018_approve_ask_for_change_perms.py
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/0019_amend_perms.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6766 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     6073 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    48193 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/services.py
--rw-r--r--   0 runner    (1001) docker     (121)    12303 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:05.716985 openimis-be-contract-1.5.0/contract/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:05.716985 openimis-be-contract-1.5.0/contract/tests/gql_tests/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/tests/gql_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8717 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/tests/gql_tests/mutation_create_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)    23883 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/tests/gql_tests/query_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     3629 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4845 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/tests/helpers_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:05.716985 openimis-be-contract-1.5.0/contract/tests/services/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16004 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/tests/services/services_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:11:55.000000 openimis-be-contract-1.5.0/contract/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:05.716985 openimis-be-contract-1.5.0/openimis_be_contract.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5024 2022-11-11 08:12:05.000000 openimis-be-contract-1.5.0/openimis_be_contract.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-11-11 08:12:05.000000 openimis-be-contract-1.5.0/openimis_be_contract.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 08:12:05.000000 openimis-be-contract-1.5.0/openimis_be_contract.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-11-11 08:12:05.000000 openimis-be-contract-1.5.0/openimis_be_contract.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-11 08:12:05.000000 openimis-be-contract-1.5.0/openimis_be_contract.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 08:12:05.716985 openimis-be-contract-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-11-11 08:12:04.000000 openimis-be-contract-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:40.030490 openimis-be-contract-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5024 2023-05-16 21:38:40.026490 openimis-be-contract-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4293 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:40.026490 openimis-be-contract-1.5.1/contract/
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5157 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3946 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:40.026490 openimis-be-contract-1.5.1/contract/gql/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/gql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:40.026490 openimis-be-contract-1.5.1/contract/gql/gql_mutations/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/gql/gql_mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2157 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/gql/gql_mutations/contract_details_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7279 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/gql/gql_mutations/contract_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4225 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/gql/gql_mutations/input_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11658 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/gql/gql_mutations/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3685 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/gql/gql_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:40.026490 openimis-be-contract-1.5.1/contract/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)    15534 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0002_auto_20201221_1547.py
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0003_auto_20201222_1044.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0004_auto_20201222_1424.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0005_auto_20201228_1151.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0006_auto_20201228_1218.py
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0007_auto_20201228_1310.py
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0008_auto_20201230_1052.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0009_auto_20210118_1427.py
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0010_auto_20210119_1204.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0011_contractmutation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1104 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0012_contractdetailsmutation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0013_auto_20210202_0815.py
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0014_auto_20210208_1236.py
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0015_auto_20210208_1506.py
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0016_auto_20210208_1508.py
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0017_contract_roles_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0018_approve_ask_for_change_perms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0019_amend_perms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/0020_auto_20230126_0903.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6766 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6889 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48626 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/services.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12303 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:40.026490 openimis-be-contract-1.5.1/contract/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:40.026490 openimis-be-contract-1.5.1/contract/tests/gql_tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/tests/gql_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8717 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/tests/gql_tests/mutation_create_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23883 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/tests/gql_tests/query_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/tests/helpers_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:40.026490 openimis-be-contract-1.5.1/contract/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16004 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/tests/services/services_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-16 21:38:30.000000 openimis-be-contract-1.5.1/contract/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:40.026490 openimis-be-contract-1.5.1/openimis_be_contract.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5024 2023-05-16 21:38:39.000000 openimis-be-contract-1.5.1/openimis_be_contract.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2037 2023-05-16 21:38:39.000000 openimis-be-contract-1.5.1/openimis_be_contract.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 21:38:39.000000 openimis-be-contract-1.5.1/openimis_be_contract.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-05-16 21:38:39.000000 openimis-be-contract-1.5.1/openimis_be_contract.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-16 21:38:39.000000 openimis-be-contract-1.5.1/openimis_be_contract.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 21:38:40.030490 openimis-be-contract-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-05-16 21:38:39.000000 openimis-be-contract-1.5.1/setup.py
```

### Comparing `openimis-be-contract-1.5.0/LICENSE.md` & `openimis-be-contract-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/PKG-INFO` & `openimis-be-contract-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-contract
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Contract reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-contract-1.5.0/README.md` & `openimis-be-contract-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/apps.py` & `openimis-be-contract-1.5.1/contract/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/config.py` & `openimis-be-contract-1.5.1/contract/config.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/gql/gql_mutations/contract_details_mutations.py` & `openimis-be-contract-1.5.1/contract/gql/gql_mutations/contract_details_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/gql/gql_mutations/input_types.py` & `openimis-be-contract-1.5.1/contract/gql/gql_mutations/input_types.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/gql/gql_mutations/mutations.py` & `openimis-be-contract-1.5.1/contract/gql/gql_mutations/mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/gql/gql_types.py` & `openimis-be-contract-1.5.1/contract/gql/gql_types.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0001_initial.py` & `openimis-be-contract-1.5.1/contract/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0002_auto_20201221_1547.py` & `openimis-be-contract-1.5.1/contract/migrations/0002_auto_20201221_1547.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0003_auto_20201222_1044.py` & `openimis-be-contract-1.5.1/contract/migrations/0003_auto_20201222_1044.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0004_auto_20201222_1424.py` & `openimis-be-contract-1.5.1/contract/migrations/0004_auto_20201222_1424.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0005_auto_20201228_1151.py` & `openimis-be-contract-1.5.1/contract/migrations/0005_auto_20201228_1151.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0006_auto_20201228_1218.py` & `openimis-be-contract-1.5.1/contract/migrations/0006_auto_20201228_1218.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0007_auto_20201228_1310.py` & `openimis-be-contract-1.5.1/contract/migrations/0007_auto_20201228_1310.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0008_auto_20201230_1052.py` & `openimis-be-contract-1.5.1/contract/migrations/0008_auto_20201230_1052.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0009_auto_20210118_1427.py` & `openimis-be-contract-1.5.1/contract/migrations/0009_auto_20210118_1427.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0010_auto_20210119_1204.py` & `openimis-be-contract-1.5.1/contract/migrations/0010_auto_20210119_1204.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0011_contractmutation.py` & `openimis-be-contract-1.5.1/contract/migrations/0011_contractmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0012_contractdetailsmutation.py` & `openimis-be-contract-1.5.1/contract/migrations/0012_contractdetailsmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0013_auto_20210202_0815.py` & `openimis-be-contract-1.5.1/contract/migrations/0013_auto_20210202_0815.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0014_auto_20210208_1236.py` & `openimis-be-contract-1.5.1/contract/migrations/0014_auto_20210208_1236.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0015_auto_20210208_1506.py` & `openimis-be-contract-1.5.1/contract/migrations/0015_auto_20210208_1506.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0016_auto_20210208_1508.py` & `openimis-be-contract-1.5.1/contract/migrations/0016_auto_20210208_1508.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/migrations/0017_contract_roles_for_admin.py` & `openimis-be-contract-1.5.1/contract/migrations/0017_contract_roles_for_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/models.py` & `openimis-be-contract-1.5.1/contract/models.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/schema.py` & `openimis-be-contract-1.5.1/contract/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import graphene
 import graphene_django_optimizer as gql_optimizer
 
 from django.db.models import Q
+from .services import check_unique_code
+from core.gql_queries import ValidationMessageGQLType
 from core.schema import signal_mutation_module_before_mutating, OrderedDjangoFilterConnectionField
 from core.utils import append_validity_filter
 from contract.models import Contract, ContractDetails, \
     ContractContributionPlanDetails, ContractMutation
 from contract.gql.gql_types import ContractGQLType, ContractDetailsGQLType, \
     ContractContributionPlanDetailsGQLType
 
@@ -43,14 +45,30 @@
     contract_contribution_plan_details = OrderedDjangoFilterConnectionField(
         ContractContributionPlanDetailsGQLType,
         insuree=graphene.UUID(),
         contributionPlanBundle=graphene.UUID(),
         orderBy=graphene.List(of_type=graphene.String),
     )
 
+    validate_contract_code = graphene.Field(
+        ValidationMessageGQLType,
+        contract_code=graphene.String(required=True),
+        description="Check that the specified contract code is unique."
+    )
+
+    def resolve_validate_contract_code(self, info, **kwargs):
+        if not info.context.user.has_perms(ContractConfig.gql_query_contract_perms):
+            if not info.context.user.has_perms(ContractConfig.gql_query_contract_policyholder_portal_perms):
+                raise PermissionError("Unauthorized")
+        errors = check_unique_code(code=kwargs['contract_code'])
+        if errors:
+            return ValidationMessageGQLType(False)
+        else:
+            return ValidationMessageGQLType(True)
+
     def resolve_contract(self, info, **kwargs):
         if not info.context.user.has_perms(ContractConfig.gql_query_contract_perms):
             if not info.context.user.has_perms(ContractConfig.gql_query_contract_policyholder_portal_perms):
                 raise PermissionError("Unauthorized")
 
         filters = append_validity_filter(**kwargs)
         client_mutation_id = kwargs.get("client_mutation_id", None)
```

### Comparing `openimis-be-contract-1.5.0/contract/services.py` & `openimis-be-contract-1.5.1/contract/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import json
 
 from copy import copy
+
+from django.core.exceptions import ValidationError
+
 from .config import get_message_counter_contract
 
 from django.db.models.query import Q
 from django.conf import settings
 from django.contrib.auth.models import AnonymousUser
 from django.core.serializers.json import DjangoJSONEncoder
 from django.core.mail import send_mail, BadHeaderError
@@ -63,14 +66,17 @@
 
     def __init__(self, user):
         self.user = user
 
     @check_authentication
     def create(self, contract):
         try:
+            incoming_code = contract.get('code')
+            if check_unique_code(incoming_code):
+                raise ValidationError(("Contract code %s already exists" % incoming_code))
             if not self.user.has_perms(ContractConfig.gql_mutation_create_contract_perms):
                 raise PermissionError("Unauthorized")
             c = ContractModel(**contract)
             c.state = ContractModel.STATE_DRAFT
             c.save(username=self.user.username)
             uuid_string = f"{c.id}"
             # check if the PH is set
@@ -939,7 +945,13 @@
             from_email=settings.EMAIL_HOST_USER,
             recipient_list=[email],
             fail_silently=False,
         )
         return email_to_send
     except BadHeaderError:
         return ValueError('Invalid header found.')
+
+
+def check_unique_code(code):
+    if ContractModel.objects.filter(code=code, is_deleted=False).exists():
+        return [{"message": "Contract code %s already exists" % code}]
+    return []
```

### Comparing `openimis-be-contract-1.5.0/contract/signals.py` & `openimis-be-contract-1.5.1/contract/signals.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/tasks.py` & `openimis-be-contract-1.5.1/contract/tasks.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/tests/gql_tests/mutation_create_tests.py` & `openimis-be-contract-1.5.1/contract/tests/gql_tests/mutation_create_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/tests/gql_tests/query_tests.py` & `openimis-be-contract-1.5.1/contract/tests/gql_tests/query_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/tests/helpers.py` & `openimis-be-contract-1.5.1/contract/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/tests/helpers_tests.py` & `openimis-be-contract-1.5.1/contract/tests/helpers_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/tests/services/services_tests.py` & `openimis-be-contract-1.5.1/contract/tests/services/services_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/contract/utils.py` & `openimis-be-contract-1.5.1/contract/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contract-1.5.0/openimis_be_contract.egg-info/PKG-INFO` & `openimis-be-contract-1.5.1/openimis_be_contract.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-contract
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Contract reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-contract-1.5.0/openimis_be_contract.egg-info/SOURCES.txt` & `openimis-be-contract-1.5.1/openimis_be_contract.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE.md
 README.md
 setup.py
 contract/__init__.py
 contract/admin.py
 contract/apps.py
 contract/config.py
+contract/exceptions.py
 contract/models.py
 contract/schema.py
 contract/services.py
 contract/signals.py
 contract/tasks.py
 contract/urls.py
 contract/utils.py
@@ -35,14 +36,15 @@
 contract/migrations/0013_auto_20210202_0815.py
 contract/migrations/0014_auto_20210208_1236.py
 contract/migrations/0015_auto_20210208_1506.py
 contract/migrations/0016_auto_20210208_1508.py
 contract/migrations/0017_contract_roles_for_admin.py
 contract/migrations/0018_approve_ask_for_change_perms.py
 contract/migrations/0019_amend_perms.py
+contract/migrations/0020_auto_20230126_0903.py
 contract/migrations/__init__.py
 contract/tests/__init__.py
 contract/tests/helpers.py
 contract/tests/helpers_tests.py
 contract/tests/gql_tests/__init__.py
 contract/tests/gql_tests/mutation_create_tests.py
 contract/tests/gql_tests/query_tests.py
```

### Comparing `openimis-be-contract-1.5.0/setup.py` & `openimis-be-contract-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-contract',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Contract reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

