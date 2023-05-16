# Comparing `tmp/openimis-be-claim-1.5.0.tar.gz` & `tmp/openimis-be-claim-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-claim-1.5.0.tar", last modified: Thu Nov 10 18:10:06 2022, max compression
+gzip compressed data, was "openimis-be-claim-1.5.1.tar", last modified: Tue May 16 21:38:23 2023, max compression
```

## Comparing `openimis-be-claim-1.5.0.tar` & `openimis-be-claim-1.5.1.tar`

### file list

```diff
@@ -1,47 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:10:06.252315 openimis-be-claim-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-11-10 18:10:06.252315 openimis-be-claim-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5273 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:10:06.252315 openimis-be-claim-1.5.0/claim/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     4633 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)    36683 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     5597 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:10:06.252315 openimis-be-claim-1.5.0/claim/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    14746 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/migrations/0002_batchrun.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/migrations/0003_claimofficer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/migrations/0004_claimattachment.py
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/migrations/0005_claimmutation.py
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/migrations/0006_claimattachment_url.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/migrations/0007_auto_20200318_1443.py
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/migrations/0008_create_claim_attachments_count_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     3223 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/migrations/0009_auto_20200421_1657.py
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/migrations/0010_auto_20200611_0601.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/migrations/0011_auto_20201126_1244.py
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/migrations/0012_item_service_jsonExtField.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23397 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:10:06.252315 openimis-be-claim-1.5.0/claim/reports/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   112176 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/reports/claim.py
--rw-r--r--   0 runner    (1001) docker     (121)     6494 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    14585 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     3164 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10061 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/test_services.py
--rw-r--r--   0 runner    (1001) docker     (121)    42350 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/test_validations.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    66939 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/validations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-11-10 18:09:54.000000 openimis-be-claim-1.5.0/claim/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:10:06.252315 openimis-be-claim-1.5.0/openimis_be_claim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-11-10 18:10:06.000000 openimis-be-claim-1.5.0/openimis_be_claim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-11-10 18:10:06.000000 openimis-be-claim-1.5.0/openimis_be_claim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 18:10:06.000000 openimis-be-claim-1.5.0/openimis_be_claim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-11-10 18:10:06.000000 openimis-be-claim-1.5.0/openimis_be_claim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-10 18:10:06.000000 openimis-be-claim-1.5.0/openimis_be_claim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 18:10:06.252315 openimis-be-claim-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-11-10 18:10:04.000000 openimis-be-claim-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:23.900708 openimis-be-claim-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-16 21:38:23.900708 openimis-be-claim-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:23.896708 openimis-be-claim-1.5.1/claim/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38595 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:23.896708 openimis-be-claim-1.5.1/claim/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:23.896708 openimis-be-claim-1.5.1/claim/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/management/commands/generateclaimadmins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/management/commands/generateclaims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:23.900708 openimis-be-claim-1.5.1/claim/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0002_batchrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0003_claimofficer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0004_claimattachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0005_claimmutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0006_claimattachment_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0007_auto_20200318_1443.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0008_create_claim_attachments_count_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0009_auto_20200421_1657.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0010_auto_20200611_0601.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0011_auto_20201126_1244.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0012_item_service_jsonExtField.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0013_feedbackprompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0014_change_code_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0015_prohibit_interaction_for_enrolment_officer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11532 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0016_update_django_scheme_with_missing_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/0017_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25911 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:23.900708 openimis-be-claim-1.5.1/claim/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112176 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/reports/claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47457 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/reports/claim_percentage_referrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42350 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/test_validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67259 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-16 21:38:12.000000 openimis-be-claim-1.5.1/claim/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:23.900708 openimis-be-claim-1.5.1/openimis_be_claim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-16 21:38:23.000000 openimis-be-claim-1.5.1/openimis_be_claim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-16 21:38:23.000000 openimis-be-claim-1.5.1/openimis_be_claim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:38:23.000000 openimis-be-claim-1.5.1/openimis_be_claim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-16 21:38:23.000000 openimis-be-claim-1.5.1/openimis_be_claim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 21:38:23.000000 openimis-be-claim-1.5.1/openimis_be_claim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:38:23.900708 openimis-be-claim-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-16 21:38:21.000000 openimis-be-claim-1.5.1/setup.py
```

### Comparing `openimis-be-claim-1.5.0/LICENSE.md` & `openimis-be-claim-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/PKG-INFO` & `openimis-be-claim-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-claim
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Claim reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-claim-1.5.0/README.md` & `openimis-be-claim-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/claim/apps.py` & `openimis-be-claim-1.5.1/claim/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/claim/gql_mutations.py` & `openimis-be-claim-1.5.1/claim/gql_mutations.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,26 @@
 from claim.validations import validate_claim, get_claim_category, validate_assign_prod_to_claimitems_and_services, \
     process_dedrem, approved_amount
 from core import filter_validity, assert_string_length
 from core.schema import TinyInt, SmallInt, OpenIMISMutation
 from core.gql.gql_mutations import mutation_on_uuids_from_filter
 from django.conf import settings
 from django.contrib.auth.models import AnonymousUser
-from django.core.exceptions import ValidationError, PermissionDenied
+from django.core.exceptions import ValidationError, PermissionDenied, ObjectDoesNotExist
 from django.utils.translation import gettext as _
 from graphene import InputObjectType
 from location.schema import UserDistrict
 
 from claim.gql_queries import ClaimGQLType
-from claim.models import Claim, Feedback, ClaimDetail, ClaimItem, ClaimService, ClaimAttachment, ClaimDedRem
+from claim.models import Claim, Feedback, FeedbackPrompt, ClaimDetail, ClaimItem, ClaimService, ClaimAttachment, \
+    ClaimDedRem
 from product.models import ProductItemOrService
 
 from claim.utils import process_items_relations, process_services_relations
-
+from .services import check_unique_claim_code
 logger = logging.getLogger(__name__)
 
 
 class ClaimItemInputType(InputObjectType):
     id = graphene.Int(required=False)
     item_id = graphene.Int(required=True)
     status = TinyInt(required=True)
@@ -270,19 +271,25 @@
     for attachment in attachments:
         create_attachment(claim_id, attachment)
 
 
 def update_or_create_claim(data, user):
     items = data.pop('items') if 'items' in data else []
     services = data.pop('services') if 'services' in data else []
+    incoming_code = data.get('code')
+    claim_uuid = data.pop("uuid", None)
+    current_claim = Claim.objects.filter(uuid=claim_uuid).first()
+    current_code = current_claim.code if current_claim else None
+    if current_code != incoming_code \
+            and check_unique_claim_code(incoming_code):
+        raise ValidationError(_("mutation.code_name_duplicated"))
     if "client_mutation_id" in data:
         data.pop('client_mutation_id')
     if "client_mutation_label" in data:
         data.pop('client_mutation_label')
-    claim_uuid = data.pop('uuid') if 'uuid' in data else None
     # update_or_create(uuid=claim_uuid, ...)
     # doesn't work because of explicit attempt to set null to uuid!
     if claim_uuid:
         claim = Claim.objects.get(uuid=claim_uuid)
         claim.save_history()
         # reset the non required fields
         # (each update is 'complete', necessary to be able to set 'null')
@@ -541,40 +548,72 @@
                 })
         if len(errors) == 1:
             errors = errors[0]['list']
         logger.debug("SubmitClaimsMutation: claim done, errors: %s", len(errors))
         return errors
 
 
-def set_claims_status(uuids, field, status, audit_data=None):
+def set_claims_status(uuids, field, status, audit_data=None, user=None):
     errors = []
     for claim_uuid in uuids:
         claim = Claim.objects \
             .filter(uuid=claim_uuid,
                     validity_to__isnull=True) \
             .first()
         if claim is None:
             errors += [{'message': _(
                 "claim.validation.id_does_not_exist") % {'id': claim_uuid}}]
             continue
         try:
             claim.save_history()
             setattr(claim, field, status)
+            # creating/cancelling feedback prompts
+            if field == 'feedback_status':
+                if status == Claim.FEEDBACK_SELECTED:
+                    create_feedback_prompt(claim_uuid, user)
+                elif status in [Claim.FEEDBACK_NOT_SELECTED, Claim.FEEDBACK_BYPASSED]:
+                    set_feedback_prompt_validity_to_to_current_date(claim_uuid)
             if audit_data:
                 for k, v in audit_data.items():
                     setattr(claim, k, v)
             claim.save()
         except Exception as exc:
             errors += [
                 {'message': _("claim.mutation.failed_to_change_status_of_claim") %
                             {'code': claim.code}}]
 
     return errors
 
 
