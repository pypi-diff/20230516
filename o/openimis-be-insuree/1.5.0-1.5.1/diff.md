# Comparing `tmp/openimis-be-insuree-1.5.0.tar.gz` & `tmp/openimis-be-insuree-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-insuree-1.5.0.tar", last modified: Thu Nov 10 18:09:34 2022, max compression
+gzip compressed data, was "openimis-be-insuree-1.5.1.tar", last modified: Tue May 16 21:38:13 2023, max compression
```

## Comparing `openimis-be-insuree-1.5.0.tar` & `openimis-be-insuree-1.5.1.tar`

### file list

```diff
@@ -1,52 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:34.556990 openimis-be-insuree-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-11-10 18:09:34.556990 openimis-be-insuree-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3136 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:34.556990 openimis-be-insuree-1.5.0/insuree/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     5669 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (121)    16913 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     7203 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:34.556990 openimis-be-insuree-1.5.0/insuree/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3084 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     3278 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/migrations/0002_family_familytype_photo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/migrations/0003_insureepolicy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2810 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/migrations/0004_confirmationtype_education_profession_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/migrations/0005_identificationtype.py
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/migrations/0006_auto_20200722_0839.py
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/migrations/0007_auto_20200722_0940.py
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/migrations/0008_auto_20200731_0443.py
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/migrations/0009_familymutation_insureemutation.py
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/migrations/0010_auto_20200731_0524.py
--rw-r--r--   0 runner    (1001) docker     (121)     2717 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/migrations/0011_auto_20200807_1309.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/migrations/0012_policyrenewaldetail.py
--rw-r--r--   0 runner    (1001) docker     (121)      820 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/migrations/0013_auto_20211103_1023.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16085 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/report.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:34.556990 openimis-be-insuree-1.5.0/insuree/reports/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    53577 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/reports/enrolled_families.py
--rw-r--r--   0 runner    (1001) docker     (121)    52864 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/reports/insuree_family_overview.py
--rw-r--r--   0 runner    (1001) docker     (121)    16221 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    12010 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/services.py
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     2596 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:34.556990 openimis-be-insuree-1.5.0/insuree/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/tests/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (121)     7197 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/tests/test_insuree_photo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/tests/test_insuree_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-10 18:09:25.000000 openimis-be-insuree-1.5.0/insuree/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:34.556990 openimis-be-insuree-1.5.0/openimis_be_insuree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-11-10 18:09:34.000000 openimis-be-insuree-1.5.0/openimis_be_insuree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-11-10 18:09:34.000000 openimis-be-insuree-1.5.0/openimis_be_insuree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 18:09:34.000000 openimis-be-insuree-1.5.0/openimis_be_insuree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-10 18:09:34.000000 openimis-be-insuree-1.5.0/openimis_be_insuree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-10 18:09:34.000000 openimis-be-insuree-1.5.0/openimis_be_insuree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 18:09:34.556990 openimis-be-insuree-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-11-10 18:09:33.000000 openimis-be-insuree-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:13.354704 openimis-be-insuree-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-16 21:38:13.354704 openimis-be-insuree-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:13.350704 openimis-be-insuree-1.5.1/insuree/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:13.350704 openimis-be-insuree-1.5.1/insuree/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:13.350704 openimis-be-insuree-1.5.1/insuree/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/management/commands/generateinsurees.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:13.354704 openimis-be-insuree-1.5.1/insuree/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/0002_family_familytype_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/0003_insureepolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/0004_confirmationtype_education_profession_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/0005_identificationtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/0006_auto_20200722_0839.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/0007_auto_20200722_0940.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/0008_auto_20200731_0443.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/0009_familymutation_insureemutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/0010_auto_20200731_0524.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/0011_auto_20200807_1309.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/0012_policyrenewaldetail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/0013_auto_20211103_1023.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/0014_add_missing_fields_to_django_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/0015_set_managed_to_true_in_all_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16073 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:13.354704 openimis-be-insuree-1.5.1/insuree/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53577 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/reports/enrolled_families.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52864 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/reports/insuree_family_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65100 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/reports/insuree_missing_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38213 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/reports/insurees_pending_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:13.354704 openimis-be-insuree-1.5.1/insuree/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/tests/test_insuree_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/tests/test_insuree_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 21:38:01.000000 openimis-be-insuree-1.5.1/insuree/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:13.354704 openimis-be-insuree-1.5.1/openimis_be_insuree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-16 21:38:13.000000 openimis-be-insuree-1.5.1/openimis_be_insuree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-16 21:38:13.000000 openimis-be-insuree-1.5.1/openimis_be_insuree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:38:13.000000 openimis-be-insuree-1.5.1/openimis_be_insuree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 21:38:13.000000 openimis-be-insuree-1.5.1/openimis_be_insuree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 21:38:13.000000 openimis-be-insuree-1.5.1/openimis_be_insuree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:38:13.354704 openimis-be-insuree-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-16 21:38:12.000000 openimis-be-insuree-1.5.1/setup.py
```

### Comparing `openimis-be-insuree-1.5.0/LICENSE.md` & `openimis-be-insuree-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/PKG-INFO` & `openimis-be-insuree-1.5.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: openimis-be-insuree
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Insuree reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE.md
```

### Comparing `openimis-be-insuree-1.5.0/README.md` & `openimis-be-insuree-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/insuree/apps.py` & `openimis-be-insuree-1.5.1/insuree/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 
 MODULE_NAME = "insuree"
 
 DEFAULT_CFG = {
     "gql_query_insurees_perms": ["101101"],
     "gql_query_insuree_perms": ["101101"],
+    "gql_query_insuree_photo_perms": ["101101"],
     "gql_query_insuree_officers_perms": [],
-    "gql_insuree_family_members": ["101101"],
+    "gql_query_insuree_family_members": ["101101"],
     "gql_query_families_perms": ["101001"],
     "gql_query_insuree_policy_perms": ["101500"],
     "gql_mutation_create_families_perms": ["101002"],
     "gql_mutation_update_families_perms": ["101003"],
     "gql_mutation_delete_families_perms": ["101004"],
     "gql_mutation_create_insurees_perms": ["101102"],
     "gql_mutation_update_insurees_perms": ["101103"],
@@ -31,37 +32,44 @@
 
 class InsureeConfig(AppConfig):
     name = MODULE_NAME
 
     gql_query_insurees_perms = []
     gql_query_insuree_perms = []
 
-    gql_insuree_family_members = []
+    gql_query_insuree_family_members = []
     gql_query_families_perms = []
     gql_query_insuree_officers_perms = []
     gql_query_insuree_policy_perms = []
+    gql_query_insuree_photo_perms = []
     gql_mutation_create_families_perms = []
     gql_mutation_update_families_perms = []
     gql_mutation_delete_families_perms = []
     gql_mutation_create_insurees_perms = []
     gql_mutation_update_insurees_perms = []
     gql_mutation_delete_insurees_perms = []
+    validation_code_taken_insuree_number = 1
+    validation_code_no_insuree_number = 2
+    validation_code_invalid_insuree_number_len = 3
+    validation_code_invalid_insuree_number_checksum = 4
+    validation_code_invalid_insuree_number_exception = 5
     insuree_photos_root_path = None
     excluded_insuree_chfids = ['999999999']
     renewal_photo_age_adult = 60
     renewal_photo_age_child = 12
     insuree_number_validator = None
     insuree_number_length = None
     insuree_number_modulo_root = None
 
     def _configure_permissions(self, cfg):
         InsureeConfig.gql_query_insurees_perms = cfg["gql_query_insurees_perms"]
         InsureeConfig.gql_query_insuree_perms = cfg["gql_query_insuree_perms"]
+        InsureeConfig.gql_query_insuree_photo_perms = cfg["gql_query_insuree_photo_perms"]
         InsureeConfig.gql_query_insuree_officers_perms = cfg["gql_query_insuree_officers_perms"]
-        InsureeConfig.gql_insuree_family_members = cfg["gql_insuree_family_members"]
+        InsureeConfig.gql_query_insuree_family_members = cfg["gql_query_insuree_family_members"]
         InsureeConfig.gql_query_families_perms = cfg["gql_query_families_perms"]
         InsureeConfig.gql_query_insuree_policy_perms = cfg["gql_query_insuree_policy_perms"]
         InsureeConfig.gql_mutation_create_families_perms = cfg["gql_mutation_create_families_perms"]
         InsureeConfig.gql_mutation_update_families_perms = cfg["gql_mutation_update_families_perms"]
         InsureeConfig.gql_mutation_create_insurees_perms = cfg["gql_mutation_create_insurees_perms"]
         InsureeConfig.gql_mutation_update_insurees_perms = cfg["gql_mutation_update_insurees_perms"]
         InsureeConfig.gql_mutation_delete_insurees_perms = cfg["gql_mutation_delete_insurees_perms"]
```

### Comparing `openimis-be-insuree-1.5.0/insuree/dataloaders.py` & `openimis-be-insuree-1.5.1/insuree/dataloaders.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/insuree/gql_mutations.py` & `openimis-be-insuree-1.5.1/insuree/gql_mutations.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,18 +147,14 @@
                     _("mutation.authentication_required"))
             if not user.has_perms(InsureeConfig.gql_mutation_create_families_perms):
                 raise PermissionDenied(_("unauthorized"))
             data['audit_user_id'] = user.id_for_audit
             from core.utils import TimeUtils
             data['validity_from'] = TimeUtils.now()
             client_mutation_id = data.get("client_mutation_id")
