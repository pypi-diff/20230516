# Comparing `tmp/openimis-be-claim_batch-1.5.1.tar.gz` & `tmp/openimis-be-claim_batch-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-claim_batch-1.5.1.tar", last modified: Fri Nov 18 12:34:03 2022, max compression
+gzip compressed data, was "openimis-be-claim_batch-1.5.2.tar", last modified: Tue May 16 21:38:26 2023, max compression
```

## Comparing `openimis-be-claim_batch-1.5.1.tar` & `openimis-be-claim_batch-1.5.2.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 12:34:03.392156 openimis-be-claim_batch-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1852 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)       36 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      646 2022-11-18 12:34:03.392156 openimis-be-claim_batch-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2249 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 12:34:03.388156 openimis-be-claim_batch-1.5.1/claim_batch/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       29 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     1335 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 12:34:03.388156 openimis-be-claim_batch-1.5.1/claim_batch/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3497 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      459 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/migrations/0002_capitationpayment.py
--rw-r--r--   0 runner    (1001) docker     (122)     1172 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/migrations/0003_capitationpayment_for_legacy_batch_runs.py
--rw-r--r--   0 runner    (1001) docker     (122)      246 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/migrations/0004_delete_capitationpayment.py
--rw-r--r--   0 runner    (1001) docker     (122)      413 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/migrations/0005_capitationpayment.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8044 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 12:34:03.392156 openimis-be-claim_batch-1.5.1/claim_batch/reports/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   137336 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/reports/pbc_H.py
--rw-r--r--   0 runner    (1001) docker     (122)   136833 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/reports/pbc_P.py
--rw-r--r--   0 runner    (1001) docker     (122)    53878 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/reports/pbh.py
--rw-r--r--   0 runner    (1001) docker     (122)    53904 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/reports/pbp.py
--rw-r--r--   0 runner    (1001) docker     (122)     7417 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)    28217 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/services.py
--rw-r--r--   0 runner    (1001) docker     (122)      707 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6976 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)      117 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1945 2022-11-18 12:33:50.000000 openimis-be-claim_batch-1.5.1/claim_batch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-18 12:34:03.392156 openimis-be-claim_batch-1.5.1/openimis_be_claim_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      646 2022-11-18 12:34:03.000000 openimis-be-claim_batch-1.5.1/openimis_be_claim_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      941 2022-11-18 12:34:03.000000 openimis-be-claim_batch-1.5.1/openimis_be_claim_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-18 12:34:03.000000 openimis-be-claim_batch-1.5.1/openimis_be_claim_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      117 2022-11-18 12:34:03.000000 openimis-be-claim_batch-1.5.1/openimis_be_claim_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-18 12:34:03.000000 openimis-be-claim_batch-1.5.1/openimis_be_claim_batch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-18 12:34:03.392156 openimis-be-claim_batch-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1260 2022-11-18 12:34:00.000000 openimis-be-claim_batch-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:26.096966 openimis-be-claim_batch-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1852 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-05-16 21:38:26.096966 openimis-be-claim_batch-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2249 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:26.092966 openimis-be-claim_batch-1.5.2/claim_batch/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1335 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:26.096966 openimis-be-claim_batch-1.5.2/claim_batch/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/migrations/0002_capitationpayment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/migrations/0003_capitationpayment_for_legacy_batch_runs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/migrations/0004_delete_capitationpayment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/migrations/0005_capitationpayment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5735 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/migrations/0006_capitationpayment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1941 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/migrations/0007_update_django_scheme_with_missing_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/migrations/0008_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8041 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:26.096966 openimis-be-claim_batch-1.5.2/claim_batch/reports/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   137336 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/reports/pbc_H.py
+-rw-r--r--   0 runner    (1001) docker     (122)   136833 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/reports/pbc_P.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53878 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/reports/pbh.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53904 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/reports/pbp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7417 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30051 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/services.py
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6976 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-05-16 21:38:14.000000 openimis-be-claim_batch-1.5.2/claim_batch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:26.096966 openimis-be-claim_batch-1.5.2/openimis_be_claim_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-05-16 21:38:26.000000 openimis-be-claim_batch-1.5.2/openimis_be_claim_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-16 21:38:26.000000 openimis-be-claim_batch-1.5.2/openimis_be_claim_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 21:38:26.000000 openimis-be-claim_batch-1.5.2/openimis_be_claim_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-16 21:38:26.000000 openimis-be-claim_batch-1.5.2/openimis_be_claim_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-16 21:38:26.000000 openimis-be-claim_batch-1.5.2/openimis_be_claim_batch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 21:38:26.096966 openimis-be-claim_batch-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-05-16 21:38:25.000000 openimis-be-claim_batch-1.5.2/setup.py
```

### Comparing `openimis-be-claim_batch-1.5.1/LICENSE.md` & `openimis-be-claim_batch-1.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.5.1/PKG-INFO` & `openimis-be-claim_batch-1.5.2/openimis_be_claim_batch.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openimis-be-claim_batch
-Version: 1.5.1
+Name: openimis-be-claim-batch
+Version: 1.5.2
 Summary: The openIMIS Backend Claim Batch reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-claim_batch-1.5.1/README.md` & `openimis-be-claim_batch-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.5.1/claim_batch/apps.py` & `openimis-be-claim_batch-1.5.2/claim_batch/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.5.1/claim_batch/migrations/0001_initial.py` & `openimis-be-claim_batch-1.5.2/claim_batch/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.5.1/claim_batch/migrations/0003_capitationpayment_for_legacy_batch_runs.py` & `openimis-be-claim_batch-1.5.2/claim_batch/migrations/0003_capitationpayment_for_legacy_batch_runs.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.5.1/claim_batch/models.py` & `openimis-be-claim_batch-1.5.2/claim_batch/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         db_column='LocationId', blank=True, null=True)
     run_date = fields.DateTimeField(db_column='RunDate')
     audit_user_id = models.IntegerField(db_column='AuditUserID')
     run_year = models.IntegerField(db_column='RunYear')
     run_month = models.SmallIntegerField(db_column='RunMonth')
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblBatchRun'
 
 
 class RelativeIndex(core_models.VersionedModel):
     id = models.AutoField(db_column='RelIndexID', primary_key=True)
     product = models.ForeignKey(
         product_models.Product, models.DO_NOTHING, db_column='ProdID')