+def create_feedback_prompt(claim_uuid, user):
+    current_claim = Claim.objects.get(uuid=claim_uuid)
+    feedback_prompt = {}
+    from core.utils import TimeUtils
+    feedback_prompt['feedback_prompt_date'] = TimeUtils.date()
+    feedback_prompt['validity_from'] = TimeUtils.now()
+    feedback_prompt['claim_id'] = current_claim
+    feedback_prompt['officer_id'] = current_claim.admin_id
+    feedback_prompt['audit_user_id'] = user.id_for_audit
+    FeedbackPrompt.objects.create(
+        **feedback_prompt
+    )
+
+
+def set_feedback_prompt_validity_to_to_current_date(claim_uuid):
+    try:
+        claim_id = Claim.objects.get(uuid=claim_uuid).id
+        feedback_prompt_id = FeedbackPrompt.objects.get(claim_id=claim_id, validity_to=None).id
+        from core.utils import TimeUtils
+        current_feedback_prompt = FeedbackPrompt.objects.get(id=feedback_prompt_id)
+        current_feedback_prompt.validity_to = TimeUtils.now()
+        current_feedback_prompt.save()
+    except ObjectDoesNotExist:
+        return "No such feedback prompt exist."
+
+
 def update_claims_dedrems(uuids, user):
     # We could do it in one query with filter(claim__uuid__in=uuids) but we'd loose the logging
     errors = []
     for uuid in uuids:
         logger.debug(f"delivering review on {uuid}, reprocessing dedrem ({user})")
         claim = Claim.objects.get(uuid=uuid)
         errors += validate_and_process_dedrem_claim(claim, user, False)
@@ -591,15 +630,15 @@
     class Input(OpenIMISMutation.Input):
         uuids = graphene.List(graphene.String)
 
     @classmethod
     def async_mutate(cls, user, **data):
         if not user.has_perms(ClaimConfig.gql_mutation_select_claim_feedback_perms):
             raise PermissionDenied(_("unauthorized"))
-        return set_claims_status(data['uuids'], 'feedback_status', Claim.FEEDBACK_SELECTED)
+        return set_claims_status(data['uuids'], 'feedback_status', Claim.FEEDBACK_SELECTED, user=user)
 
 
 class BypassClaimsFeedbackMutation(OpenIMISMutation):
     """
     Bypass feedback for one or several claims
     """
     _mutation_module = "claim"
@@ -667,14 +706,15 @@
                 claim=claim,
                 defaults=feedback
             )
             claim.feedback = f
             claim.feedback_status = Claim.FEEDBACK_DELIVERED
             claim.feedback_available = True
             claim.save()
+            set_feedback_prompt_validity_to_to_current_date(claim.uuid)
             return None
         except Exception as exc:
             return [{
                 'message': _("claim.mutation.failed_to_update_claim") % {'code': claim.code if claim else None},
                 'detail': str(exc)}]
```

### Comparing `openimis-be-claim-1.5.0/claim/gql_queries.py` & `openimis-be-claim-1.5.1/claim/gql_queries.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from core import prefix_filterset, ExtendedConnection, filter_validity
 from graphene.utils.deduplicator import deflate
 from graphene_django import DjangoObjectType
 from insuree.schema import InsureeGQLType
 from location.schema import HealthFacilityGQLType
 from medical.schema import DiagnosisGQLType
 from claim_batch.schema import BatchRunGQLType
+from .apps import ClaimConfig
 from .models import ClaimDedRem, Claim, ClaimAdmin, Feedback, ClaimItem, ClaimService, ClaimAttachment
+from django.utils.translation import gettext as _
+from django.core.exceptions import PermissionDenied
 
 
 class ClaimDedRemGQLType(DjangoObjectType):
     """
     Details about Claim demands and remunerated amounts
     """
     class Meta:
@@ -50,19 +53,23 @@
     """
 
     attachments_count = graphene.Int()
     client_mutation_id = graphene.String()
     date_processed_to = graphene.Date()
 
     def resolve_insuree(self, info):
+        if not info.context.user.has_perms(ClaimConfig.gql_query_claims_perms):
+            raise PermissionDenied(_("unauthorized"))
         if "insuree_loader" in info.context.dataloaders and self.insuree_id:
             return info.context.dataloaders["insuree_loader"].load(self.insuree_id)
         return self.insuree
 
     def resolve_health_facility(self, info):
+        if not info.context.user.has_perms(ClaimConfig.gql_query_claims_perms):
+            raise PermissionDenied(_("unauthorized"))
         if (
             "health_facility_loader" in info.context.dataloaders
             and self.health_facility_id
         ):
             return info.context.dataloaders["health_facility_loader"].load(
                 self.health_facility_id
             )
@@ -70,15 +77,15 @@
 
     class Meta:
         model = Claim
         interfaces = (graphene.relay.Node,)
         filter_fields = {
             "uuid": ["exact"],
             "code": ["exact", "istartswith", "icontains", "iexact"],
-            "status": ["exact"],
+            "status": ["exact", "gt"],
             "date_claimed": ["exact", "lt", "lte", "gt", "gte"],
             "date_from": ["exact", "lt", "lte", "gt", "gte"],
             "date_to": ["exact", "lt", "lte", "gt", "gte"],
             "date_processed": ["exact", "lt", "lte", "gt", "gte"],
             "feedback_status": ["exact"],
             "review_status": ["exact"],
             "claimed": ["exact", "lt", "lte", "gt", "gte"],
@@ -90,23 +97,31 @@
             **prefix_filterset("health_facility__", HealthFacilityGQLType._meta.filter_fields),
             **prefix_filterset("insuree__", InsureeGQLType._meta.filter_fields),
             **prefix_filterset("batch_run__", BatchRunGQLType._meta.filter_fields)
         }
         connection_class = ExtendedConnection
 
     def resolve_attachments_count(self, info):
-        return self.attachments.filter(legacy_id__isnull=True).count()
+        if not info.context.user.has_perms(ClaimConfig.gql_query_claims_perms):
+            raise PermissionDenied(_("unauthorized"))
+        return self.attachments.filter(legacy_id__isnull=True).filter(validity_to__isnull=True).count()
 
     def resolve_items(self, info):
+        if not info.context.user.has_perms(ClaimConfig.gql_query_claims_perms):
+            raise PermissionDenied(_("unauthorized"))
         return self.items.filter(legacy_id__isnull=True).filter(validity_to__isnull=True)
 
     def resolve_services(self, info):
+        if not info.context.user.has_perms(ClaimConfig.gql_query_claims_perms):
+            raise PermissionDenied(_("unauthorized"))
         return self.services.filter(legacy_id__isnull=True).filter(validity_to__isnull=True)
 
     def resolve_client_mutation_id(self, info):
+        if not info.context.user.has_perms(ClaimConfig.gql_query_claims_perms):
+            raise PermissionDenied(_("unauthorized"))
         claim_mutation = self.mutations.select_related(
             'mutation').filter(mutation__status=0).first()
         return claim_mutation.mutation.client_mutation_id if claim_mutation else None
 
     @classmethod
     def get_queryset(cls, queryset, info):
         claim_ids = Claim.get_queryset(queryset, info).values('uuid').all()
```

### Comparing `openimis-be-claim-1.5.0/claim/migrations/0001_initial.py` & `openimis-be-claim-1.5.1/claim/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/claim/migrations/0002_batchrun.py` & `openimis-be-claim-1.5.1/claim/migrations/0002_batchrun.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/claim/migrations/0003_claimofficer.py` & `openimis-be-claim-1.5.1/claim/migrations/0003_claimofficer.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/claim/migrations/0004_claimattachment.py` & `openimis-be-claim-1.5.1/claim/migrations/0004_claimattachment.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/claim/migrations/0005_claimmutation.py` & `openimis-be-claim-1.5.1/claim/migrations/0005_claimmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/claim/migrations/0009_auto_20200421_1657.py` & `openimis-be-claim-1.5.1/claim/migrations/0009_auto_20200421_1657.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/claim/migrations/0010_auto_20200611_0601.py` & `openimis-be-claim-1.5.1/claim/migrations/0010_auto_20200611_0601.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/claim/migrations/0012_item_service_jsonExtField.py` & `openimis-be-claim-1.5.1/claim/migrations/0012_item_service_jsonExtField.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/claim/models.py` & `openimis-be-claim-1.5.1/claim/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,21 +9,25 @@
 from graphql import ResolveInfo
 from insuree import models as insuree_models
 from location import models as location_models
 from location.models import UserDistrict
 from medical import models as medical_models
 from policy import models as policy_models
 from product import models as product_models
+from django.apps import apps
+
+core_config = apps.get_app_config('core')
 
 
 class ClaimAdmin(core_models.VersionedModel):
     id = models.AutoField(db_column='ClaimAdminId', primary_key=True)
     uuid = models.CharField(db_column='ClaimAdminUUID', max_length=36, default=uuid.uuid4, unique=True)
 
-    code = models.CharField(db_column='ClaimAdminCode', max_length=8, blank=True, null=True)
+    code = models.CharField(db_column='ClaimAdminCode', max_length=core_config.user_username_and_code_length_limit,
+                            blank=True, null=True)
     last_name = models.CharField(db_column='LastName', max_length=100, blank=True, null=True)
     other_names = models.CharField(db_column='OtherNames', max_length=100, blank=True, null=True)
     dob = models.DateField(db_column='DOB', blank=True, null=True)
     email_id = models.CharField(db_column='EmailId', max_length=200, blank=True, null=True)
     phone = models.CharField(db_column='Phone', max_length=50, blank=True, null=True)
     health_facility = models.ForeignKey(
         location_models.HealthFacility, models.DO_NOTHING, db_column='HFId', blank=True, null=True)
@@ -71,16 +75,32 @@
 
     def set_password(self, raw_password):
         raise NotImplementedError("Shouldn't set a password on an Officer")
 
     def check_password(self, raw_password):
         return False
 
+    @property
+    def officer_allowed_locations(self):
+        """
+        Returns uuid of all locations allowed for given officer
+        """
+        district = self.health_facility.location
+        all_allowed_uuids = [district.parent.uuid, district.uuid]
+        child_locations = location_models.Location.objects.filter(parent=district).values_list('uuid', flat=True)
+        while child_locations:
+            all_allowed_uuids.extend(child_locations)
+            child_locations = location_models.Location.objects\
+                .filter(parent__uuid__in=child_locations)\
+                .values_list('uuid', flat=True)
+
+        return location_models.Location.objects.filter(uuid__in=all_allowed_uuids)
+
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblClaimAdmin'
 
 
 class Feedback(core_models.VersionedModel):
     id = models.AutoField(db_column='FeedbackID', primary_key=True)
     uuid = models.CharField(db_column='FeedbackUUID', max_length=36, default=uuid.uuid4, unique=True)
     claim = models.OneToOneField(
@@ -92,15 +112,15 @@
     asessment = models.SmallIntegerField(db_column='Asessment', blank=True, null=True)
     # No FK in database (so value may not be an existing officer.id !)
     officer_id = models.IntegerField(db_column='CHFOfficerCode', blank=True, null=True)
     feedback_date = fields.DateTimeField(db_column='FeedbackDate', blank=True, null=True)
     audit_user_id = models.IntegerField(db_column='AuditUserID')
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblFeedback'
 
     @classmethod
     def get_queryset(cls, queryset, user):
         queryset = cls.filter_queryset(queryset)
         # GraphQL calls with an info object while Rest calls with the user itself
         if isinstance(user, ResolveInfo):
@@ -111,14 +131,47 @@
             dist = UserDistrict.get_user_districts(user._u)
             return queryset.filter(
                 claim__health_facility__location_id__in=[l.location_id for l in dist]
             )
         return queryset
 
 
+class FeedbackPrompt(core_models.VersionedModel):
+    id = models.AutoField(db_column='FeedbackPromptID', primary_key=True)
+    feedback_prompt_date = fields.DateField(db_column='FeedbackPromptDate', blank=True, null=True)
+    claim_id = models.OneToOneField(
+        "Claim", models.DO_NOTHING, db_column='ClaimID', blank=True, null=True, related_name="+")
+    officer_id = models.IntegerField(db_column='OfficerID', blank=True, null=True)
+    phone_number = models.CharField(db_column='PhoneNumber', max_length=36, unique=True)
+    sms_status = models.IntegerField(db_column='SMSStatus', blank=True, null=True)
+    validity_from = fields.DateTimeField(db_column='ValidityFrom', blank=True, null=True)
+    validity_to = fields.DateTimeField(db_column='ValidityTo', blank=True, null=True)
+    legacy_id = models.IntegerField(db_column='LegacyID', blank=True, null=True)
+    audit_user_id = models.IntegerField(db_column='AuditUserID', blank=True, null=True)
+
+    class Meta:
+        managed = True
+        db_table = 'tblFeedbackPrompt'
+
+    @classmethod
+    def get_queryset(cls, queryset, user):
+        queryset = cls.filter_queryset(queryset)
+        # GraphQL calls with an info object while Rest calls with the user itself
+        if isinstance(user, ResolveInfo):
+            user = user.context.user
+        if settings.ROW_SECURITY and user.is_anonymous:
+            return queryset.filter(id=-1)
+        if settings.ROW_SECURITY:
+            dist = UserDistrict.get_user_districts(user._u)
+            return queryset.filter(
+                claim__health_facility__location_id__in=[l.location_id for l in dist]
+            )
+        return queryset
+
+
 signal_claim_rejection = dispatch.Signal(providing_args=["claim"])
 
 
 class Claim(core_models.VersionedModel, core_models.ExtendableModel):
     id = models.AutoField(db_column='ClaimID', primary_key=True)
     uuid = models.CharField(db_column='ClaimUUID',
                             max_length=36, default=uuid.uuid4, unique=True)
@@ -216,15 +269,15 @@
         db_column='AuditUserIDSubmit', blank=True, null=True)
     audit_user_id_process = models.IntegerField(
         db_column='AuditUserIDProcess', blank=True, null=True)
 
     # row_id = models.BinaryField(db_column='RowID', blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblClaim'
 
     STATUS_REJECTED = 1
     STATUS_ENTERED = 2
     STATUS_CHECKED = 4
     STATUS_PROCESSED = 8
     STATUS_VALUATED = 16
@@ -288,15 +341,15 @@
 
 
 class ClaimAttachmentsCount(models.Model):
     claim = models.OneToOneField(Claim, primary_key=True, related_name='attachments_count', on_delete=models.DO_NOTHING)
     value = models.IntegerField(db_column='attachments_count')
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'claim_ClaimAttachmentsCountView'
 
 
 class ClaimMutation(core_models.UUIDModel):
     claim = models.ForeignKey(Claim, models.DO_NOTHING,
                               related_name='mutations')
     mutation = models.ForeignKey(
@@ -389,15 +442,15 @@
     price_origin = models.CharField(
         db_column='PriceOrigin', max_length=1, blank=True, null=True)
     exceed_ceiling_amount_category = models.DecimalField(
         db_column='ExceedCeilingAmountCategory', max_digits=18, decimal_places=2, blank=True, null=True)
     objects = ClaimDetailManager()
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblClaimItems'
 
 
 class ClaimAttachment(core_models.UUIDModel, core_models.UUIDVersionedModel):
     claim = models.ForeignKey(
         Claim, models.DO_NOTHING, related_name='attachments')
     type = models.TextField(blank=True, null=True)
@@ -468,15 +521,15 @@
         db_column='PriceOrigin', max_length=1, blank=True, null=True)
     exceed_ceiling_amount_category = models.DecimalField(
         db_column='ExceedCeilingAmountCategory', max_digits=18, decimal_places=2, blank=True, null=True)
 
     objects = ClaimDetailManager()
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblClaimServices'
 
 
 class ClaimDedRem(core_models.VersionedModel):
     id = models.AutoField(db_column='ExpenditureID', primary_key=True)
 
     policy = models.ForeignKey('policy.Policy', models.DO_NOTHING, db_column='PolicyID', blank=True, null=True,
@@ -498,9 +551,9 @@
                                               blank=True, null=True)
     rem_antenatal = models.DecimalField(db_column='RemAntenatal', max_digits=18, decimal_places=2,
                                         blank=True, null=True)
 
     audit_user_id = models.IntegerField(db_column='AuditUserID')
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblClaimDedRem'
```

### Comparing `openimis-be-claim-1.5.0/claim/reports/claim.py` & `openimis-be-claim-1.5.1/claim/reports/claim.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/claim/schema.py` & `openimis-be-claim-1.5.1/claim/schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from core.models import Officer
+from location.models import HealthFacility
+from .services import check_unique_claim_code
 import django
 from core.schema import signal_mutation_module_validate
 from django.db.models import OuterRef, Subquery, Avg, Q
 import graphene_django_optimizer as gql_optimizer
 from core.schema import OrderedDjangoFilterConnectionField, OfficerGQLType
 from core import filter_validity
 from django.db.models.functions import Cast
 
 from .models import ClaimMutation
 from django.utils.translation import gettext as _
 from graphene_django.filter import DjangoFilterConnectionField
+import ast
 
 # We do need all queries and mutations in the namespace here.
 from .gql_queries import *  # lgtm [py/polluting-import]
 from .gql_mutations import *  # lgtm [py/polluting-import]
 
 
 class Query(graphene.ObjectType):
@@ -23,24 +26,43 @@
         code_is_not=graphene.String(),
         orderBy=graphene.List(of_type=graphene.String),
         items=graphene.List(of_type=graphene.String),
         services=graphene.List(of_type=graphene.String),
         json_ext=graphene.JSONString(),
     )
 
-    claim = graphene.Field(ClaimGQLType, id=graphene.Int(), uuid=graphene.UUID())
+    claim = graphene.Field(
+        ClaimGQLType, id=graphene.Int(), uuid=graphene.UUID()
+    )
 
-    claim_attachments = DjangoFilterConnectionField(ClaimAttachmentGQLType)
+    claim_attachments = DjangoFilterConnectionField(
+        ClaimAttachmentGQLType
+    )
     claim_admins = DjangoFilterConnectionField(
-        ClaimAdminGQLType, search=graphene.String()
+        ClaimAdminGQLType,
+        search=graphene.String(),
+        region_uuid=graphene.String(),
+        district_uuid=graphene.String()
     )
     claim_officers = DjangoFilterConnectionField(
         OfficerGQLType, search=graphene.String()
     )
 
+    validate_claim_code = graphene.Field(
+        graphene.Boolean,
+        claim_code=graphene.String(required=True),
+        description="Checks that the specified claim code is unique."
+    )
+
+    def resolve_validate_claim_code(self, info, **kwargs):
+        if not info.context.user.has_perms(ClaimConfig.gql_query_claims_perms):
+            raise PermissionDenied(_("unauthorized"))
+        errors = check_unique_claim_code(code=kwargs['claim_code'])
+        return False if errors else True
+
     def resolve_claim(self, info, id=None, uuid=None, **kwargs):
         if (
             not info.context.user.has_perms(ClaimConfig.gql_query_claims_perms)
             and settings.ROW_SECURITY
         ):
             raise PermissionDenied(_("unauthorized"))
 
@@ -83,40 +105,71 @@
                 Claim.objects.filter(*filter_validity(**kwargs))
                 .filter(date_claimed__gt=last_year)
                 .values("icd__code")
                 .filter(icd__code=OuterRef("icd__code"))
                 .annotate(diag_avg=Avg("approved"))
                 .values("diag_avg")
             )
-            variance_filter = Q(claimed__gt=(1 + variance / 100) * Subquery(diag_avg))
+            variance_filter = Q(claimed__gt=(
+                1 + variance / 100) * Subquery(diag_avg))
             if not ClaimConfig.gql_query_claim_diagnosis_variance_only_on_existing:
                 diags = (
                     Claim.objects.filter(*filter_validity(**kwargs))
                     .filter(date_claimed__gt=last_year)
                     .values("icd__code")
                     .distinct()
                 )
                 variance_filter = variance_filter | ~Q(icd__code__in=diags)
             query = query.filter(variance_filter)
+
+        from location.models import Location
+        user_districts = UserDistrict.get_user_districts(info.context.user._u)
+        query = query.filter(
+            Q(health_facility__location__in=Location.objects.filter(uuid__in=user_districts.values_list('location__uuid', flat=True))) | Q(
+                health_facility__location__in=Location.objects.filter(uuid__in=user_districts.values_list('location__parent__uuid', flat=True))))
+
         return gql_optimizer.query(query.all(), info)
 
     def resolve_claim_attachments(self, info, **kwargs):
         if not info.context.user.has_perms(ClaimConfig.gql_query_claims_perms):
             raise PermissionDenied(_("unauthorized"))
 
-    def resolve_claim_admins(self, info, search=None, **kwargs):
-        if not info.context.user.has_perms(ClaimConfig.gql_query_claim_admins_perms):
+    def resolve_claim_admins(
+            self,
+            info,
+            search=None,
+            **kwargs
+    ):
+        if not info.context.user.has_perms(
+                ClaimConfig.gql_query_claim_admins_perms
+        ):
             raise PermissionDenied(_("unauthorized"))
 
-        if search is not None:
-            return ClaimAdmin.objects.filter(
-                Q(code__icontains=search)
-                | Q(last_name__icontains=search)
-                | Q(other_names__icontains=search)
-            )
+        hf_filters = [*filter_validity(**kwargs)]
+        district_uuid = kwargs.get('district_uuid', None)
+        region_uuid = kwargs.get('region_uuid', None)
+        if district_uuid is not None:
+            hf_filters += [Q(location__uuid=district_uuid)]
+        if region_uuid is not None:
+            hf_filters += [Q(location__parent__uuid=region_uuid)]
+        if settings.ROW_SECURITY:
+            dist = UserDistrict.get_user_districts(info.context.user._u)
+            hf_filters += [Q(location__id__in=[l.location_id for l in dist])]
+        user_health_facility = HealthFacility.objects.filter(*hf_filters)
+
+        filters = [*filter_validity(**kwargs)]
+        if user_health_facility:
+            filters += [Q(health_facility__in=user_health_facility)]
+
+        if search:
+            filters += filters[Q(code__icontains=search) |
+                               Q(last_name__icontains=search) |
+                               Q(other_names__icontains=search)]
+
+        return ClaimAdmin.objects.filter(*filters)
 
     def resolve_claim_officers(self, info, search=None, **kwargs):
         if not info.context.user.has_perms(ClaimConfig.gql_query_claim_officers_perms):
             raise PermissionDenied(_("unauthorized"))
 
         qs = Officer.objects
 
@@ -154,13 +207,14 @@
     if not uuids:
         uuid = kwargs["data"].get("claim_uuid", None)
         uuids = [uuid] if uuid else []
     if not uuids:
         return []
     impacted_claims = Claim.objects.filter(uuid__in=uuids).all()
     for claim in impacted_claims:
-        ClaimMutation.objects.create(claim=claim, mutation_id=kwargs["mutation_log_id"])
+        ClaimMutation.objects.create(
+            claim=claim, mutation_id=kwargs["mutation_log_id"])
     return []
 
 
 def bind_signals():
     signal_mutation_module_validate["claim"].connect(on_claim_mutation)
```

### Comparing `openimis-be-claim-1.5.0/claim/services.py` & `openimis-be-claim-1.5.1/claim/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,7 +369,13 @@
         return claim
 
     def __process_items(self, claim, items, services):
         claimed = 0
         claimed += process_items_relations(self.user, claim, items)
         claimed += process_services_relations(self.user, claim, services)
         claim.claimed = claimed
+
+
+def check_unique_claim_code(code):
+    if Claim.objects.filter(code=code, validity_to__isnull=True).exists():
+        return [{"message": "Claim code %s already exists" % code}]
+    return []
```

### Comparing `openimis-be-claim-1.5.0/claim/test_helpers.py` & `openimis-be-claim-1.5.1/claim/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/claim/test_services.py` & `openimis-be-claim-1.5.1/claim/test_services.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/claim/test_validations.py` & `openimis-be-claim-1.5.1/claim/test_validations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/claim/utils.py` & `openimis-be-claim-1.5.1/claim/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim-1.5.0/claim/validations.py` & `openimis-be-claim-1.5.1/claim/validations.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,30 +46,31 @@
     :param check_max: max amount to validate. Everything above will be rejected
     :return: (result_code, error_details)
     """
     logger.debug(f"Validating claim {claim.uuid}")
     if ClaimConfig.default_validations_disabled:
         return []
     errors = []