-            # Validate insuree number right away
-            errors = validate_insuree_number(data.get("head_insuree", {}).get("chf_id", None), True)
-            if errors:
-                return errors
             family = update_or_create_family(data, user)
             FamilyMutation.object_mutated(user, client_mutation_id=client_mutation_id, family=family)
             return None
         except Exception as exc:
             logger.exception("insuree.mutation.failed_to_create_family")
             return [{
                 'message': _("insuree.mutation.failed_to_create_family"),
@@ -248,18 +244,14 @@
                     _("mutation.authentication_required"))
             if not user.has_perms(InsureeConfig.gql_mutation_create_insurees_perms):
                 raise PermissionDenied(_("unauthorized"))
             data['audit_user_id'] = user.id_for_audit
             from core.utils import TimeUtils
             data['validity_from'] = TimeUtils.now()
             client_mutation_id = data.get("client_mutation_id")
-            # Validate insuree number right away
-            errors = validate_insuree_number(data.get("chf_id", None), True)
-            if errors:
-                return errors
             insuree = update_or_create_insuree(data, user)
             InsureeMutation.object_mutated(user, client_mutation_id=client_mutation_id, insuree=insuree)
             return None
         except Exception as exc:
             logger.exception("insuree.mutation.failed_to_create_insuree")
             return [{
                 'message': _("insuree.mutation.failed_to_create_insuree"),
@@ -281,14 +273,16 @@
     def async_mutate(cls, user, **data):
         try:
             if type(user) is AnonymousUser or not user.id:
                 raise ValidationError(
                     _("mutation.authentication_required"))
             if not user.has_perms(InsureeConfig.gql_mutation_create_insurees_perms):
                 raise PermissionDenied(_("unauthorized"))
+            if 'uuid' not in data:
+                raise ValidationError("There is no uuid in updateMutation input!")
             data['audit_user_id'] = user.id_for_audit
             client_mutation_id = data.get("client_mutation_id")
             insuree = update_or_create_insuree(data, user)
             InsureeMutation.object_mutated(user, client_mutation_id=client_mutation_id, insuree=insuree)
             return None
         except Exception as exc:
             logger.exception("insuree.mutation.failed_to_update_insuree")
```

### Comparing `openimis-be-insuree-1.5.0/insuree/gql_queries.py` & `openimis-be-insuree-1.5.1/insuree/gql_queries.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 from .apps import InsureeConfig
 from .models import Insuree, InsureePhoto, Education, Profession, Gender, IdentificationType, \
     Family, FamilyType, ConfirmationType, Relation, InsureePolicy, FamilyMutation, InsureeMutation
 from location.schema import LocationGQLType
 from policy.gql_queries import PolicyGQLType
 from core import prefix_filterset, filter_validity, ExtendedConnection
+from django.utils.translation import gettext as _
+from django.core.exceptions import PermissionDenied
 
 from .services import load_photo_file
 
 
 class GenderGQLType(DjangoObjectType):
     class Meta:
         model = Gender
@@ -19,14 +21,16 @@
         }
 
 
 class PhotoGQLType(DjangoObjectType):
     photo = graphene.String()
 
     def resolve_photo(self, info):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_insuree_photo_perms):
+            raise PermissionDenied(_("unauthorized"))
         if self.photo:
             return self.photo
         elif InsureeConfig.insuree_photos_root_path and self.folder and self.filename:
             return load_photo_file(self.folder, self.filename)
         return None
 
     class Meta:
@@ -88,33 +92,41 @@
 
 class InsureeGQLType(DjangoObjectType):
     age = graphene.Int(source='age')
     client_mutation_id = graphene.String()
     photo = PhotoGQLType()
 
     def resolve_current_village(self, info):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_insuree_perms):
