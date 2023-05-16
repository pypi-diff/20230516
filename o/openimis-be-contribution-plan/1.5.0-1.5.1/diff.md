# Comparing `tmp/openimis-be-contribution-plan-1.5.0.tar.gz` & `tmp/openimis-be-contribution-plan-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-contribution-plan-1.5.0.tar", last modified: Fri Nov 11 08:11:54 2022, max compression
+gzip compressed data, was "openimis-be-contribution-plan-1.5.1.tar", last modified: Tue May 16 21:38:35 2023, max compression
```

## Comparing `openimis-be-contribution-plan-1.5.0.tar` & `openimis-be-contribution-plan-1.5.1.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:54.713272 openimis-be-contribution-plan-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-11-11 08:11:54.713272 openimis-be-contribution-plan-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:54.709272 openimis-be-contribution-plan-1.5.0/contribution_plan/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     4949 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:54.709272 openimis-be-contribution-plan-1.5.0/contribution_plan/gql/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/gql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:54.709272 openimis-be-contribution-plan-1.5.0/contribution_plan/gql/gql_mutations/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/gql/gql_mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1865 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/gql/gql_mutations/contribution_plan_bundle_details_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     4311 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/gql/gql_mutations/contribution_plan_bundle_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/gql/gql_mutations/contribution_plan_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3868 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/gql/gql_mutations/input_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2850 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/gql/gql_mutations/payment_plan_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     4084 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/gql/gql_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:54.709272 openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    14098 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0002_auto_20201204_1353.py
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0003_auto_20201204_1439.py
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0004_auto_20201217_0946.py
--rw-r--r--   0 runner    (1001) docker     (121)     1805 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0005_contributionplanbundlemutation_contributionplanmutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     5583 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0006_auto_20210118_1349.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0007_auto_20210217_1302.py
--rw-r--r--   0 runner    (1001) docker     (121)     5470 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0008_historicalpaymentplan_paymentplan.py
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0009_contributionplan_roles_for_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0010_payment_plan_roles_for_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     5142 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     7229 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    14417 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/services.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:54.709272 openimis-be-contribution-plan-1.5.0/contribution_plan/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:54.709272 openimis-be-contribution-plan-1.5.0/contribution_plan/tests/gql_tests/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/tests/gql_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11834 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/tests/gql_tests/mutations_cp_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)    11419 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/tests/gql_tests/mutations_cpb_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     6897 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/tests/gql_tests/mutations_cpbd_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     7201 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/tests/gql_tests/mutations_pp_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     7194 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/tests/gql_tests/query_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     3732 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5296 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/tests/helpers_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:54.709272 openimis-be-contribution-plan-1.5.0/contribution_plan/tests/services/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24239 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/tests/services/services_cp_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:11:44.000000 openimis-be-contribution-plan-1.5.0/contribution_plan/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:54.713272 openimis-be-contribution-plan-1.5.0/openimis_be_contribution_plan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-11-11 08:11:54.000000 openimis-be-contribution-plan-1.5.0/openimis_be_contribution_plan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2022-11-11 08:11:54.000000 openimis-be-contribution-plan-1.5.0/openimis_be_contribution_plan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 08:11:54.000000 openimis-be-contribution-plan-1.5.0/openimis_be_contribution_plan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-11-11 08:11:54.000000 openimis-be-contribution-plan-1.5.0/openimis_be_contribution_plan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-11 08:11:54.000000 openimis-be-contribution-plan-1.5.0/openimis_be_contribution_plan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 08:11:54.713272 openimis-be-contribution-plan-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-11-11 08:11:53.000000 openimis-be-contribution-plan-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:35.078549 openimis-be-contribution-plan-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-05-16 21:38:35.078549 openimis-be-contribution-plan-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2852 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:35.074548 openimis-be-contribution-plan-1.5.1/contribution_plan/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4949 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:35.074548 openimis-be-contribution-plan-1.5.1/contribution_plan/gql/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/gql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:35.074548 openimis-be-contribution-plan-1.5.1/contribution_plan/gql/gql_mutations/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/gql/gql_mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3116 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/gql/gql_mutations/contribution_plan_bundle_details_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5789 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/gql/gql_mutations/contribution_plan_bundle_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3059 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/gql/gql_mutations/contribution_plan_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/gql/gql_mutations/input_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3267 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/gql/gql_mutations/payment_plan_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4084 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/gql/gql_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:35.078549 openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)    14098 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23110 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0001_squashed_0010_payment_plan_roles_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      990 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0002_auto_20201204_1353.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0002_auto_20230126_0903.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0003_auto_20201204_1439.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0004_auto_20201217_0946.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1805 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0005_contributionplanbundlemutation_contributionplanmutation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5583 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0006_auto_20210118_1349.py
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0007_auto_20210217_1302.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5470 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0008_historicalpaymentplan_paymentplan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0009_contributionplan_roles_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0010_payment_plan_roles_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5141 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9325 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15151 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/services.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:35.078549 openimis-be-contribution-plan-1.5.1/contribution_plan/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:35.078549 openimis-be-contribution-plan-1.5.1/contribution_plan/tests/gql_tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/tests/gql_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10638 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/tests/gql_tests/mutations_cp_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10317 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/tests/gql_tests/mutations_cpb_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6897 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/tests/gql_tests/mutations_cpbd_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7201 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/tests/gql_tests/mutations_pp_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7194 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/tests/gql_tests/query_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3732 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5296 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/tests/helpers_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:35.078549 openimis-be-contribution-plan-1.5.1/contribution_plan/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24193 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/tests/services/services_cp_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-16 21:38:26.000000 openimis-be-contribution-plan-1.5.1/contribution_plan/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:35.078549 openimis-be-contribution-plan-1.5.1/openimis_be_contribution_plan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-05-16 21:38:35.000000 openimis-be-contribution-plan-1.5.1/openimis_be_contribution_plan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2358 2023-05-16 21:38:35.000000 openimis-be-contribution-plan-1.5.1/openimis_be_contribution_plan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 21:38:35.000000 openimis-be-contribution-plan-1.5.1/openimis_be_contribution_plan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-16 21:38:35.000000 openimis-be-contribution-plan-1.5.1/openimis_be_contribution_plan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-16 21:38:35.000000 openimis-be-contribution-plan-1.5.1/openimis_be_contribution_plan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 21:38:35.078549 openimis-be-contribution-plan-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1349 2023-05-16 21:38:34.000000 openimis-be-contribution-plan-1.5.1/setup.py
```

### Comparing `openimis-be-contribution-plan-1.5.0/LICENSE.md` & `openimis-be-contribution-plan-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/PKG-INFO` & `openimis-be-contribution-plan-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-contribution-plan
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Contribution Plan reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-contribution-plan-1.5.0/README.md` & `openimis-be-contribution-plan-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/apps.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/gql/gql_mutations/input_types.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/gql/gql_mutations/input_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     code = graphene.String(required=True, max_length=32)
     name = graphene.String(required=False, max_length=255)
     periodicity = graphene.Int(required=False)
     date_valid_from = graphene.Date(required=False)
     date_valid_to = graphene.Date(required=False)
     json_ext = graphene.types.json.JSONString(required=False)
 