+    detail_errors = []
     errors += validate_target_date(claim)
     if len(errors) == 0:
         errors += validate_family(claim, claim.insuree)
     if len(errors) == 0:
-        validate_claimitems(claim)
-        validate_claimservices(claim)
+        detail_errors += validate_claimitems(claim)
+        detail_errors += validate_claimservices(claim)
 
     if check_max:
         # we went over the maximum for a category, all items and services in the claim are rejected
         over_category_errors = [
-            x for x in errors if x['code'] in [REJECTION_REASON_MAX_HOSPITAL_ADMISSIONS,
-                                               REJECTION_REASON_MAX_VISITS,
-                                               REJECTION_REASON_MAX_CONSULTATIONS,
-                                               REJECTION_REASON_MAX_SURGERIES,
-                                               REJECTION_REASON_MAX_DELIVERIES,
-                                               REJECTION_REASON_MAX_ANTENATAL]]
+            x for x in detail_errors if x['code'] in [REJECTION_REASON_MAX_HOSPITAL_ADMISSIONS,
+                                                      REJECTION_REASON_MAX_VISITS,
+                                                      REJECTION_REASON_MAX_CONSULTATIONS,
+                                                      REJECTION_REASON_MAX_SURGERIES,
+                                                      REJECTION_REASON_MAX_DELIVERIES,
+                                                      REJECTION_REASON_MAX_ANTENATAL]]
         if len(over_category_errors) > 0:
             rtn_items_rejected = claim.items.filter(validity_to__isnull=True) \
                 .update(status=ClaimItem.STATUS_REJECTED,
                         qty_approved=0,
                         rejection_reason=over_category_errors[0]['code'])
             rtn_services_rejected = claim.services.filter(validity_to__isnull=True) \
                 .update(status=ClaimService.STATUS_REJECTED,
@@ -101,142 +102,192 @@
         claim.rejection_reason = REJECTION_REASON_INVALID_ITEM_OR_SERVICE
         claim.save()
     logger.debug(f"Validation found {len(errors)} error(s)")
     return errors
 
 
 def validate_claimitems(claim):
+    errors = []
     target_date = claim.date_from if claim.date_from else claim.date_to
     for claimitem in claim.items \
             .filter(validity_to__isnull=True) \
             .filter(Q(rejection_reason=0) | Q(rejection_reason__isnull=True)):
-        validate_claimitem_validity(claimitem)
+        errors += validate_claimitem_validity(claim, claimitem)
         if not claimitem.rejection_reason:
-            validate_claimitem_in_price_list(claim, claimitem)
+            errors += validate_claimitem_in_price_list(claim, claimitem)
         if not claimitem.rejection_reason:
-            validate_claimdetail_care_type(claim, claimitem)
+            errors += validate_claimdetail_care_type(claim, claimitem)
         if not claimitem.rejection_reason:
-            validate_claimdetail_limitation_fail(claim, claimitem)
+            errors += validate_claimdetail_limitation_fail(claim, claimitem)
         if not claimitem.rejection_reason:
-            validate_claimitem_frequency(claim, claimitem)
+            errors += validate_claimitem_frequency(claim, claimitem)
         if not claimitem.rejection_reason:
-            validate_item_product_family(
+            errors += validate_item_product_family(
                 claimitem=claimitem,
                 target_date=target_date,
                 item=claimitem.item,
                 insuree_id=claim.insuree_id,
                 adult=claim.insuree.is_adult(target_date)
             )
         if claimitem.rejection_reason:
             claimitem.status = ClaimItem.STATUS_REJECTED
         else:
             claimitem.rejection_reason = 0
             claimitem.status = ClaimItem.STATUS_PASSED
         claimitem.save()
+    return errors
 
 
 def validate_claimservices(claim):
+    errors = []
     target_date = claim.date_from if claim.date_from else claim.date_to
     base_category = get_claim_category(claim)
 
     for claimservice in claim.services \
             .filter(validity_to__isnull=True) \
             .filter(Q(rejection_reason=0) | Q(rejection_reason__isnull=True)):
-        validate_claimservice_validity(claimservice)
+        errors += validate_claimservice_validity(claim, claimservice)
         if not claimservice.rejection_reason:
-            validate_claimservice_in_price_list(claim, claimservice)
+            errors += validate_claimservice_in_price_list(claim, claimservice)
         if not claimservice.rejection_reason:
-            validate_claimdetail_care_type(claim, claimservice)
+            errors += validate_claimdetail_care_type(claim, claimservice)
         if not claimservice.rejection_reason:
-            validate_claimservice_frequency(claim, claimservice)
+            errors += validate_claimservice_frequency(claim, claimservice)
         if not claimservice.rejection_reason:
-            validate_claimdetail_limitation_fail(claim, claimservice)
+            errors += validate_claimdetail_limitation_fail(claim, claimservice)
         if not claimservice.rejection_reason:
-            validate_service_product_family(
+            errors += validate_service_product_family(
                 claimservice=claimservice,
                 target_date=target_date,
                 service=claimservice.service,
                 insuree_id=claim.insuree_id,
                 adult=claim.insuree.is_adult(target_date),
                 base_category=base_category,
+                claim=claim,
             )
         if claimservice.rejection_reason:
             claimservice.status = ClaimService.STATUS_REJECTED
         else:
             claimservice.rejection_reason = 0
             claimservice.status = ClaimService.STATUS_PASSED
         claimservice.save()
+    return errors
 
 
-def validate_claimitem_validity(claimitem):
+def validate_claimitem_validity(claim, claimitem):
     # In the stored procedure, this check used a complex query to get the latest item but the latest item seems to
     # always be updated.
     # select *
     # from tblClaimItems tCI inner join tblItems tI on tCI.ItemID = tI.ItemID
     # where ti.ValidityTo is not null and tI.LegacyID is not null;
     # gives no result, so no claimitem is pointing to an old item and the complex query always fetched the last one.
     # Here, claimitem.item.legacy_id is always None
+    errors = []
     if claimitem.validity_to is None and claimitem.item.validity_to is not None:
         claimitem.rejection_reason = REJECTION_REASON_INVALID_ITEM_OR_SERVICE
+        errors += [{'code': REJECTION_REASON_INVALID_ITEM_OR_SERVICE,
+                    'message': _("claim.validation.claimitem_validity") % {
+                        'code': claim.code
+                    },
+                    'detail': claim.uuid}]
+    return errors
 
 
-def validate_claimservice_validity(claimservice):
+def validate_claimservice_validity(claim, claimservice):
     # See note in validate_claimitem_validity
+    errors = []
     if claimservice.validity_to is None and claimservice.service.validity_to is not None:
         claimservice.rejection_reason = REJECTION_REASON_INVALID_ITEM_OR_SERVICE
+        errors += [{'code': REJECTION_REASON_INVALID_ITEM_OR_SERVICE,
+                    'message': _("claim.validation.claimservice_validity") % {
+                        'code': claim.code
+                    },
+                    'detail': claim.uuid}]
+    return errors
 
 
 def validate_claimitem_in_price_list(claim, claimitem):
+    errors = []
     pricelist_detail = ItemsPricelistDetail.objects \
         .filter(item_id=claimitem.item_id,
                 validity_to__isnull=True,
                 items_pricelist=claim.health_facility.items_pricelist,
                 items_pricelist__validity_to__isnull=True
                 ) \
         .first()
     if not pricelist_detail:
         claimitem.rejection_reason = REJECTION_REASON_NOT_IN_PRICE_LIST
+        errors += [{'code': REJECTION_REASON_NOT_IN_PRICE_LIST,
+                    'message': _("claim.validation.claimitem_in_price_list_validity") % {
+                        'code': claim.code
+                    },
+                    'detail': claim.uuid}]
+    return errors
 
 
 def validate_claimservice_in_price_list(claim, claimservice):
+    errors = []
     pricelist_detail = ServicesPricelistDetail.objects \
         .filter(service_id=claimservice.service_id,
                 validity_to__isnull=True,
                 services_pricelist=claim.health_facility.services_pricelist,
                 services_pricelist__validity_to__isnull=True
                 ) \
         .first()
     if not pricelist_detail:
         claimservice.rejection_reason = REJECTION_REASON_NOT_IN_PRICE_LIST
+        errors += [{'code': REJECTION_REASON_NOT_IN_PRICE_LIST,
+                    'message': _("claim.validation.claimservice_in_price_list_validity") % {
+                        'code': claim.code
+                    },
+                    'detail': claim.uuid}]
+    return errors
 
 
 def validate_claimdetail_care_type(claim, claimdetail):
+    errors = []
     care_type = claimdetail.itemsvc.care_type
     hf_care_type = claim.health_facility.care_type if claim.health_facility.care_type else 'B'
     target_date = claim.date_to if claim.date_to else claim.date_from
 
     if (
             care_type == 'I' and (
             hf_care_type == 'O'
             or target_date == claim.date_from)
     ) or (
             care_type == 'O' and (
             hf_care_type == 'I'
             or target_date != claim.date_from)
     ):
         claimdetail.rejection_reason = REJECTION_REASON_CARE_TYPE
+        errors += [{'code': REJECTION_REASON_CARE_TYPE,
+                    'message': _("claim.validation.claimdetail_care_type_validity") % {
+                        'code': claim.code
+                    },
+                    'detail': claim.uuid}]
+    return errors
 
 
 def validate_claimdetail_limitation_fail(claim, claimdetail):
+    # if the mask is empty, it should be valid for everyone
+    if claimdetail.itemsvc.patient_category == 0:
+        return []
+    errors = []
     target_date = claim.date_to if claim.date_to else claim.date_from
     patient_category_mask = utils.patient_category_mask(
         claim.insuree, target_date)
-
+    
     if claimdetail.itemsvc.patient_category & patient_category_mask != patient_category_mask:
         claimdetail.rejection_reason = REJECTION_REASON_CATEGORY_LIMITATION
+        errors += [{'code': REJECTION_REASON_CATEGORY_LIMITATION,
+                    'message': _("claim.validation.claimdetail_limitation_validity") % {
+                        'code': claim.code
+                    },
+                    'detail': claim.uuid}]
+    return errors
 
 
 def frequency_check(qs, claim, elt):
     td = claim.date_from if not claim.date_to else claim.date_to
     delta = datetimedelta(days=elt.frequency)
     return qs \
         .annotate(target_date=Coalesce("claim__date_to", "claim__date_from")) \
@@ -249,23 +300,37 @@
                 ) \
         .exclude(claim__uuid=claim.uuid) \
         .order_by('-claim__date_from') \
         .exists()
 
 
 def validate_claimitem_frequency(claim, claimitem):
+    errors = []
     if claimitem.item.frequency and \
             frequency_check(ClaimItem.objects.filter(item=claimitem.item), claim, claimitem.item):
         claimitem.rejection_reason = REJECTION_REASON_FREQUENCY_FAILURE
+        errors += [{'code': REJECTION_REASON_FREQUENCY_FAILURE,
+                    'message': _("claim.validation.claimitem_frequency_validity") % {
+                        'code': claim.code
+                    },
+                    'detail': claim.uuid}]
+    return errors
 
 
 def validate_claimservice_frequency(claim, claimservice):
+    errors = []
     if claimservice.service.frequency and \
             frequency_check(ClaimService.objects.filter(service=claimservice.service), claim, claimservice.service):
         claimservice.rejection_reason = REJECTION_REASON_FREQUENCY_FAILURE
+        errors += [{'code': REJECTION_REASON_FREQUENCY_FAILURE,
+                    'message': _("claim.validation.claimservice_frequency_validity") % {
+                        'code': claim.code
+                    },
+                    'detail': claim.uuid}]
+    return errors
 
 
 def validate_target_date(claim):
     errors = []
     if (claim.date_from is None and claim.date_to is None) \
             or claim.date_claimed < claim.date_from:
         claim.reject(REJECTION_REASON_TARGET_DATE)
@@ -311,236 +376,195 @@
             found = True
             core = __import__("core")
             insuree_policy_effective_date = core.datetime.date.from_ad_date(
                 insuree_policy_effective_date)
             expiry_date = core.datetime.date.from_ad_date(expiry_date)
             product_item = ProductItem.objects.get(pk=product_item_id)
             # START CHECK 17 --> Item/Service waiting period violation (17)
-            waiting_period = None
-            if policy_stage == 'N' or policy_effective_date < insuree_policy_effective_date:
-                if adult:
-                    waiting_period = product_item.waiting_period_adult
-                else:
-                    waiting_period = product_item.waiting_period_child
-            if waiting_period and target_date < \
-                    (insuree_policy_effective_date.to_datetime() + datetimedelta(months=waiting_period)):
-                claimitem.rejection_reason = REJECTION_REASON_WAITING_PERIOD_FAIL
-                errors += [{'code': REJECTION_REASON_WAITING_PERIOD_FAIL,
-                            'message': _("claim.validation.product_family.waiting_period") % {
-                                'code': claimitem.claim.code,
-                                'element': str(item)},
-                            'detail': claimitem.claim.uuid}]
+            errors = check_service_item_waiting_period(policy_stage, policy_effective_date,
+                                                       insuree_policy_effective_date,
+                                                       item, adult, product_item, target_date, claimitem)
 
             # **** START CHECK 16 --> Item/Service Maximum provision (16)*****
-            if adult:
-                limit_no = product_item.limit_no_adult
-            else:
-                limit_no = product_item.limit_no_child
-            if limit_no is not None and limit_no >= 0:
-                # count qty provided
-                total_qty_provided = ClaimItem.objects \
-                    .annotate(target_date=Coalesce("claim__date_to", "claim__date_from")) \
-                    .filter(Q(rejection_reason=0) | Q(rejection_reason__isnull=True),
-                            validity_to__isnull=True,
-                            claim__insuree_id=insuree_id,
-                            item_id=item.id,
-                            target_date__gt=insuree_policy_effective_date,
-                            target_date__lte=expiry_date,
-                            claim__status__gt=Policy.STATUS_ACTIVE,
-                            claim__validity_to__isnull=True
-                            ) \
-                    .aggregate(Sum("qty_provided"))
-                qty = total_qty_provided["qty_provided__sum"] or 0
-                qty += claimitem.qty_provided if claimitem.qty_approved is None else claimitem.qty_approved
-                if qty > limit_no:
-                    claimitem.rejection_reason = REJECTION_REASON_QTY_OVER_LIMIT
-                    errors += [{'code': REJECTION_REASON_QTY_OVER_LIMIT,
-                                'message': _("claim.validation.product_family.max_nb_allowed") % {
-                                    'code': claimitem.claim.code,
-                                    'element': str(item),
-                                    'provided': total_qty_provided,
-                                    'max': limit_no},
-                                'detail': claimitem.claim.uuid}]
+            errors += check_service_item_max_provision(adult, product_item, item, insuree_policy_effective_date,
+                                                       expiry_date, insuree_id, claimitem)
         if not found:
             claimitem.rejection_reason = REJECTION_REASON_NO_PRODUCT_FOUND
             errors += [{'code': REJECTION_REASON_NO_PRODUCT_FOUND,
                         'message': _("claim.validation.product_family.no_product_found") % {
                             'code': claimitem.claim.code,
                             'element': str(item)},
                         'detail': claimitem.claim.uuid}]
 
     return errors
 
 
 # noinspection DuplicatedCode
-def validate_service_product_family(claimservice, target_date, service, insuree_id, adult, base_category):
+def validate_service_product_family(claimservice, target_date, service, insuree_id, adult, base_category, claim):
     errors = []
     found = False
     with get_products(target_date, service.id, insuree_id, adult, 'Service') as cursor:
         for (product_id, product_service_id, insuree_policy_effective_date, policy_effective_date, expiry_date,
              policy_stage) in cursor.fetchall():
             found = True
             core = __import__("core")
             insuree_policy_effective_date = core.datetime.date.from_ad_date(
                 insuree_policy_effective_date)
             expiry_date = core.datetime.date.from_ad_date(expiry_date)
             product_service = ProductService.objects.get(pk=product_service_id)
+
             # START CHECK 17 --> Item/Service waiting period violation (17)
-            waiting_period = None
-            if policy_stage == 'N' or policy_effective_date < insuree_policy_effective_date:
-                if adult:
-                    waiting_period = product_service.waiting_period_adult
-                else:
-                    waiting_period = product_service.waiting_period_child
-            if waiting_period and target_date < \
-                    (insuree_policy_effective_date.to_datetime() + datetimedelta(months=waiting_period)):
-                claimservice.rejection_reason = REJECTION_REASON_WAITING_PERIOD_FAIL
-                errors += [{'code': REJECTION_REASON_WAITING_PERIOD_FAIL,
-                            'message': _("claim.validation.product_family.waiting_period") % {
-                                'code': claimservice.claim.code,
-                                'element': str(service)},
-                            'detail': claimservice.claim.uuid}]
+            errors += check_service_item_waiting_period(policy_stage, policy_effective_date,
+                                                        insuree_policy_effective_date, service, adult,
+                                                        product_service, target_date, claimservice)
 
             # **** START CHECK 16 --> Item/Service Maximum provision (16)*****
-            if adult:
-                limit_no = product_service.limit_no_adult
-            else:
-                limit_no = product_service.limit_no_child
-            if limit_no is not None and limit_no >= 0:
-                # count qty provided
-                total_qty_provided = ClaimService.objects \
-                    .annotate(target_date=Coalesce("claim__date_to", "claim__date_from")) \
-                    .filter(Q(rejection_reason=0) | Q(rejection_reason__isnull=True),
-                            validity_to__isnull=True,
-                            service_id=service.id,
-                            target_date__gte=insuree_policy_effective_date,
-                            target_date__lte=expiry_date,
-                            claim__insuree_id=insuree_id,
-                            claim__status__gt=Policy.STATUS_ACTIVE,
-                            claim__validity_to__isnull=True
-                            ) \
-                    .aggregate(Sum("qty_provided"))
-                qty = total_qty_provided["qty_provided__sum"] or 0
-                qty += claimservice.qty_provided if claimservice.qty_approved is None else claimservice.qty_approved
-                if qty > limit_no:
-                    claimservice.rejection_reason = REJECTION_REASON_QTY_OVER_LIMIT
-                    errors += [{'code': REJECTION_REASON_QTY_OVER_LIMIT,
-                                'message': _("claim.validation.product_family.max_nb_allowed") % {
-                                    'code': claimservice.claim.code,
-                                    'element': str(service),
-                                    'provided': total_qty_provided,
-                                    'max': limit_no},
-                                'detail': claimservice.claim.uuid}]
+            errors += check_service_item_max_provision(adult, product_service, service, insuree_policy_effective_date,
+                                                       expiry_date, insuree_id, claimservice)
 
-            # The following checks (TODO: extract them from this method) use various limits from the product
             # Each violation is meant to interrupt the validation
+            error_len = len(errors)
             product = Product.objects.filter(pk=product_id).first()
-            # **** START CHECK 13 --> Maximum consultations (13)*****
-            if base_category == 'C':
-                if product.max_no_consultation is not None and product.max_no_consultation >= 0:
-                    count = get_claim_queryset_by_category(expiry_date, insuree_id, insuree_policy_effective_date, 'C') \
-                        .count()
-                    if count and count >= product.max_no_consultation:
-                        claimservice.rejection_reason = REJECTION_REASON_MAX_CONSULTATIONS
-                        errors += [{'message': _("claim.validation.product_family.max_nb_consultation") % {
-                            'code': claimservice.claim.code,
-                            'count': count,
-                            'max': product.max_no_consultation},
-                                    'detail': claimservice.claim.uuid}]
-                        break
-
-            # **** START CHECK 14 --> Maximum Surgeries (14)*****
-            if base_category == 'S':
-                if product.max_no_surgery is not None and product.max_no_surgery >= 0:
-                    count = get_claim_queryset_by_category(expiry_date, insuree_id, insuree_policy_effective_date, 'S') \
-                        .count()
-                    if count and count >= product.max_no_surgery:
-                        claimservice.rejection_reason = REJECTION_REASON_MAX_SURGERIES
-                        errors += [{'message': _("claim.validation.product_family.max_nb_surgeries") % {
-                            'code': claimservice.claim.code,
-                            'count': count,
-                            'max': product.max_no_surgery},
-                                    'detail': claimservice.claim.uuid}]
-                        break
-
-            # **** START CHECK 15 --> Maximum Deliveries (15)*****
-            if base_category == 'D':
-                if product.max_no_delivery is not None and product.max_no_delivery >= 0:
-                    count = get_claim_queryset_by_category(expiry_date, insuree_id, insuree_policy_effective_date, 'D') \
-                        .count()
-                    if count and count >= product.max_no_delivery:
-                        claimservice.rejection_reason = REJECTION_REASON_MAX_DELIVERIES
-                        errors += [{'message': _("claim.validation.product_family.max_nb_deliveries") % {
-                            'code': claimservice.claim.code,
-                            'count': count,
-                            'max': product.max_no_delivery},
-                                    'detail': claimservice.claim.uuid}]
-                        break
-
-            # **** START CHECK 19 --> Maximum Antenatal  (19)*****
-            if base_category == 'A':
-                if product.max_no_antenatal is not None and product.max_no_antenatal >= 0:
-                    count = get_claim_queryset_by_category(expiry_date, insuree_id, insuree_policy_effective_date, 'A') \
-                        .count()
-                    if count and count >= product.max_no_antenatal:
-                        claimservice.rejection_reason = REJECTION_REASON_MAX_ANTENATAL
-                        errors += [{'message': _("claim.validation.product_family.max_nb_antenatal") % {
-                            'code': claimservice.claim.code,
-                            'count': count,
-                            'max': product.max_no_antenatal},
-                                    'detail': claimservice.claim.uuid}]
-                        break
-
-            # **** START CHECK 11 --> Maximum Hospital admissions (11)*****
-            if base_category == 'H':
-                if product.max_no_hospitalization is not None and product.max_no_hospitalization >= 0:
-                    count = get_claim_queryset_by_category(expiry_date, insuree_id, insuree_policy_effective_date, 'H') \
-                        .count()
-                    if count and count >= product.max_no_hospitalization:
-                        claimservice.rejection_reason = REJECTION_REASON_MAX_HOSPITAL_ADMISSIONS
-                        errors += [{'message': _("claim.validation.product_family.max_nb_hospitalizations") % {
-                            'code': claimservice.claim.code,
-                            'count': count,
-                            'max': product.max_no_hospitalization},
-                                    'detail': claimservice.claim.uuid}]
-                        break
-
-            # **** START CHECK 12 --> Maximum Visits (OP) (12)*****
-            if base_category == 'V':
-                if product.max_no_visits is not None and product.max_no_visits >= 0:
-                    count = get_claim_queryset_by_category(expiry_date, insuree_id, insuree_policy_effective_date, 'V') \
-                        .count()
-                    if count and count >= product.max_no_visits:
-                        claimservice.rejection_reason = REJECTION_REASON_MAX_VISITS
-                        errors += [{'message': _("claim.validation.product_family.max_nb_visits") % {
-                            'code': claimservice.claim.code,
-                            'count': count,
-                            'max': product.max_no_visits},
-                                    'detail': claimservice.claim.uuid}]
-                        break
+            if base_category != 'O':
+                errors += check_claim_max_no_category(base_category, product, expiry_date, insuree_id,
+                                                      insuree_policy_effective_date, claim, claimservice)
+                if error_len != len(errors):
+                    break
 
         if not found:
             claimservice.rejection_reason = REJECTION_REASON_NO_PRODUCT_FOUND
             errors += [{'code': REJECTION_REASON_NO_PRODUCT_FOUND,
                         'message': _("claim.validation.product_family.no_product_found") % {
                             'code': claimservice.claim.code,
                             'element': str(service)},
                         'detail': claimservice.claim.uuid}]
 
     return errors
 
+def check_service_item_waiting_period(policy_stage, policy_effective_date, insuree_policy_effective_date, service_or_item,
+                                 adult, product_service_item, target_date, claim_service_item):
+    errors = []
+    waiting_period = None
+    if policy_stage == 'N' or policy_effective_date < insuree_policy_effective_date:
+        if adult:
+            waiting_period = product_service_item.waiting_period_adult
+        else:
+            waiting_period = product_service_item.waiting_period_child
+    if waiting_period and target_date < \
+            (insuree_policy_effective_date.to_datetime() + datetimedelta(months=waiting_period)):
+        claim_service_item.rejection_reason = REJECTION_REASON_WAITING_PERIOD_FAIL
+        errors += [{'code': REJECTION_REASON_WAITING_PERIOD_FAIL,
+                    'message': _("claim.validation.product_family.waiting_period") % {
+                        'code': claim_service_item.claim.code,
+                        'element': str(service_or_item)},
+                    'detail': claim_service_item.claim.uuid}]
+    return errors
+
+
+def check_service_item_max_provision(adult, product_service_item, service_or_item, insuree_policy_effective_date,
+                                     expiry_date, insuree_id, claim_service_item):
+    errors = []
+    if adult:
+        limit_no = product_service_item.limit_no_adult
+    else:
+        limit_no = product_service_item.limit_no_child
+    if limit_no is not None and limit_no >= 0:
+        # count qty provided
+        total_qty_provided = _get_total_qty_provided(claim_service_item, service_or_item, insuree_policy_effective_date,
+                                                     expiry_date, insuree_id)
+        qty = total_qty_provided + claim_service_item.qty_provided if claim_service_item.qty_approved is None \
+                                                                   else claim_service_item.qty_approved
+        if qty > limit_no:
+            # it would be good to add a warning msg, here is a related ticket: OTC-943
+            if total_qty_provided < limit_no:
+                remaining_qty = limit_no - total_qty_provided
+                if claim_service_item.qty_approved is None:
+                    claim_service_item.qty_provided = remaining_qty
+                else:
+                    claim_service_item.qty_approved = remaining_qty
+                claim_service_item.save()
+            else:
+                claim_service_item.rejection_reason = REJECTION_REASON_QTY_OVER_LIMIT
+                errors += [{'code': REJECTION_REASON_QTY_OVER_LIMIT,
+                            'message': _("claim.validation.product_family.max_nb_allowed") % {
+                                'code': claim_service_item.claim.code,
+                                'element': str(service_or_item),
+                                'provided': total_qty_provided,
+                                'max': limit_no},
+                            'detail': claim_service_item.claim.uuid}]
+
+    return errors
+
+
+def _get_total_qty_provided(claim_service_item, service_or_item, insuree_policy_effective_date,
+                            expiry_date, insuree_id):
+    return claim_service_item.__class__.objects \
+            .annotate(target_date=Coalesce("claim__date_to", "claim__date_from")) \
+            .filter(Q(rejection_reason=0) | Q(rejection_reason__isnull=True),
+                    validity_to__isnull=True,
+                    **{
+                        f"{'service' if isinstance(service_or_item, Service) else 'item'}_id": service_or_item.id},
+                    policy__validity_to__isnull=True,
+                    target_date__gte=insuree_policy_effective_date,
+                    target_date__lte=expiry_date,
+                    claim__insuree_id=insuree_id,
+                    claim__status__gt=Claim.STATUS_ENTERED,
+                    claim__validity_to__isnull=True
+                    ) \
+            .aggregate(total_qty_provided=Sum(Coalesce("qty_approved", "qty_provided"))) \
+            .get("total_qty_provided") or 0
 
-def get_claim_queryset_by_category(expiry_date, insuree_id, insuree_policy_effective_date, category):
+def check_claim_max_no_category(base_category, product, expiry_date, insuree_id,
+                                insuree_policy_effective_date, claim, claimservice):
+    errors = []
+    category_dict = {
+        'C': {'max': product.max_no_consultation,
+              "reason": REJECTION_REASON_MAX_CONSULTATIONS,
+              "message": "claim.validation.product_family.max_nb_consultation"},
+        'S': {"max": product.max_no_surgery,
+              "reason": REJECTION_REASON_MAX_SURGERIES,
+              "message": "claim.validation.product_family.max_nb_surgeries"},
+        'D': {"max": product.max_no_delivery,
+              "reason": REJECTION_REASON_MAX_DELIVERIES,
+              "message": "claim.validation.product_family.max_nb_deliveries"},
+        'A': {"max": product.max_no_antenatal,
+              "reason": REJECTION_REASON_MAX_ANTENATAL,
+              "message": "claim.validation.product_family.max_nb_antenatal"},
+        'H': {"max": product.max_no_hospitalization,
+              "reason": REJECTION_REASON_MAX_HOSPITAL_ADMISSIONS,
+              "message": "claim.validation.product_family.max_nb_hospitalizations"},
+        'V': {"max": product.max_no_visits,
+              "reason": REJECTION_REASON_MAX_VISITS,
+              "message": "claim.validation.product_family.max_nb_visits"},
+    }.get(base_category)
+
+    if category_dict['max'] is not None and category_dict['max'] >= 0:
+        count = get_claim_queryset_by_category(expiry_date, insuree_id, insuree_policy_effective_date, base_category, claim) \
+            .count()
+        if count and count >= category_dict['max']:
+            claimservice.rejection_reason = category_dict['reason']
+            errors += [{'code': category_dict['reason'],
+                        'message': _(category_dict['message']) % {
+                            'code': claimservice.claim.code,
+                            'count': count,
+                            'max': category_dict['max']},
+                        'detail': claimservice.claim.uuid}]
+    return errors
+
+
+def get_claim_queryset_by_category(expiry_date, insuree_id, insuree_policy_effective_date, category, claim=None):
     queryset = Claim.objects \
         .annotate(target_date=Coalesce("date_to", "date_from")) \
         .filter(insuree_id=insuree_id,
                 validity_to__isnull=True,
-                status__gt=2,
+                status__gt=Claim.STATUS_ENTERED,
                 target_date__gte=insuree_policy_effective_date,
                 target_date__lte=expiry_date)
+    if claim:
+        queryset = queryset.exclude(uuid=claim.uuid)
     if category == 'V':
         queryset = queryset.filter(
             Q(category=category) | Q(category__isnull=True))
     else:
         queryset = queryset.filter(category=category)
     return queryset
 
@@ -639,21 +663,24 @@
         Service.CATEGORY_DELIVERY,
         Service.CATEGORY_ANTENATAL,
         Service.CATEGORY_HOSPITALIZATION,
         Service.CATEGORY_CONSULTATION,
         Service.CATEGORY_OTHER,
         Service.CATEGORY_VISIT,
     ]
+    target_date = claim.date_to if claim.date_to else claim.date_from
     services = claim.services \
         .filter(validity_to__isnull=True, service__validity_to__isnull=True) \
         .values("service__category").distinct()
     claim_service_categories = [
         service["service__category"]
         for service in services
     ]
+    if claim.date_from != target_date:
+        claim_service_categories.append(Service.CATEGORY_HOSPITALIZATION)
     for category in service_categories:
         if category in claim_service_categories:
             claim_category = category
             break
     else:
         # One might expect "O" here but the legacy code uses "V"
         claim_category = Service.CATEGORY_VISIT
@@ -908,15 +935,15 @@
         product__isnull=False,
         product__validity_to__isnull=True
     ).values("policy_id", "product_id")
     services_query = claim.services.filter(
         Q(service__validity_to__isnull=True) | Q(service__validity_to__gte=target_date),
         validity_to__isnull=True,
         rejection_reason=0,
-        service__validity_from__lte=target_date,
+        service__validity_from__date__lte=target_date,
         product__isnull=False, product__validity_to__isnull=True
     ).values("policy_id", "product_id")
     if items_query.count() == 0 and services_query.count() == 0:
         logger.warning(f"claim {claim.uuid} did not have any item or service to valuate.")
     for policy_product in items_query.union(services_query, all=True):
         product = Product.objects.get(id=policy_product["product_id"])
         policy_members = InsureePolicy.objects.filter(
@@ -1003,15 +1030,15 @@
                     ceiling = max_ip
                     prev_remunerated = max_ip.prev
                 if product.max_ip_policy:
                     if policy_members > product.threshold:  # Threshold is NOT NULL
                         if product.max_policy_extra_member_ip:
                             ceiling = Deductible(
                                 product.max_ip_policy + (
-                                            policy_members - product.threshold) * product.max_policy_extra_member_ip,
+                                        policy_members - product.threshold) * product.max_policy_extra_member_ip,
                                 ceiling.type,
                                 ceiling.prev
                             )
                         if product.max_ceiling_policy_ip and ceiling.amount > product.max_ceiling_policy_ip:
                             ceiling = Deductible(
                                 product.max_ceiling_policy_ip,
                                 ceiling.type,
@@ -1029,15 +1056,15 @@
                     ceiling = max_op
                     prev_remunerated = max_op.prev
                 if product.max_op_policy:
                     if product.threshold and policy_members > product.threshold:
                         if product.max_policy_extra_member_op:
                             ceiling = Deductible(
                                 product.max_op_policy + (
-                                            policy_members - product.threshold) * product.max_policy_extra_member_op,
+                                        policy_members - product.threshold) * product.max_policy_extra_member_op,
                                 ceiling.type,
                                 ceiling.prev
                             )
                         if product.max_ceiling_policy_op and ceiling.amount > product.max_ceiling_policy_op:
                             ceiling = Deductible(
                                 product.max_ceiling_policy_op,
                                 ceiling.type,
@@ -1070,19 +1097,32 @@
             itemsvc_pricelist_detail = (ItemsPricelistDetail if detail_is_item else ServicesPricelistDetail).objects \
                 .filter(itemsvcs_pricelist=claim.health_facility.items_pricelist
             if detail_is_item else claim.health_facility.services_pricelist,
                         itemsvc=claim_detail.itemsvc,
                         itemsvcs_pricelist__validity_to__isnull=True,
                         validity_to__isnull=True) \
                 .first()
-            product_itemsvc = (ProductItem if detail_is_item else ProductService).objects \
-                .filter(product=claim_detail.product,
-                        itemsvc=claim_detail.itemsvc,
-                        validity_to__isnull=True) \
-                .first()
+            product_itemsvc = None
+
+            if detail_is_item:
+                product_itemsvc = ProductItem.objects.filter(
+                    product_id=claim_detail.product_id,
+                    item_id=claim_detail.item_id,
+                    validity_to__isnull=True
+                ).first()
+                if product_itemsvc is None:
+                    raise ValueError("Product Item not found")
+            else:
+                product_itemsvc = ProductService.objects.filter(
+                    product=claim_detail.product,
+                    service_id=claim_detail.service_id,
+                    validity_to__isnull=True
+                ).first()
+                if product_itemsvc is None:
+                    raise ValueError("Product Service not found")
 
             pl_price = itemsvc_pricelist_detail.price_overrule if itemsvc_pricelist_detail.price_overrule \
                 else claim_detail.itemsvc.price
 
             if claim_detail.price_approved is not None:
                 set_price_adjusted = claim_detail.price_approved
             else:
@@ -1182,15 +1222,15 @@
                         else:
                             exceed_ceiling_amount_category = work_value + prev_remunerated_consult \
                                                              + remunerated_consultation - product.max_amount_consultation
                             work_value -= exceed_ceiling_amount_category
                             remunerated_consultation += work_value
 
             # TODO big rework of this condition is needed. putting the ceiling_exclusion_? into a variable as first step
-            if (claim.insuree.is_adult
+            if (product_itemsvc is not None and claim.insuree.is_adult
                 and (
                         (
                                 product.ceiling_interpretation == Product.CEILING_INTERPRETATION_IN_PATIENT and hospitalization == 1)
                         or (
                                 product.ceiling_interpretation == Product.CEILING_INTERPRETATION_HOSPITAL and hf_level == "H")
                 )
                 and product_itemsvc.ceiling_exclusion_adult in ("B", "H")
@@ -1232,15 +1272,15 @@
                     if ceiling.amount - prev_remunerated - remunerated > 0:
                         if ceiling.amount - prev_remunerated - remunerated >= work_value:
                             exceed_ceiling_amount = 0
                             set_price_valuated = work_value
                             set_price_remunerated = work_value
                             remunerated += work_value
                         else:
-                            total = ceiling.amount + prev_remunerated + remunerated
+                            total = ceiling.amount - prev_remunerated - remunerated
                             exceed_ceiling_amount = work_value - total
                             set_price_valuated = total
                             set_price_remunerated = total
                             remunerated += total
                     else:
                         exceed_ceiling_amount = work_value
                         # remunerated += 0
```

### Comparing `openimis-be-claim-1.5.0/claim/views.py` & `openimis-be-claim-1.5.1/claim/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 import base64
 from django.conf import settings
 from django.core.exceptions import PermissionDenied
 from django.http import HttpResponse
+from rest_framework.decorators import api_view, permission_classes
+
 from report.services import ReportService
+from tools.views import checkUserWithRights
 from .services import ClaimReportService
 from .reports import claim
 from .apps import ClaimConfig
 from .models import ClaimAttachment
 from django.utils.translation import gettext as _
 import core
 
 
+@api_view(['GET'])
 def print(request):
     if not request.user.has_perms(ClaimConfig.claim_print_perms):
         raise PermissionDenied(_("unauthorized"))
     report_service = ReportService(request.user)
     report_data_service = ClaimReportService(request.user)
     data = report_data_service.fetch(request.GET['uuid'])
     return report_service.process('claim_claim', data, claim.template)
 
 
+@api_view(["GET", "POST"])
+@permission_classes(
+    [
+        checkUserWithRights(
+            ClaimConfig.gql_query_claims_perms,
+        )
+    ]
+)
 def attach(request):
     queryset = ClaimAttachment.objects.filter(*core.filter_validity())
     if settings.ROW_SECURITY:
         from location.models import UserDistrict
         dist = UserDistrict.get_user_districts(request.user._u)
         queryset = queryset.select_related("claim")\
             .filter(
             claim__health_facility__location__id__in=[
-                l.location_id for l in dist]
+                loc.location_id for loc in dist]
         )
     attachment = queryset\
         .filter(id=request.GET['id'])\
         .first()
     if not attachment:
         raise PermissionDenied(_("unauthorized"))
```

### Comparing `openimis-be-claim-1.5.0/openimis_be_claim.egg-info/PKG-INFO` & `openimis-be-claim-1.5.1/openimis_be_claim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-claim
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Claim reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-claim-1.5.0/openimis_be_claim.egg-info/SOURCES.txt` & `openimis-be-claim-1.5.1/openimis_be_claim.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -4,37 +4,48 @@
 setup.py
 claim/__init__.py
 claim/admin.py
 claim/apps.py
 claim/gql_mutations.py
 claim/gql_queries.py
 claim/models.py
+claim/report.py
 claim/schema.py
 claim/services.py
 claim/test_helpers.py
 claim/test_services.py
 claim/test_validations.py
 claim/tests.py
 claim/urls.py
 claim/utils.py
 claim/validations.py
 claim/views.py
+claim/management/__init__.py
+claim/management/commands/__init__.py
+claim/management/commands/generateclaimadmins.py
+claim/management/commands/generateclaims.py
 claim/migrations/0001_initial.py
 claim/migrations/0002_batchrun.py
 claim/migrations/0003_claimofficer.py
 claim/migrations/0004_claimattachment.py
 claim/migrations/0005_claimmutation.py
 claim/migrations/0006_claimattachment_url.py
 claim/migrations/0007_auto_20200318_1443.py
 claim/migrations/0008_create_claim_attachments_count_view.py
 claim/migrations/0009_auto_20200421_1657.py
 claim/migrations/0010_auto_20200611_0601.py
 claim/migrations/0011_auto_20201126_1244.py
 claim/migrations/0012_item_service_jsonExtField.py
+claim/migrations/0013_feedbackprompt.py
+claim/migrations/0014_change_code_limit.py
+claim/migrations/0015_prohibit_interaction_for_enrolment_officer.py
+claim/migrations/0016_update_django_scheme_with_missing_fields.py
+claim/migrations/0017_set_managed_to_true.py
 claim/migrations/__init__.py
 claim/reports/__init__.py
 claim/reports/claim.py
+claim/reports/claim_percentage_referrals.py
 openimis_be_claim.egg-info/PKG-INFO
 openimis_be_claim.egg-info/SOURCES.txt
 openimis_be_claim.egg-info/dependency_links.txt
 openimis_be_claim.egg-info/requires.txt
 openimis_be_claim.egg-info/top_level.txt
```

### Comparing `openimis-be-claim-1.5.0/setup.py` & `openimis-be-claim-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-claim',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Claim reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