+            raise PermissionDenied(_("unauthorized"))
         if "location_loader" in info.context.dataloaders and self.current_village_id:
             return info.context.dataloaders["location_loader"].load(
                 self.current_village_id
             )
         return self.current_village
 
     def resolve_family(self, info):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_insuree_perms):
+            raise PermissionDenied(_("unauthorized"))
         if "family_loader" in info.context.dataloaders and self.family_id:
             return info.context.dataloaders["family_loader"].load(self.family_id)
         return self.family
 
     def resolve_health_facility(self, info):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_insuree_perms):
+            raise PermissionDenied(_("unauthorized"))
         if "health_facililty" in info.context.dataloaders and self.health_facility_id:
             return info.context.dataloaders["health_facility"].load(
                 self.health_facility_id
             )
         return self.health_facility
 
     def resolve_photo(self, info):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_insuree_perms):
+            raise PermissionDenied(_("unauthorized"))
         return self.photo
 
     class Meta:
         model = Insuree
         filter_fields = {
             "uuid": ["exact"],
             "chf_id": ["exact", "istartswith", "icontains", "iexact"],
@@ -133,31 +145,37 @@
             "photo": ["isnull"],
             **prefix_filterset("gender__", GenderGQLType._meta.filter_fields)
         }
         interfaces = (graphene.relay.Node,)
         connection_class = ExtendedConnection
 
     def resolve_client_mutation_id(self, info):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_insuree_perms):
+            raise PermissionDenied(_("unauthorized"))
         insuree_mutation = self.mutations.select_related(
             'mutation').filter(mutation__status=0).first()
         return insuree_mutation.mutation.client_mutation_id if insuree_mutation else None
 
     @classmethod
     def get_queryset(cls, queryset, info):
         return Insuree.get_queryset(queryset, info)
 
 
 class FamilyGQLType(DjangoObjectType):
     client_mutation_id = graphene.String()
 
     def resolve_location(self, info):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_families_perms):
+            raise PermissionDenied(_("unauthorized"))
         if "location_loader" in info.context.dataloaders:
             return info.context.dataloaders["location_loader"].load(self.location_id)
 
     def resolve_head_insuree(self, info):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_families_perms):
+            raise PermissionDenied(_("unauthorized"))
         if "insuree_loader" in info.context.dataloaders:
             return info.context.dataloaders["insuree_loader"].load(self.head_insuree_id)
 
     class Meta:
         model = Family
         filter_fields = {
             "uuid": ["exact"],
@@ -172,14 +190,16 @@
             **prefix_filterset("head_insuree__", InsureeGQLType._meta.filter_fields),
             ** prefix_filterset("members__", InsureeGQLType._meta.filter_fields)
         }
         interfaces = (graphene.relay.Node,)
         connection_class = ExtendedConnection
 
     def resolve_client_mutation_id(self, info):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_families_perms):
+            raise PermissionDenied(_("unauthorized"))
         family_mutation = self.mutations.select_related(
             'mutation').filter(mutation__status=0).first()
         return family_mutation.mutation.client_mutation_id if family_mutation else None
 
     @classmethod
     def get_queryset(cls, queryset, info):
         return Family.get_queryset(queryset, info)