-
 class ContributionPlanBundleUpdateInputType(OpenIMISMutation.Input):
     id = graphene.UUID(required=True)
     name = graphene.String(required=False, max_length=255)
     periodicity = graphene.Int(required=False)
     json_ext = graphene.types.json.JSONString(required=False)
     date_valid_from = graphene.Date(required=False)
     date_valid_to = graphene.Date(required=False)
@@ -57,14 +56,15 @@
 class ContributionPlanReplaceInputType(ReplaceInputType):
     name = graphene.String(required=False, max_lenght=255)
     calculation = graphene.UUID(required=False)
     benefit_plan_id = graphene.Int(required=False)
     periodicity = graphene.Int(required=False)
     date_valid_from = graphene.Date(required=True)
     date_valid_to = graphene.Date(required=False)
+    json_ext = graphene.types.json.JSONString(required=False)
 
 
 class ContributionPlanBundleDetailsInputType(OpenIMISMutation.Input):
     id = graphene.UUID(required=False)
     contribution_plan_bundle_id = graphene.UUID(required=True)
     contribution_plan_id = graphene.UUID(required=True)
     date_valid_from = graphene.Date(required=False)
```

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/gql/gql_mutations/payment_plan_mutations.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/gql/gql_mutations/payment_plan_mutations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,76 @@
 from core.gql.gql_mutations import DeleteInputType
 from core.gql.gql_mutations.base_mutation import BaseMutation, BaseDeleteMutation, BaseReplaceMutation, \
     BaseHistoryModelCreateMutationMixin, BaseHistoryModelUpdateMutationMixin, \
     BaseHistoryModelDeleteMutationMixin, BaseHistoryModelReplaceMutationMixin
+from contribution_plan.services import PaymentPlan as PaymentPlanService
 from contribution_plan.gql.gql_mutations import PaymentPlanInputType, PaymentPlanUpdateInputType, \
     PaymentPlanReplaceInputType
 from contribution_plan.apps import ContributionPlanConfig
 from contribution_plan.models import PaymentPlan
 from django.contrib.auth.models import AnonymousUser
 from django.core.exceptions import ValidationError
+from django.utils.translation import gettext as _
 
 
 class CreatePaymentPlanMutation(BaseHistoryModelCreateMutationMixin, BaseMutation):
     _mutation_class = "PaymentPlanMutation"
     _mutation_module = "contribution_plan"
     _model = PaymentPlan
 
     @classmethod
     def _validate_mutation(cls, user, **data):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
                 ContributionPlanConfig.gql_mutation_create_paymentplan_perms):
-            raise ValidationError("mutation.authentication_required")
+            raise ValidationError(_("mutation.authentication_required"))
+        if PaymentPlanService.check_unique_code(data['code']):
+            raise ValidationError(_("mutation.payment_plan_code_duplicated"))
 
     class Input(PaymentPlanInputType):
         pass
 
 
 class UpdatePaymentPlanMutation(BaseHistoryModelUpdateMutationMixin, BaseMutation):
     _mutation_class = "PaymentPlanMutation"
     _mutation_module = "contribution_plan"
     _model = PaymentPlan
 
     @classmethod
     def _validate_mutation(cls, user, **data):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
                 ContributionPlanConfig.gql_mutation_update_paymentplan_perms):
-            raise ValidationError("mutation.authentication_required")
+            raise ValidationError(_("mutation.authentication_required"))
+        if PaymentPlanService.check_unique_code(data['code']):
+            raise ValidationError(_("mutation.payment_plan_code_duplicated"))
 
     class Input(PaymentPlanUpdateInputType):
         pass
 
 
 class DeletePaymentPlanMutation(BaseHistoryModelDeleteMutationMixin, BaseDeleteMutation):
     _mutation_class = "PaymentPlanMutation"
     _mutation_module = "contribution_plan"
     _model = PaymentPlan
 
     @classmethod
     def _validate_mutation(cls, user, **data):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
                 ContributionPlanConfig.gql_mutation_delete_paymentplan_perms):
-            raise ValidationError("mutation.authentication_required")
+            raise ValidationError(_("mutation.authentication_required"))
 
     class Input(DeleteInputType):
         pass
 
 
 class ReplacePaymentPlanMutation(BaseHistoryModelReplaceMutationMixin, BaseReplaceMutation):
     _mutation_class = "PaymentPlanMutation"
     _mutation_module = "contribution_plan"
     _model = PaymentPlan
 
     @classmethod
     def _validate_mutation(cls, user, **data):
         if type(user) is AnonymousUser or not user.id or not user.has_perms(
                 ContributionPlanConfig.gql_mutation_replace_paymentplan_perms):
-            raise ValidationError("mutation.authentication_required")
+            raise ValidationError(_("mutation.authentication_required"))
 
     class Input(PaymentPlanReplaceInputType):
         pass
```

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/gql/gql_types.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/gql/gql_types.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0001_initial.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0002_auto_20201204_1353.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0002_auto_20201204_1353.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0003_auto_20201204_1439.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0003_auto_20201204_1439.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0004_auto_20201217_0946.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0004_auto_20201217_0946.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0005_contributionplanbundlemutation_contributionplanmutation.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0005_contributionplanbundlemutation_contributionplanmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0006_auto_20210118_1349.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0006_auto_20210118_1349.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0007_auto_20210217_1302.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0007_auto_20210217_1302.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0008_historicalpaymentplan_paymentplan.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0008_historicalpaymentplan_paymentplan.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0009_contributionplan_roles_for_admin.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0009_contributionplan_roles_for_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/migrations/0010_payment_plan_roles_for_admin.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/migrations/0010_payment_plan_roles_for_admin.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/mixins.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/mixins.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/models.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
         self.length = self.periodicity
         get_contribution_length_signal.send(sender=self.__class__,  instance=self)
         return self.length
 
     class Meta:
         db_table = 'tblContributionPlan'
 