@@ -39,15 +39,15 @@
     audit_user_id = models.IntegerField(db_column='AuditUserID')
     location = models.ForeignKey(
         location_models.Location, models.DO_NOTHING, db_column='LocationId', blank=True, null=True,
         related_name="relative_indexes"
     )
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblRelIndex'
 
     CARE_TYPE_OUT_PATIENT = "O"
     CARE_TYPE_IN_PATIENT = "I"
     CARE_TYPE_BOTH = "B"
 
     TYPE_MONTH = 12
@@ -77,15 +77,15 @@
     validity_to = models.DateTimeField(
         db_column='ValidityTo', blank=True, null=True)
     legacy_id = models.IntegerField(
         db_column='LegacyID', blank=True, null=True)
     audit_user_id = models.IntegerField(db_column='AuditUserID')
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblRelDistr'
 
 
     CARE_TYPE_OUT_PATIENT = "O"
     CARE_TYPE_IN_PATIENT = "I"
     CARE_TYPE_BOTH = "B"
```

### Comparing `openimis-be-claim_batch-1.5.1/claim_batch/reports/pbc_H.py` & `openimis-be-claim_batch-1.5.2/claim_batch/reports/pbc_H.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.5.1/claim_batch/reports/pbc_P.py` & `openimis-be-claim_batch-1.5.2/claim_batch/reports/pbc_P.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.5.1/claim_batch/reports/pbh.py` & `openimis-be-claim_batch-1.5.2/claim_batch/reports/pbh.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.5.1/claim_batch/reports/pbp.py` & `openimis-be-claim_batch-1.5.2/claim_batch/reports/pbp.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.5.1/claim_batch/schema.py` & `openimis-be-claim_batch-1.5.2/claim_batch/schema.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.5.1/claim_batch/services.py` & `openimis-be-claim_batch-1.5.2/claim_batch/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import calendar
 import datetime
 import uuid
 import logging
 import pandas as pd