```

### Comparing `openimis-be-insuree-1.5.0/insuree/migrations/0001_initial.py` & `openimis-be-insuree-1.5.1/insuree/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/insuree/migrations/0002_family_familytype_photo.py` & `openimis-be-insuree-1.5.1/insuree/migrations/0002_family_familytype_photo.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/insuree/migrations/0003_insureepolicy.py` & `openimis-be-insuree-1.5.1/insuree/migrations/0003_insureepolicy.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/insuree/migrations/0004_confirmationtype_education_profession_relation.py` & `openimis-be-insuree-1.5.1/insuree/migrations/0004_confirmationtype_education_profession_relation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/insuree/migrations/0005_identificationtype.py` & `openimis-be-insuree-1.5.1/insuree/migrations/0005_identificationtype.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/insuree/migrations/0007_auto_20200722_0940.py` & `openimis-be-insuree-1.5.1/insuree/migrations/0007_auto_20200722_0940.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/insuree/migrations/0009_familymutation_insureemutation.py` & `openimis-be-insuree-1.5.1/insuree/migrations/0009_familymutation_insureemutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/insuree/migrations/0010_auto_20200731_0524.py` & `openimis-be-insuree-1.5.1/insuree/migrations/0010_auto_20200731_0524.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/insuree/migrations/0011_auto_20200807_1309.py` & `openimis-be-insuree-1.5.1/insuree/migrations/0011_auto_20200807_1309.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/insuree/migrations/0012_policyrenewaldetail.py` & `openimis-be-insuree-1.5.1/insuree/migrations/0012_policyrenewaldetail.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/insuree/migrations/0013_auto_20211103_1023.py` & `openimis-be-insuree-1.5.1/insuree/migrations/0013_auto_20211103_1023.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/insuree/models.py` & `openimis-be-insuree-1.5.1/insuree/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         db_column='Gender', max_length=50, blank=True, null=True)
     alt_language = models.CharField(
         db_column='AltLanguage', max_length=50, blank=True, null=True)
     sort_order = models.IntegerField(
         db_column='SortOrder', blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblGender'
 
 
 class InsureePhoto(core_models.VersionedModel):
     id = models.AutoField(db_column='PhotoID', primary_key=True)
     uuid = models.CharField(db_column='PhotoUUID',
                             max_length=36, default=uuid.uuid4, unique=True)
@@ -48,44 +48,44 @@
 
     def full_file_path(self):
         if not InsureeConfig.insuree_photos_root_path or not self.filename:
             return None
         return os.path.join(InsureeConfig.insuree_photos_root_path, self.folder, self.filename)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblPhotos'
 
 
 class FamilyType(models.Model):
     code = models.CharField(
         db_column='FamilyTypeCode', primary_key=True, max_length=2)
     type = models.CharField(db_column='FamilyType', max_length=50)
     sort_order = models.IntegerField(
         db_column='SortOrder', blank=True, null=True)
     alt_language = models.CharField(
         db_column='AltLanguage', max_length=50, blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblFamilyTypes'
 
 
 class ConfirmationType(models.Model):
     code = models.CharField(
         db_column='ConfirmationTypeCode', primary_key=True, max_length=3)
     confirmationtype = models.CharField(
         db_column='ConfirmationType', max_length=50)
     sort_order = models.IntegerField(
         db_column='SortOrder', blank=True, null=True)
     alt_language = models.CharField(
         db_column='AltLanguage', max_length=50, blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblConfirmationTypes'
 
 
 class Family(core_models.VersionedModel, core_models.ExtendableModel):
     id = models.AutoField(db_column='FamilyID', primary_key=True)
     uuid = models.CharField(db_column='FamilyUUID',
                             max_length=36, default=uuid.uuid4, unique=True)
@@ -139,65 +139,65 @@
             dist = UserDistrict.get_user_districts(user._u)
             return queryset.filter(
                 location__parent__parent_id__in=[l.location_id for l in dist]
             )
         return queryset
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblFamilies'
 
 
 class Profession(models.Model):
     id = models.SmallIntegerField(db_column='ProfessionId', primary_key=True)
     profession = models.CharField(db_column='Profession', max_length=50)
     sort_order = models.IntegerField(
         db_column='SortOrder', blank=True, null=True)
     alt_language = models.CharField(
         db_column='AltLanguage', max_length=50, blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblProfessions'
 
 
 class Education(models.Model):
     id = models.SmallIntegerField(db_column='EducationId', primary_key=True)
     education = models.CharField(db_column='Education', max_length=50)
     sort_order = models.IntegerField(
         db_column='SortOrder', blank=True, null=True)
     alt_language = models.CharField(
         db_column='AltLanguage', max_length=50, blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblEducations'
 
 
 class IdentificationType(models.Model):
     code = models.CharField(db_column='IdentificationCode', primary_key=True, max_length=1)  # Field name made lowercase.
     identification_type = models.CharField(db_column='IdentificationTypes', max_length=50)  # Field name made lowercase.
     alt_language = models.CharField(db_column='AltLanguage', max_length=50, blank=True, null=True)  # Field name made lowercase.
     sort_order = models.IntegerField(db_column='SortOrder', blank=True, null=True)  # Field name made lowercase.
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblIdentificationTypes'
 
 
 class Relation(models.Model):
     id = models.SmallIntegerField(db_column='RelationId', primary_key=True)
     relation = models.CharField(db_column='Relation', max_length=50)
     sort_order = models.IntegerField(
         db_column='SortOrder', blank=True, null=True)
     alt_language = models.CharField(
         db_column='AltLanguage', max_length=50, blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblRelations'
 
 
 class Insuree(core_models.VersionedModel, core_models.ExtendableModel):
     id = models.AutoField(db_column='InsureeID', primary_key=True)
     uuid = models.CharField(db_column='InsureeUUID', max_length=36, default=uuid.uuid4, unique=True)
 
@@ -291,15 +291,15 @@
             return queryset.filter(
                 models.Q(family__location__parent__parent_id__in=[l.location.id for l in dist]) |
                 models.Q(family__isnull=True)
             )
         return queryset
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblInsuree'
 
 
 class InsureePolicy(core_models.VersionedModel):
     id = models.AutoField(db_column='InsureePolicyID', primary_key=True)
 
     insuree = models.ForeignKey(Insuree, models.DO_NOTHING, db_column='InsureeID', related_name="insuree_policies")
@@ -332,15 +332,15 @@
             dist = UserDistrict.get_user_districts(user._u)
             return queryset.filter(
                 insuree__family__location__parent__parent_id__in=[l.location_id for l in dist]
             )
         return queryset
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblInsureePolicy'
 
 
 class InsureeMutation(core_models.UUIDModel, core_models.ObjectMutation):
     insuree = models.ForeignKey(Insuree, models.DO_NOTHING, related_name='mutations')
     mutation = models.ForeignKey(core_models.MutationLog, models.DO_NOTHING, related_name='insurees')
 
@@ -369,9 +369,9 @@
                                 related_name='policy_renewal_details')
     policy_renewal = models.ForeignKey('policy.PolicyRenewal', models.DO_NOTHING, db_column='RenewalID',
                                        related_name='details')
 
     audit_user_id = models.IntegerField(db_column='AuditCreateUser', null=True, blank=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblPolicyRenewalDetails'
```

### Comparing `openimis-be-insuree-1.5.0/insuree/reports/enrolled_families.py` & `openimis-be-insuree-1.5.1/insuree/reports/enrolled_families.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/insuree/reports/insuree_family_overview.py` & `openimis-be-insuree-1.5.1/insuree/reports/insuree_family_overview.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/insuree/schema.py` & `openimis-be-insuree-1.5.1/insuree/schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,64 @@
+import graphene
+
+from claim.apps import ClaimConfig
 from core.schema import signal_mutation_module_validate
 from core.utils import filter_validity
 from django.db.models import Q
 from django.core.exceptions import PermissionDenied
 from django.dispatch import Signal
 from graphene_django.filter import DjangoFilterConnectionField
 import graphene_django_optimizer as gql_optimizer
+from location.models import Location, UserDistrict
 
 from .apps import InsureeConfig
 from .models import FamilyMutation, InsureeMutation
 from django.utils.translation import gettext as _
 from location.apps import LocationConfig
 from core.schema import OrderedDjangoFilterConnectionField, OfficerGQLType
+from core.gql_queries import ValidationMessageGQLType
 from policy.models import Policy
 
 # We do need all queries and mutations in the namespace here.
 from .gql_queries import *  # lgtm [py/polluting-import]
 from .gql_mutations import *  # lgtm [py/polluting-import]
-from .signals import signal_before_insuree_policy_query, _read_signal_results, signal_before_family_query
+from .signals import signal_before_insuree_policy_query, _read_signal_results, \
+    signal_before_family_query, signal_before_insuree_search_query
 
 
 def family_fk(arg):
     return arg.startswith("members_") or arg.startswith("head_insuree_")
 
 
 class FamiliesConnectionField(OrderedDjangoFilterConnectionField):
     @classmethod
     def resolve_queryset(
             cls, connection, iterable, info, args, filtering_args, filterset_class
     ):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_families_perms):
+            raise PermissionDenied(_("unauthorized"))
         qs = super(FamiliesConnectionField, cls).resolve_queryset(
             connection, iterable, info,
-            {k: args[k] for k in args.keys() if not k.startswith("members_") and not k.startswith("head_insuree_")},
+            {k: args[k] for k in args.keys() if not k.startswith(
+                "members_") and not k.startswith("head_insuree_")},
             filtering_args,
             filterset_class
         )
-        head_insuree_filters = {k: args[k] for k in args.keys() if k.startswith("head_insuree__")}
-        members_filters = {k: args[k] for k in args.keys() if k.startswith("members__")}
+        head_insuree_filters = {
+            k: args[k] for k in args.keys() if k.startswith("head_insuree__")}
+        members_filters = {k: args[k]
+                           for k in args.keys() if k.startswith("members__")}
         if len(head_insuree_filters) or len(members_filters):
             qs = qs._next_is_sticky()
         if len(head_insuree_filters):
-            qs = qs.filter(Q(head_insuree__validity_to__isnull=True), **head_insuree_filters)
+            qs = qs.filter(
+                Q(head_insuree__validity_to__isnull=True), **head_insuree_filters)
         if len(members_filters):
-            qs = qs.filter(Q(members__validity_to__isnull=True), **members_filters)
+            qs = qs.filter(Q(members__validity_to__isnull=True),
+                           **members_filters)
         return OrderedDjangoFilterConnectionField.orderBy(qs, args)
 
 
 class Query(graphene.ObjectType):
     can_add_insuree = graphene.Field(
         graphene.List(graphene.String),
         family_id=graphene.Int(required=True),
@@ -54,15 +67,17 @@
     insuree_genders = graphene.List(GenderGQLType)
     insurees = OrderedDjangoFilterConnectionField(
         InsureeGQLType,
         show_history=graphene.Boolean(),
         parent_location=graphene.String(),
         parent_location_level=graphene.Int(),
         client_mutation_id=graphene.String(),
+        ignore_location=graphene.Boolean(),
         orderBy=graphene.List(of_type=graphene.String),
+        additional_filters=graphene.JSONString()
     )
     identification_types = graphene.List(IdentificationTypeGQLType)
     educations = graphene.List(EducationGQLType)
     professions = graphene.List(ProfessionGQLType)
     family_types = graphene.List(FamilyTypeGQLType)
     confirmation_types = graphene.List(ConfirmationTypeGQLType)
     relations = graphene.List(RelationGQLType)
@@ -87,28 +102,31 @@
         InsureePolicyGQLType,
         parent_location=graphene.String(),
         parent_location_level=graphene.Int(),
         orderBy=graphene.List(of_type=graphene.String),
         additional_filter=graphene.JSONString(),
     )
     insuree_number_validity = graphene.Field(
-        graphene.Boolean,
+        ValidationMessageGQLType,
         insuree_number=graphene.String(required=True),
-        new_insuree=graphene.Boolean(required=False),
         description="Checks that the specified insuree number is valid"
     )
 
     def resolve_insuree_number_validity(self, info, **kwargs):
-        errors = validate_insuree_number(kwargs['insuree_number'], kwargs.get('new_insuree', False))
+        if not info.context.user.has_perms(InsureeConfig.gql_query_insurees_perms):
+            raise PermissionDenied(_("unauthorized"))
+        errors = validate_insuree_number(kwargs['insuree_number'])
         if errors:
-            return False
+            return ValidationMessageGQLType(False, errors[0]['errorCode'], errors[0]['message'])
         else:
-            return True
+            return ValidationMessageGQLType(True, 0, "")
 
     def resolve_can_add_insuree(self, info, **kwargs):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_insuree_perms):
+            raise PermissionDenied(_("unauthorized"))
         family = Family.objects.get(id=kwargs.get('family_id'))
         warnings = []
         policies = family.policies\
             .filter(validity_to__isnull=True)\
             .exclude(status__in=[Policy.STATUS_EXPIRED, Policy.STATUS_SUSPENDED])
         for policy in policies:
             if not policy.can_add_insuree():
@@ -122,65 +140,99 @@
                             validity_to__isnull=True
                         ).count(),
                     }
                 )
         return warnings
 
     def resolve_insuree_genders(self, info, **kwargs):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_insuree_perms):