-
 class PaymentPlan(GenericPlan):
 
     class Meta:
         db_table = 'tblPaymentPlan'
 
 
 class ContributionPlanBundleDetailsManager(models.Manager):
```

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/services.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/services.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             }
         else:
             result = function(self, *args, **kwargs)
             return result
     return wrapper
 
 
-class ContributionPlan(object):
+class ContributionPlanService(object):
 
     def __init__(self, user):
         self.user = user
 
     @check_authentication
     def get_by_id(self, by_contribution_plan):
         try:
@@ -89,16 +89,22 @@
             "success": True,
             "message": "Ok",
             "detail": "",
             "old_object": json.loads(json.dumps(dict_representation, cls=DjangoJSONEncoder)),
             "uuid_new_object": str(cp_to_replace.replacement_uuid),
         }
 
+    @staticmethod
+    def check_unique_code(code):
+        if ContributionPlanModel.objects.filter(code=code, is_deleted=0).exists():
+            return [{"message": "Contribution plan code %s already exists" % code}]
+        return []
 
-class ContributionPlanBundle(object):
+
+class ContributionPlanBundleService(object):
 
     def __init__(self, user):
         self.user = user
 
     @check_authentication
     def get_by_id(self, by_contribution_plan_bundle):
         try:
@@ -162,14 +168,22 @@
             "success": True,
             "message": "Ok",
             "detail": "",
             "old_object": json.loads(json.dumps(dict_representation, cls=DjangoJSONEncoder)),
             "uuid_new_object": str(cpb_to_replace.replacement_uuid),
         }
 
+    @staticmethod
+    def check_unique_code(code):
+        if ContributionPlanBundleModel.objects.filter(code=code, is_deleted=0).exists():
+            return [{"message": "Contribution plan bundle code %s already exists" % code}]
+        return []
+
+
+
 
 class ContributionPlanBundleDetails(object):
 
     def __init__(self, user):
         self.user = user
 
     @check_authentication
@@ -291,14 +305,20 @@
             "success": True,
             "message": "Ok",
             "detail": "",
             "old_object": json.loads(json.dumps(dict_representation, cls=DjangoJSONEncoder)),
             "uuid_new_object": str(pp_to_replace.replacement_uuid),
         }
 
+    @staticmethod
+    def check_unique_code(code):
+        if PaymentPlanModel.objects.filter(code=code, is_deleted=False).exists():
+            return [{"message": "Payment plan code %s already exists" % code}]
+        return []
+
 
 def _output_exception(model_name, method, exception):
     return {
         "success": False,
         "message": f"Failed to {method} {model_name}",
         "detail": str(exception),
         "data": "",
```

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/tests/gql_tests/mutations_cp_tests.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/tests/gql_tests/mutations_cp_tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,40 +80,14 @@
         time_stamp = datetime.datetime.now()
         input_param = {
             "name": "XYZ test name xyz - " + str(time_stamp),
         }
         result_mutation = self.add_mutation("createContributionPlan", input_param)
         self.assertEqual(True, 'errors' in result_mutation)
 