+from django.contrib.admin.options import get_content_type_for_model
+
 import core
 
 from datetime import date
 from django.db import connection, transaction
-from django.db.models import Value, F, Sum, Q, Prefetch, Count , Subquery, OuterRef, FloatField
+from django.db.models import Value, F, Sum, Q, Prefetch, Count, Subquery, OuterRef, FloatField
 from django.db.models.functions import Coalesce, ExtractMonth, ExtractYear
 from django.utils.translation import gettext as _
 
 from calculation.services import run_calculation_rules, get_calculation_object
 from claim.models import ClaimItem, Claim, ClaimService, ClaimDetail
 from claim_batch.models import BatchRun, RelativeIndex, RelativeDistribution
 from contribution.models import Premium
 from contribution_plan.models import PaymentPlan
 from core.signals import *
+from invoice.models import BillPayment, InvoicePayment, BillItem, InvoiceLineItem
 from location.models import HealthFacility, Location
 from product.models import Product, ProductItemOrService
 
 logger = logging.getLogger(__name__)
 
 
 @core.comparable
@@ -84,22 +87,22 @@
 
     @classmethod
     def capitation_report_data_for_summit(cls, submit):
         capitation_payment_products = []
         for svc_item in [ClaimItem, ClaimService]:
             capitation_payment_products.extend(
                 svc_item.objects
-                    .filter(claim__status=Claim.STATUS_VALUATED)
-                    .filter(claim__validity_to__isnull=True)
-                    .filter(validity_to__isnull=True)
-                    .filter(status=svc_item.STATUS_PASSED)
-                    .annotate(prod_location=Coalesce("product__location_id", Value(-1)))
-                    .filter(prod_location=submit.location_id if submit.location_id else -1)
-                    .values('product_id')
-                    .distinct()
+                .filter(claim__status=Claim.STATUS_VALUATED)
+                .filter(claim__validity_to__isnull=True)
+                .filter(validity_to__isnull=True)
+                .filter(status=svc_item.STATUS_PASSED)
+                .annotate(prod_location=Coalesce("product__location_id", Value(-1)))
+                .filter(prod_location=submit.location_id if submit.location_id else -1)
+                .values('product_id')
+                .distinct()
             )
 
         region_id, district_id = _get_capitation_region_and_district(submit.location_id)
         for product in set(map(lambda x: x['product_id'], capitation_payment_products)):
             params = {
                 'region_id': region_id,
                 'district_id': district_id,
@@ -116,15 +119,15 @@
     @classmethod
     def batch_run_already_executed(cls, year, month, location_id):
         return BatchRun.objects \
             .filter(run_year=year) \
             .filter(run_month=month) \
             .annotate(nn_location_id=Coalesce("location_id", Value(-1))) \
             .filter(nn_location_id=-1 if location_id is None else location_id) \
-            .filter(validity_to__isnull=True)\
+            .filter(validity_to__isnull=True) \
             .exists()
 
 
 @transaction.atomic
 def process_batch(audit_user_id, location_id, period, year):
     # declare table tblClaimsIDs
     if location_id == -1:
@@ -140,17 +143,17 @@
 
     if already_run_batch:
         return [str(ProcessBatchSubmitError(2))]
     _, days_in_month = calendar.monthrange(year, period)
     end_date = datetime.datetime(year, period, days_in_month)
     now = datetime.datetime.now()
     # TODO - double check this condition
-    #if end_date < now:
+    # if end_date < now:
     #    return [str(ProcessBatchSubmitError(3))]
-        ## TODO create message "Batch cannot be run before the end of the selected period"
+    ## TODO create message "Batch cannot be run before the end of the selected period"
     try:
         do_process_batch(audit_user_id, location_id, end_date)
     except (KeyboardInterrupt, SystemExit):
         raise
     except Exception as exc:
         logger.warning(
             f"Exception while processing batch user {audit_user_id}, location {location_id}, period {period}, year {year}",
@@ -220,16 +223,16 @@
             logger.debug("do_process_batch created run: %s", created_run.id)
     else:
         logger.info("no product found in  %s for %s/%s", location_id, period, year)
     return created_run
 
 
 def trigger_calculation_based_on_context(
-    context, work_data, end_date, product,
-    location_id, allocated_contribution, user_id
+        context, work_data, end_date, product,
+        location_id, allocated_contribution, user_id
 ):
     if work_data["payment_plans"]:
         for payment_plan in work_data["payment_plans"]:
             start_date = get_start_date(end_date, payment_plan.periodicity)
             # run only when it makes sense based on periodicitiy
             if start_date is not None:
                 allocated_contribution, work_data = update_work_data(
@@ -249,81 +252,117 @@
 def update_work_data(work_data, product, start_date, end_date, allocated_contribution=None):
     work_data["start_date"] = start_date
     # 1.3 generate queryset
     work_data["items"] = get_items_queryset(product, start_date, end_date)
     work_data["services"] = get_services_queryset(product, start_date, end_date)
     work_data["contributions"] = get_contribution_queryset(product, start_date, end_date)
     work_data['claims'] = get_claim_queryset(product, start_date, end_date)
+    work_data['bill_payments'] = get_bill_payment_queryset(product, start_date, end_date)
+    work_data['invoice_payments'] = get_invoice_payment_queryset(product, start_date, end_date)
     if allocated_contribution is None:
         allocated_contribution = {}
     start_date_str = str(start_date)
     if start_date_str not in allocated_contribution:
-        allocated_contribution[start_date_str] = get_allocated_premium(work_data["contributions"], start_date, end_date)
+        allocated_contribution[start_date_str] = get_allocated_premium(
+            get_allocated_contribution_queryset(product, start_date, end_date), start_date, end_date)
     work_data['allocated_contributions'] = allocated_contribution[start_date_str]
     return allocated_contribution, work_data
 
 
 def get_payment_plan_queryset(product, end_date):
-    return PaymentPlan.objects\
-        .filter(date_valid_to__gte=end_date)\
-        .filter(date_valid_from__lte=end_date)\
-        .filter(benefit_plan=product)\
+    return PaymentPlan.objects \
+        .filter(date_valid_to__gte=end_date) \
+        .filter(date_valid_from__lte=end_date) \
+        .filter(benefit_plan=product) \
         .filter(is_deleted=False)
 
 
 def get_items_queryset(product, start_date, end_date):
-    return ClaimItem.objects\
-        .filter(validity_to__isnull=True)\
-        .filter(claim__process_stamp__lte=end_date)\
-        .filter(claim__process_stamp__gte=start_date)\
-        .filter(product=product)\
-        .select_related('claim__health_facility')\
+    return ClaimItem.objects \
+        .filter(validity_to__isnull=True) \
+        .filter(claim__process_stamp__lte=end_date) \
+        .filter(claim__process_stamp__gte=start_date) \
+        .filter(product=product) \
+        .select_related('claim__health_facility') \
         .order_by('claim__health_facility').order_by('claim')
 
 
 def get_services_queryset(product, start_date, end_date):
-    return ClaimService.objects\
-        .filter(claim__process_stamp__lte=end_date)\
-        .filter(claim__process_stamp__gte=start_date)\
-        .filter(validity_to__isnull=True)\
-        .filter(product=product)\
-        .select_related('claim__health_facility')\
+    return ClaimService.objects \
+        .filter(claim__process_stamp__lte=end_date) \
+        .filter(claim__process_stamp__gte=start_date) \
+        .filter(validity_to__isnull=True) \
+        .filter(product=product) \
+        .select_related('claim__health_facility') \
         .order_by('claim__health_facility').order_by('claim')
 
 
 def get_claim_queryset(product, start_date, end_date):
-    return Claim.objects\
-        .filter(validity_from__lte=end_date)\
-        .filter(validity_from__gte=start_date)\
-        .filter(validity_to__isnull=True)\
-        .filter(process_stamp__lte=end_date)\
-        .filter((Q(items__product=product) | Q(services__product=product)))\
+    return Claim.objects \
+        .filter(validity_from__lte=end_date) \
+        .filter(validity_from__gte=start_date) \
+        .filter(validity_to__isnull=True) \
+        .filter(process_stamp__lte=end_date) \
+        .filter((Q(items__product=product) | Q(services__product=product))) \
         .distinct()
 
 
-def get_contribution_queryset(product, start_date, end_date):
+def get_allocated_contribution_queryset(product, start_date, end_date):
     return Premium.objects \
         .filter(policy__effective_date__lte=end_date) \
         .filter(policy__expiry_date__gte=start_date) \
-        .filter(validity_to__isnull=True)\
-        .filter(policy__product=product)\
+        .filter(validity_to__isnull=True) \
+        .filter(policy__product=product) \
         .select_related('policy')
 
 
 def get_product_queryset(end_date, location_id):
-    queryset = Product.objects\
-        .filter(validity_to__isnull=True)\
-        .filter(date_from__lte=end_date)\
+    queryset = Product.objects \
+        .filter(validity_to__isnull=True) \
+        .filter(date_from__lte=end_date) \
         .filter(Q(date_to__gte=end_date) | Q(date_to__isnull=True))
     if location_id is not None:
         return queryset.filter(location_id=location_id)
     else:
         return queryset.filter(location_id__isnull=True)
 
 
+def get_contribution_queryset(product, start_date, end_date):
+    return Premium.objects \
+        .filter(validity_to__isnull=True) \
+        .filter(created_date__range=(start_date, end_date)) \
+        .filter(policy__product=product)
+
+
+def get_bill_payment_queryset(product, start_date, end_date):
+    return BillPayment.objects \
+        .filter(is_deleted=False) \
+        .filter(date_created__range=(start_date, end_date)) \
+        .filter(bill__line_items_bill__in=BillItem.objects
+                .filter(is_deleted=False)
+                .filter(line_type=get_content_type_for_model(Premium))
+                .filter(line_id__in=Premium.objects
+                        .filter(validity_to__isnull=True)
+                        .filter(policy__product=product)
+                        .values_list('id', flat=True)))
+
+
+def get_invoice_payment_queryset(product, start_date, end_date):
+    return InvoicePayment.objects \
+        .filter(is_deleted=False) \
+        .filter(date_created__range=(start_date, end_date)) \
+        .filter(invoice__line_items__in=InvoiceLineItem.objects
+                .filter(is_deleted=False)
+                .filter(line_type=get_content_type_for_model(Premium))
+                .filter(line_id__in=Premium.objects
+                        .filter(validity_to__isnull=True)
+                        .filter(policy__product=product)
+                        .values_list('id', flat=True)))
+
+
 def get_allocated_premium(premiums, start_date, end_date):
     # Calculate allcated contributions
     # go trough the contribution and find the allocated contribution
     allocated_premiums = 0
     for premium in premiums:
         allocation_start = max(premium.policy.effective_date, start_date)
         if isinstance(allocation_start, datetime.datetime):
@@ -337,17 +376,17 @@
     return allocated_premiums
 
 
 def get_hospital_claim_filter(ceiling_interpretation, mode='I', prefix=''):
     # return the filter base on cieling interpretation and mode (I inpatient, O outpatient),
     # prefix is required if the queryset is not about claims
     if ceiling_interpretation == Product.CEILING_INTERPRETATION_HOSPITAL:
-        Qterm = (Q(('%shealth_facility_level' % prefix,HealthFacility.LEVEL_HOSPITAL)))
+        Qterm = (Q(('%shealth_facility_level' % prefix, HealthFacility.LEVEL_HOSPITAL)))
     else:
-        Qterm = (Q('%sdate_to__isnull' % prefix,False) & Q('%sdate_to__gt' % prefix,F('date_from')))
+        Qterm = (Q('%sdate_to__isnull' % prefix, False) & Q('%sdate_to__gt' % prefix, F('date_from')))
     if mode == 'I':
         return Qterm
     elif mode == 'O':
         return ~Qterm
     else:
         return Q()
```

### Comparing `openimis-be-claim_batch-1.5.1/claim_batch/test_helpers.py` & `openimis-be-claim_batch-1.5.2/claim_batch/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.5.1/claim_batch/tests.py` & `openimis-be-claim_batch-1.5.2/claim_batch/tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-claim_batch-1.5.1/claim_batch/views.py` & `openimis-be-claim_batch-1.5.2/claim_batch/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from django.core.exceptions import PermissionDenied
+
+from core.jwt_authentication import JWTAuthentication
 from report.services import ReportService
 from .services import ReportDataService
 from .reports import pbh, pbp, pbc_H, pbc_P
 from .apps import ClaimBatchConfig
 from django.utils.translation import gettext as _
 
 
@@ -18,19 +20,20 @@
     else:
         report = "claim_batch_pbp"
         default = pbp.template
     return report, default
 
 
 def report(request):
-    if not request.user.has_perms(ClaimBatchConfig.account_preview_perms):
+    user = JWTAuthentication().authenticate(request)[0]
+    if not user.has_perms(ClaimBatchConfig.account_preview_perms):
         raise PermissionDenied(_("unauthorized"))
-    report_service = ReportService(request.user)
+    report_service = ReportService(user)
     report, default = _report(request.GET)
-    report_data_service = ReportDataService(request.user)
+    report_data_service = ReportDataService(user)
     data = report_data_service.fetch(request.GET)
     return report_service.process(report,
                                   {'data': data,
                                    'DateFrom': request.GET['dateFrom'],
                                    'DateTo': request.GET['dateTo'],
                                    'RegionCode': request.GET['regionCode'],
                                    'RegionName': request.GET['regionName'],
```

### Comparing `openimis-be-claim_batch-1.5.1/openimis_be_claim_batch.egg-info/PKG-INFO` & `openimis-be-claim_batch-1.5.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openimis-be-claim-batch
-Version: 1.5.1
+Name: openimis-be-claim_batch
+Version: 1.5.2
 Summary: The openIMIS Backend Claim Batch reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-claim_batch-1.5.1/openimis_be_claim_batch.egg-info/SOURCES.txt` & `openimis-be-claim_batch-1.5.2/openimis_be_claim_batch.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 claim_batch/urls.py
 claim_batch/views.py
 claim_batch/migrations/0001_initial.py
 claim_batch/migrations/0002_capitationpayment.py
 claim_batch/migrations/0003_capitationpayment_for_legacy_batch_runs.py
 claim_batch/migrations/0004_delete_capitationpayment.py
 claim_batch/migrations/0005_capitationpayment.py
+claim_batch/migrations/0006_capitationpayment.py
+claim_batch/migrations/0007_update_django_scheme_with_missing_fields.py
+claim_batch/migrations/0008_set_managed_to_true.py
 claim_batch/migrations/__init__.py
 claim_batch/reports/__init__.py
 claim_batch/reports/pbc_H.py
 claim_batch/reports/pbc_P.py
 claim_batch/reports/pbh.py
 claim_batch/reports/pbp.py
 openimis_be_claim_batch.egg-info/PKG-INFO
```

### Comparing `openimis-be-claim_batch-1.5.1/setup.py` & `openimis-be-claim_batch-1.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-claim_batch',
-    version='1.5.1',
+    version='v1.5.2',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Claim Batch reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