+            raise PermissionDenied(_("unauthorized"))
         return Gender.objects.order_by('sort_order').all()
 
     def resolve_insurees(self, info, **kwargs):
         if not info.context.user.has_perms(InsureeConfig.gql_query_insurees_perms):
             raise PermissionDenied(_("unauthorized"))
         filters = []
+        additional_filter = kwargs.get('additional_filters', None)
+        chf_id = kwargs.get('chf_id')
+        if chf_id is not None:
+            filters.append(Q(chf_id=chf_id))
+        if additional_filter:
+            filters_from_signal = _insuree_insuree_additional_filters(
+                sender=self, additional_filter=additional_filter, user=info.context.user
+            )
+            filters.extend(filters_from_signal)
         show_history = kwargs.get('show_history', False)
         if not show_history and not kwargs.get('uuid', None):
             filters += filter_validity(**kwargs)
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
-            filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
+            filters.append(
+                Q(mutations__mutation__client_mutation_id=client_mutation_id))
         parent_location = kwargs.get('parent_location')
         if parent_location is not None:
             parent_location_level = kwargs.get('parent_location_level')
             if parent_location_level is None:
-                raise NotImplementedError("Missing parentLocationLevel argument when filtering on parentLocation")
+                raise ValueError(
+                    "Missing parentLocationLevel argument when filtering on parentLocation")
             f = "uuid"
             for i in range(len(LocationConfig.location_types) - parent_location_level - 1):
                 f = "parent__" + f
             current_village = "current_village__" + f
             family_location = "family__location__" + f
             filters += [(Q(current_village__isnull=False) & Q(**{current_village: parent_location})) |
                         (Q(current_village__isnull=True) & Q(**{family_location: parent_location}))]
+
+        if (kwargs.get('ignore_location') == False or kwargs.get('ignore_location') is None):
+            # Limit the list by the logged in user location mapping
+            user_districts = UserDistrict.get_user_districts(
+                info.context.user._u)
+
+            filters += [Q(family__location__parent__parent__in=Location.objects.filter(
+                uuid__in=user_districts.values_list('location__uuid', flat=True)))]
+
         return gql_optimizer.query(Insuree.objects.filter(*filters).all(), info)
 
     def resolve_family_members(self, info, **kwargs):
-        if not info.context.user.has_perms(InsureeConfig.gql_query_insurees_perms):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_insuree_family_members):
             raise PermissionDenied(_("unauthorized"))
         family = Family.objects.get(Q(uuid=kwargs.get('family_uuid')))
         return Insuree.objects.filter(
             Q(family=family),
             *filter_validity(**kwargs)
         ).order_by('-head', 'dob')
 
     def resolve_educations(self, info, **kwargs):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_families_perms):
+            raise PermissionDenied(_("unauthorized"))
         return Education.objects.order_by('sort_order').all()
 
     def resolve_professions(self, info, **kwargs):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_families_perms):