-    def test_contribution_plan_delete_more(self):
-        time_stamp = datetime.datetime.now()
-        input_param = {
-            "code": "XYZ deletion",
-            "name": "XYZ test deletion xyz - " + str(time_stamp),
-            "benefitPlanId": self.test_product.id,
-            "calculation": f"{self.test_calculation}",
-            "periodicity": 12,
-        }
-        self.add_mutation("createContributionPlan", input_param)
-        self.add_mutation("createContributionPlan", input_param)
-        result = self.find_by_exact_attributes_query("contributionPlan", {**input_param, 'isDeleted': False})
-        converted_ids = [f"{base64.b64decode(edge['node']['id']).decode('utf-8').split(':')[1]}" for edge in
-                         result["edges"]]
-
-        input_param2 = {
-            "uuids": converted_ids,
-        }
-        self.add_mutation("deleteContributionPlan", input_param2)
-        result2 = self.find_by_exact_attributes_query("contributionPlan", {**input_param, 'isDeleted': False})
-
-        # tear down the test data
-        ContributionPlan.objects.filter(id__in=converted_ids).delete()
-
-        self.assertEqual((2, 0), (result["totalCount"], result2["totalCount"]))
-
     def test_contribution_plan_delete_single_deletion(self):
         time_stamp = datetime.datetime.now()
         input_param = {
             "code": "XYZ deletion",
             "name": "XYZ test deletion xyz - " + str(time_stamp),
             "benefitPlanId": self.test_product.id,
             "calculation": f"{self.test_calculation}",
```

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/tests/gql_tests/mutations_cpb_tests.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/tests/gql_tests/mutations_cpb_tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,37 +57,14 @@
         time_stamp = datetime.datetime.now()
         input_param = {
             "name": "XYZ test name xyz - " + str(time_stamp),
         }
         result_mutation = self.add_mutation("createContributionPlanBundle", input_param)
         self.assertEqual(True, 'errors' in result_mutation)
 
-    def test_contribution_plan_bundle_delete_more(self):
-        time_stamp = datetime.datetime.now()
-        input_param = {
-            "code": "XYZ deletion",
-            "name": "XYZ test deletion xyz - " + str(time_stamp),
-        }
-        self.add_mutation("createContributionPlanBundle", input_param)
-        self.add_mutation("createContributionPlanBundle", input_param)
-        result = self.find_by_exact_attributes_query("contributionPlanBundle", {**input_param, 'isDeleted': False})
-        converted_ids = [f"{base64.b64decode(edge['node']['id']).decode('utf-8').split(':')[1]}" for edge in
-                         result["edges"]]
-
-        input_param2 = {
-            "uuids": converted_ids,
-        }
-        self.add_mutation("deleteContributionPlanBundle", input_param2)
-        result2 = self.find_by_exact_attributes_query("contributionPlanBundle", {**input_param, 'isDeleted': False})
-
-        # tear down the test data
-        ContributionPlanBundle.objects.filter(id__in=converted_ids).delete()
-
-        self.assertEqual((2, 0), (result["totalCount"], result2["totalCount"]))
-
     def test_contribution_plan_bundle_delete_single_deletion(self):
         time_stamp = datetime.datetime.now()
         input_param = {
             "code": "XYZ deletion",
             "name": "XYZ test deletion xyz - " + str(time_stamp),
         }
         self.add_mutation("createContributionPlanBundle", input_param)
```

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/tests/gql_tests/mutations_cpbd_tests.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/tests/gql_tests/mutations_cpbd_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/tests/gql_tests/mutations_pp_tests.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/tests/gql_tests/mutations_pp_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/tests/gql_tests/query_tests.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/tests/gql_tests/query_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/tests/helpers.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/tests/helpers_tests.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/tests/helpers_tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/tests/services/services_cp_tests.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/tests/services/services_cp_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.test import TestCase
-from contribution_plan.services import ContributionPlan as ContributionPlanService, \
-    ContributionPlanBundle as ContributionPlanBundleService, \
+from contribution_plan.services import ContributionPlanService, \
+    ContributionPlanBundleService, \
     ContributionPlanBundleDetails as ContributionPlanBundleDetailsService, PaymentPlan as PaymentPlanService
 from contribution_plan.models import ContributionPlan, ContributionPlanBundle, \
     ContributionPlanBundleDetails, PaymentPlan
 from calculation.calculation_rule import ContributionValuationRule
 from core.models import User
 from contribution_plan.tests.helpers import create_test_contribution_plan, \
     create_test_contribution_plan_bundle
```

### Comparing `openimis-be-contribution-plan-1.5.0/contribution_plan/utils.py` & `openimis-be-contribution-plan-1.5.1/contribution_plan/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-plan-1.5.0/openimis_be_contribution_plan.egg-info/PKG-INFO` & `openimis-be-contribution-plan-1.5.1/openimis_be_contribution_plan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-contribution-plan
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Contribution Plan reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-contribution-plan-1.5.0/openimis_be_contribution_plan.egg-info/SOURCES.txt` & `openimis-be-contribution-plan-1.5.1/openimis_be_contribution_plan.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 contribution_plan/gql/gql_mutations/__init__.py
 contribution_plan/gql/gql_mutations/contribution_plan_bundle_details_mutations.py
 contribution_plan/gql/gql_mutations/contribution_plan_bundle_mutations.py
 contribution_plan/gql/gql_mutations/contribution_plan_mutations.py
 contribution_plan/gql/gql_mutations/input_types.py
 contribution_plan/gql/gql_mutations/payment_plan_mutations.py
 contribution_plan/migrations/0001_initial.py
+contribution_plan/migrations/0001_squashed_0010_payment_plan_roles_for_admin.py
 contribution_plan/migrations/0002_auto_20201204_1353.py
+contribution_plan/migrations/0002_auto_20230126_0903.py
 contribution_plan/migrations/0003_auto_20201204_1439.py
 contribution_plan/migrations/0004_auto_20201217_0946.py
 contribution_plan/migrations/0005_contributionplanbundlemutation_contributionplanmutation.py
 contribution_plan/migrations/0006_auto_20210118_1349.py
 contribution_plan/migrations/0007_auto_20210217_1302.py
 contribution_plan/migrations/0008_historicalpaymentplan_paymentplan.py
 contribution_plan/migrations/0009_contributionplan_roles_for_admin.py
```

### Comparing `openimis-be-contribution-plan-1.5.0/setup.py` & `openimis-be-contribution-plan-1.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-contribution-plan',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Contribution Plan reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