+            raise PermissionDenied(_("unauthorized"))
         return Profession.objects.order_by('sort_order').all()
 
     def resolve_identification_types(self, info, **kwargs):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_families_perms):
+            raise PermissionDenied(_("unauthorized"))
         return IdentificationType.objects.order_by('sort_order').all()
 
     def resolve_confirmation_types(self, info, **kwargs):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_families_perms):
+            raise PermissionDenied(_("unauthorized"))
         return ConfirmationType.objects.order_by('sort_order').all()
 
     def resolve_relations(self, info, **kwargs):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_families_perms):
+            raise PermissionDenied(_("unauthorized"))
         return Relation.objects.order_by('sort_order').all()
 
     def resolve_family_types(self, info, **kwargs):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_families_perms):
+            raise PermissionDenied(_("unauthorized"))
         return FamilyType.objects.order_by('sort_order').all()
 
     def resolve_families(self, info, **kwargs):
         if not info.context.user.has_perms(InsureeConfig.gql_query_families_perms):
             raise PermissionDenied(_("unauthorized"))
 
         filters = []
@@ -189,47 +241,60 @@
             filters_from_signal = _family_additional_filters(
                 sender=self, additional_filter=additional_filter, user=info.context.user
             )
             filters.extend(filters_from_signal)
 
         officer = kwargs.get('officer', None)
         if officer:
-            officer_policies_families = Policy.objects.filter(officer__uuid=officer).values_list('family', flat=True)
+            officer_policies_families = Policy.objects.filter(
+                officer__uuid=officer).values_list('family', flat=True)
             filters.append(Q(id__in=officer_policies_families))
 
         null_as_false_poverty = kwargs.get('null_as_false_poverty')
         if null_as_false_poverty is not None:
-            filters += [Q(poverty=True)] if null_as_false_poverty else [Q(poverty=False) | Q(poverty__isnull=True)]
+            filters += [Q(poverty=True)] if null_as_false_poverty else [
+                Q(poverty=False) | Q(poverty__isnull=True)]
         show_history = kwargs.get('show_history', False)
         if not show_history:
             filters += filter_validity(**kwargs)
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
-            filters.append(Q(mutations__mutation__client_mutation_id=client_mutation_id))
+            filters.append(
+                Q(mutations__mutation__client_mutation_id=client_mutation_id))
         parent_location = kwargs.get('parent_location')
         if parent_location is not None:
             parent_location_level = kwargs.get('parent_location_level')
             if parent_location_level is None:
-                raise NotImplementedError("Missing parentLocationLevel argument when filtering on parentLocation")
+                raise NotImplementedError(
+                    "Missing parentLocationLevel argument when filtering on parentLocation")
             f = "uuid"
             for i in range(len(LocationConfig.location_types) - parent_location_level - 1):
                 f = "parent__" + f
             f = "location__" + f
             filters += [Q(**{f: parent_location})]
 
+        # Limit the list by the logged in user location mapping
+        user_districts = UserDistrict.get_user_districts(
+            info.context.user._u)
+
+        filters += [Q(location__parent__parent__in=Location.objects.filter(
+            uuid__in=user_districts.values_list('location__uuid', flat=True)))]
+
         # Duplicates cannot be removed with distinct, as TEXT field is not comparable
         ids = Family.objects.filter(*filters).values_list('id')
         dinstinct_queryset = Family.objects.filter(id__in=ids)
         return gql_optimizer.query(dinstinct_queryset.all(), info)
 
     def resolve_insuree_officers(self, info, **kwargs):
         if not info.context.user.has_perms(InsureeConfig.gql_query_insuree_officers_perms):
             raise PermissionDenied(_("unauthorized"))
 
     def resolve_insuree_policy(self, info, **kwargs):
+        if not info.context.user.has_perms(InsureeConfig.gql_query_insuree_policy_perms):
+            raise PermissionDenied(_("unauthorized"))
         filters = []
         additional_filter = kwargs.get('additional_filter', None)
         # go to process additional filter only when this arg of filter was passed into query
         if additional_filter:
             filters_from_signal = _insuree_additional_filters(
                 sender=self, additional_filter=additional_filter, user=info.context.user
             )
@@ -239,15 +304,16 @@
             filters.extend(filters_from_signal)
         if not info.context.user.has_perms(InsureeConfig.gql_query_insuree_policy_perms):
             raise PermissionDenied(_("unauthorized"))
         parent_location = kwargs.get('parent_location')
         if parent_location is not None:
             parent_location_level = kwargs.get('parent_location_level')
             if parent_location_level is None:
-                raise NotImplementedError("Missing parentLocationLevel argument when filtering on parentLocation")
+                raise NotImplementedError(
+                    "Missing parentLocationLevel argument when filtering on parentLocation")
             f = "uuid"
             for i in range(len(LocationConfig.location_types) - parent_location_level - 1):
                 f = "parent__" + f
             current_village = "current_village__" + f
             family_location = "family__location__" + f
             filters += [(Q(current_village__isnull=False) & Q(**{current_village: parent_location})) |
                         (Q(current_village__isnull=True) & Q(**{family_location: parent_location}))]
@@ -267,15 +333,16 @@
 
 
 def on_family_mutation(kwargs, k='uuid'):
     family_uuid = kwargs['data'].get('uuid', None)
     if not family_uuid:
         return []
     impacted_family = Family.objects.get(Q(uuid=family_uuid))
-    FamilyMutation.objects.create(family=impacted_family, mutation_id=kwargs['mutation_log_id'])
+    FamilyMutation.objects.create(
+        family=impacted_family, mutation_id=kwargs['mutation_log_id'])
     return []
 
 
 def on_families_mutation(kwargs):
     uuids = kwargs['data'].get('uuids', [])
     if not uuids:
         uuid = kwargs['data'].get('uuid', None)
@@ -290,15 +357,16 @@
 
 
 def on_insuree_mutation(kwargs, k='uuid'):
     insuree_uuid = kwargs['data'].get('uuid', None)
     if not insuree_uuid:
         return []
     impacted_insuree = Insuree.objects.get(Q(uuid=insuree_uuid))
-    InsureeMutation.objects.create(insuree=impacted_insuree, mutation_id=kwargs['mutation_log_id'])
+    InsureeMutation.objects.create(
+        insuree=impacted_insuree, mutation_id=kwargs['mutation_log_id'])
     return []
 
 
 def on_insurees_mutation(kwargs):
     uuids = kwargs['data'].get('uuids', [])
     if not uuids:
         uuid = kwargs['data'].get('uuid', None)
@@ -341,14 +409,17 @@
 def bind_signals():
     signal_mutation_module_validate["insuree"].connect(on_mutation)
 
 
 def _insuree_additional_filters(sender, additional_filter, user):
     return _get_additional_filter(sender, additional_filter, user, signal_before_insuree_policy_query)
 
+def _insuree_insuree_additional_filters(sender, additional_filter, user):
+    return _get_additional_filter(sender, additional_filter, user, signal_before_insuree_search_query)
+
 
 def _family_additional_filters(sender, additional_filter, user):
     return _get_additional_filter(sender, additional_filter, user, signal_before_family_query)
 
 
 def _get_additional_filter(sender, additional_filter, user, signal: Signal):
     # function to retrieve additional filters from signal
```

### Comparing `openimis-be-insuree-1.5.0/insuree/services.py` & `openimis-be-insuree-1.5.1/insuree/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,48 +37,75 @@
             validity_from=now,
             audit_user_id=0,
         )
         logger.debug("Photo due for renewal for insuree %s, renewal detail %s, created an entry ? %s",
                      photo.insuree_id, detail.id, detail_created)
 
 
-def validate_insuree_number(insuree_number, is_new_insuree=False):
-    if is_new_insuree:
-        if Insuree.objects.filter(chf_id=insuree_number).exists():
-            return [{"message": "Insuree number has to be unique, %s exists in system" % insuree_number}]
+def validate_insuree_number(insuree_number, uuid=None):
+    query = Insuree.objects.filter(chf_id=insuree_number, validity_to__isnull=True)
+    insuree = query.first()
+    if insuree and insuree.uuid != uuid:
+        return [{"errorCode": InsureeConfig.validation_code_taken_insuree_number,
+                 "message": "Insuree number has to be unique, %s exists in system" % insuree_number}]
 
     if InsureeConfig.get_insuree_number_validator():
         return InsureeConfig.get_insuree_number_validator()(insuree_number)
     if InsureeConfig.get_insuree_number_length():
         if not insuree_number:
             return [
                 {
+                    "errorCode": InsureeConfig.validation_code_no_insuree_number,
                     "message": "Invalid insuree number (empty), should be %s" %
                                (InsureeConfig.get_insuree_number_length(),)
                 }
             ]
         if len(insuree_number) != InsureeConfig.get_insuree_number_length():
             return [
                 {
+                    "errorCode": InsureeConfig.validation_code_invalid_insuree_number_len,
                     "message": "Invalid insuree number length %s, should be %s" %
                                (len(insuree_number), InsureeConfig.get_insuree_number_length())
                 }
             ]
-    if InsureeConfig.get_insuree_number_modulo_root():
+    config_modulo = InsureeConfig.get_insuree_number_modulo_root()
+    if config_modulo:
         try:
-            base = int(insuree_number[:-1])
-            mod = int(insuree_number[-1])
-            if base % InsureeConfig.get_insuree_number_modulo_root() != mod:
-                return [{"message": "Invalid checksum"}]
+            if config_modulo == 10:
+                if not is_modulo_10_number_valid(insuree_number):
+                    return invalid_checksum()
+            else:
+                base = int(insuree_number[:-1])
+                mod = int(insuree_number[-1])
+                if base % config_modulo != mod:
+                    return invalid_checksum()
         except Exception as exc:
             logger.exception("Failed insuree number validation", exc)
-            return [{"message": "Insuree number validation failed"}]
+            return [{"errorCode": InsureeConfig.validation_code_invalid_insuree_number_exception,
+                     "message": "Insuree number validation failed"}]
     return []
 
 
+def is_modulo_10_number_valid(insuree_number: str) -> bool:
+    """
+    This function checks whether an insuree number is valid, according to the modulo 10 technique.
+    Contrarily to its name, this technique does not simply check if number % 10 == 0.
+    This function uses Luhn's algorithm (https://en.wikipedia.org/wiki/Luhn_algorithm).
+    """
+    return (sum(
+        (element + (index % 2 == 0) * (element - 9 * (element > 4))
+         for index, element in enumerate(map(int, insuree_number[:-1])))
+    ) + int(insuree_number[-1])) % 10 == 0
+
+
+def invalid_checksum():
+    return [{"errorCode": InsureeConfig.validation_code_invalid_insuree_number_checksum,
+             "message": "Invalid checksum"}]
+
+
 def reset_insuree_before_update(insuree):
     insuree.family = None
     insuree.chf_id = None
     insuree.last_name = None
     insuree.other_names = None
     insuree.gender = None
     insuree.dob = None
@@ -139,29 +166,29 @@
         insuree_photo = InsureePhoto.objects.create(**data)
     insuree_photo.save()
     return insuree_photo
 
 
 def photo_changed(insuree_photo, data):
     return (not insuree_photo and data) or \
-           (data and insuree_photo and insuree_photo.date != data.get('date', None)) or \
-           (data and insuree_photo and insuree_photo.officer_id != data.get('officer_id', None)) or \
-           (data and insuree_photo and insuree_photo.folder != data.get('folder', None)) or \
-           (data and insuree_photo and insuree_photo.filename != data.get('filename', None)) or \
-           (data and insuree_photo and insuree_photo.photo != data.get('photo', None))
+        (data and insuree_photo and insuree_photo.date != data.get('date', None)) or \
+        (data and insuree_photo and insuree_photo.officer_id != data.get('officer_id', None)) or \
+        (data and insuree_photo and insuree_photo.folder != data.get('folder', None)) or \
+        (data and insuree_photo and insuree_photo.filename != data.get('filename', None)) or \
+        (data and insuree_photo and insuree_photo.photo != data.get('photo', None))
 
 
 def _photo_dir(file_dir, file_name):
     root = InsureeConfig.insuree_photos_root_path
     return path.join(root, file_dir, file_name)
 
 
 def _create_dir(file_dir):
     root = InsureeConfig.insuree_photos_root_path
-    pathlib.Path(path.join(root, file_dir))\
+    pathlib.Path(path.join(root, file_dir)) \
         .mkdir(parents=True, exist_ok=True)
 
 
 def create_file(date, insuree_id, photo_bin):
     file_dir = path.join(str(date.year), str(date.month), str(date.day), str(insuree_id))
     file_name = str(uuid.uuid4())
 
@@ -195,27 +222,26 @@
     def create_or_update(self, data):
         photo = data.pop('photo', None)
         from core import datetime
         now = datetime.datetime.now()
         data['audit_user_id'] = self.user.id_for_audit
         data['validity_from'] = now
         insuree_uuid = data.pop('uuid', None)
+        errors = validate_insuree_number(data["chf_id"], insuree_uuid)
+        if errors:
+            raise Exception("Invalid insuree number")
         if insuree_uuid:
             insuree = Insuree.objects.prefetch_related("photo").get(uuid=insuree_uuid)
             insuree.save_history()
             # reset the non required fields
             # (each update is 'complete', necessary to be able to set 'null')
             reset_insuree_before_update(insuree)
             [setattr(insuree, key, data[key]) for key in data]
         else:
-            errors = validate_insuree_number(data["chf_id"])
-            if errors:
-                raise Exception("Invalid insuree number")
-            else:
-                insuree = Insuree.objects.create(**data)
+            insuree = Insuree.objects.create(**data)
         insuree.save()
         photo = handle_insuree_photo(self.user, now, insuree, photo)
         if photo:
             insuree.photo = photo
             insuree.photo_date = photo.date
             insuree.save()
         return insuree
```

### Comparing `openimis-be-insuree-1.5.0/insuree/test_helpers.py` & `openimis-be-insuree-1.5.1/insuree/test_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 from insuree.models import Insuree, Family, Gender, InsureePhoto
 
 
-def create_test_insuree(with_family=True, custom_props=None, family_custom_props={}):
+def create_test_insuree(with_family=True, is_head=False, custom_props=None, family_custom_props=None):
     # insuree has a mandatory reference to family and family has a mandatory reference to insuree
     # So we first insert the family with a dummy id and then update it
     if with_family:
         family = Family.objects.create(
             validity_from="2019-01-01",
             head_insuree_id=1,  # dummy
             audit_user_id=-1,
+            **(family_custom_props if family_custom_props else {})
         )
     else:
         family = None
 
     insuree = Insuree.objects.create(
         **{
             "last_name": "Test Last",
             "other_names": "First Second",
             "chf_id": "chf_dflt",
             "family": family,
             "gender": Gender.objects.get(code='M'),
             "dob": "1970-01-01",
-            "head": True,
+            "head": is_head,
             "card_issued": True,
             "validity_from": "2019-01-01",
             "audit_user_id": -1,
             **(custom_props if custom_props else {})
         }
     )
     if with_family:
         family.head_insuree_id = insuree.id
-        for k, v in family_custom_props.items():
-            setattr(family, k, v)
+        if family_custom_props:
+            for k, v in family_custom_props.items():
+                setattr(family, k, v)
         family.save()
 
     return insuree
 
 
 base64_blank_jpg = """
 /9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAgGBgcGBQgHBwcJCQgKDBQNDAsLDBkSEw8UHRofHh0aHBwgJC4nICIsIxwcKDcpLDAxNDQ0Hyc5PTgyPC4zNDL
```

### Comparing `openimis-be-insuree-1.5.0/insuree/tests/test_graphql.py` & `openimis-be-insuree-1.5.1/insuree/tests/test_graphql.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,20 @@
         assign_user_districts(cls.admin_dist_user, ["R1D1", "R2D1", "R2D2"])
         cls.admin_dist_token = get_token(cls.admin_dist_user, DummyContext(user=cls.admin_dist_user))
 
     def test_query_insuree_number_validity(self):
         response = self.query(
             '''
             {
-                insureeNumberValidity(insureeNumber:"123456782", newInsuree:false)
+                insureeNumberValidity(insureeNumber:"123456782")
+                {
+                  isValid
+                  errorCode
+                  errorMessage
+                }
             }
             ''',
             headers={"HTTP_AUTHORIZATION": f"Bearer {self.admin_token}"},
         )
 
         self.assertEquals(response.status_code, status.HTTP_200_OK)
         content = json.loads(response.content)
```

### Comparing `openimis-be-insuree-1.5.0/insuree/tests/test_insuree_validation.py` & `openimis-be-insuree-1.5.1/insuree/tests/test_insuree_validation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-insuree-1.5.0/openimis_be_insuree.egg-info/PKG-INFO` & `openimis-be-insuree-1.5.1/openimis_be_insuree.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: openimis-be-insuree
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Insuree reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE.md
```

### Comparing `openimis-be-insuree-1.5.0/openimis_be_insuree.egg-info/SOURCES.txt` & `openimis-be-insuree-1.5.1/openimis_be_insuree.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,31 +12,38 @@
 insuree/report.py
 insuree/schema.py
 insuree/services.py
 insuree/signals.py
 insuree/test_helpers.py
 insuree/urls.py
 insuree/views.py
+insuree/management/__init__.py
+insuree/management/commands/__init__.py
+insuree/management/commands/generateinsurees.py
 insuree/migrations/0001_initial.py
 insuree/migrations/0002_family_familytype_photo.py
 insuree/migrations/0003_insureepolicy.py
 insuree/migrations/0004_confirmationtype_education_profession_relation.py
 insuree/migrations/0005_identificationtype.py
 insuree/migrations/0006_auto_20200722_0839.py
 insuree/migrations/0007_auto_20200722_0940.py
 insuree/migrations/0008_auto_20200731_0443.py
 insuree/migrations/0009_familymutation_insureemutation.py
 insuree/migrations/0010_auto_20200731_0524.py
 insuree/migrations/0011_auto_20200807_1309.py
 insuree/migrations/0012_policyrenewaldetail.py
 insuree/migrations/0013_auto_20211103_1023.py
+insuree/migrations/0014_add_missing_fields_to_django_scheme.py
+insuree/migrations/0015_set_managed_to_true_in_all_models.py
 insuree/migrations/__init__.py
 insuree/reports/__init__.py
 insuree/reports/enrolled_families.py
 insuree/reports/insuree_family_overview.py
+insuree/reports/insuree_missing_photo.py
+insuree/reports/insurees_pending_enrollment.py
 insuree/tests/__init__.py
 insuree/tests/test_graphql.py
 insuree/tests/test_insuree_photo.py
 insuree/tests/test_insuree_validation.py
 openimis_be_insuree.egg-info/PKG-INFO
 openimis_be_insuree.egg-info/SOURCES.txt
 openimis_be_insuree.egg-info/dependency_links.txt
```

### Comparing `openimis-be-insuree-1.5.0/setup.py` & `openimis-be-insuree-1.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-insuree',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Insuree reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
@@ -23,16 +23,18 @@
         'django-db-signals',
         'djangorestframework',
         'openimis-be-location',
     ],
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
-        'Framework :: Django :: 3.0',
+        'Framework :: Django :: 3.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
 )
```

