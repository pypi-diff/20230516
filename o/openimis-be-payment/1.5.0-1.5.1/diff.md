# Comparing `tmp/openimis-be-payment-1.5.0.tar.gz` & `tmp/openimis-be-payment-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-payment-1.5.0.tar", last modified: Thu Nov 10 18:10:01 2022, max compression
+gzip compressed data, was "openimis-be-payment-1.5.1.tar", last modified: Tue May 16 21:38:20 2023, max compression
```

## Comparing `openimis-be-payment-1.5.0.tar` & `openimis-be-payment-1.5.1.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:10:01.477568 openimis-be-payment-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-11-10 18:10:01.477568 openimis-be-payment-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:10:01.477568 openimis-be-payment-1.5.0/openimis_be_payment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-11-10 18:10:01.000000 openimis-be-payment-1.5.0/openimis_be_payment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-11-10 18:10:01.000000 openimis-be-payment-1.5.0/openimis_be_payment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 18:10:01.000000 openimis-be-payment-1.5.0/openimis_be_payment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-10 18:10:01.000000 openimis-be-payment-1.5.0/openimis_be_payment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-10 18:10:01.000000 openimis-be-payment-1.5.0/openimis_be_payment.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:10:01.477568 openimis-be-payment-1.5.0/payment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     6239 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3155 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:10:01.477568 openimis-be-payment-1.5.0/payment/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     5643 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/migrations/0002_incorrect_name.py
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/migrations/0003_auto_20220401_1149.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5966 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4785 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    17177 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/services.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1723 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    13877 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-10 18:09:49.000000 openimis-be-payment-1.5.0/payment/views.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 18:10:01.477568 openimis-be-payment-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-11-10 18:10:00.000000 openimis-be-payment-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:20.095719 openimis-be-payment-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-16 21:38:20.095719 openimis-be-payment-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:20.095719 openimis-be-payment-1.5.1/openimis_be_payment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-16 21:38:20.000000 openimis-be-payment-1.5.1/openimis_be_payment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-16 21:38:20.000000 openimis-be-payment-1.5.1/openimis_be_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:38:20.000000 openimis-be-payment-1.5.1/openimis_be_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:20.000000 openimis-be-payment-1.5.1/openimis_be_payment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 21:38:20.000000 openimis-be-payment-1.5.1/openimis_be_payment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:20.095719 openimis-be-payment-1.5.1/payment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:20.095719 openimis-be-payment-1.5.1/payment/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/migrations/0002_incorrect_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/migrations/0003_auto_20220401_1149.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/migrations/0004_update_django_scheme_with_missing_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/migrations/0005_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17305 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:07.000000 openimis-be-payment-1.5.1/payment/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:38:20.095719 openimis-be-payment-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-16 21:38:18.000000 openimis-be-payment-1.5.1/setup.py
```

### Comparing `openimis-be-payment-1.5.0/LICENSE.md` & `openimis-be-payment-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.5.0/PKG-INFO` & `openimis-be-payment-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-payment
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Payment reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-payment-1.5.0/README.md` & `openimis-be-payment-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.5.0/openimis_be_payment.egg-info/PKG-INFO` & `openimis-be-payment-1.5.1/openimis_be_payment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-payment
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Payment reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-payment-1.5.0/openimis_be_payment.egg-info/SOURCES.txt` & `openimis-be-payment-1.5.1/openimis_be_payment.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,8 +19,10 @@
 payment/test_helpers.py
 payment/tests.py
 payment/urls.py
 payment/views.py
 payment/migrations/0001_initial.py
 payment/migrations/0002_incorrect_name.py
 payment/migrations/0003_auto_20220401_1149.py
+payment/migrations/0004_update_django_scheme_with_missing_fields.py
+payment/migrations/0005_set_managed_to_true.py
 payment/migrations/__init__.py
```

### Comparing `openimis-be-payment-1.5.0/payment/apps.py` & `openimis-be-payment-1.5.1/payment/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.5.0/payment/gql_mutations.py` & `openimis-be-payment-1.5.1/payment/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.5.0/payment/gql_queries.py` & `openimis-be-payment-1.5.1/payment/gql_queries.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import graphene
 from graphene_django import DjangoObjectType
+
+from .apps import PaymentConfig
 from .models import Payment, PaymentDetail, PaymentMutation
 from core import prefix_filterset, ExtendedConnection
+from django.utils.translation import gettext as _
+from django.core.exceptions import PermissionDenied
 
 
 from contribution.schema import PremiumGQLType
 
 
 class PaymentGQLType(DjangoObjectType):
     client_mutation_id = graphene.String()
@@ -35,14 +39,16 @@
             "type_of_payment": ["exact", "istartswith", "icontains", "iexact", "isnull"],
             "reconc_req_id": ["exact", "istartswith", "icontains", "iexact", "isnull"],
             "reconciliation_date": ["exact", "lt", "lte", "gt", "gte", "isnull"]
         }
         connection_class = ExtendedConnection
 
     def resolve_client_mutation_id(self, info):
+        if not info.context.user.has_perms(PaymentConfig.gql_query_payments_perms):
+            raise PermissionDenied(_("unauthorized"))
         payment_mutation = self.mutations.select_related(
             'mutation').filter(mutation__status=0).first()
         return payment_mutation.mutation.client_mutation_id if payment_mutation else None
 
 
 class PaymentDetailGQLType(DjangoObjectType):
     class Meta:
```

### Comparing `openimis-be-payment-1.5.0/payment/migrations/0001_initial.py` & `openimis-be-payment-1.5.1/payment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.5.0/payment/migrations/0002_incorrect_name.py` & `openimis-be-payment-1.5.1/payment/migrations/0002_incorrect_name.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.5.0/payment/migrations/0003_auto_20220401_1149.py` & `openimis-be-payment-1.5.1/payment/migrations/0003_auto_20220401_1149.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.5.0/payment/models.py` & `openimis-be-payment-1.5.1/payment/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         db_column='ReconciliationDate', null=True, blank=True)
 
     # rowid = models.TextField(db_column='RowID')
     # auditED, not audit ???
     # auditeduser_id = models.IntegerField(db_column='AuditedUSerID', blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblPayment'
 
     def __str__(self):
         return f"id:{self.id}, expected_amount: {self.expected_amount}, status:{self.status}, " \
                f"type:{self.type_of_payment}, uuid:{self.uuid}"
 
 
@@ -113,15 +113,15 @@
 
     # rowid = models.TextField(db_column='RowID', blank=True, null=True)  # Field name made lowercase. This field type is a guess.
     # ! auditED in field name
     audit_user_id = models.IntegerField(
         db_column='AuditedUserId', blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblPaymentDetails'
 
     def __str__(self):
         return f"id:{self.id}, payment:{self.payment_id}, ins_nb:{self.insurance_number}, amount:{self.amount}, " \
                f"premium:{self.premium_id}"
```

### Comparing `openimis-be-payment-1.5.0/payment/schema.py` & `openimis-be-payment-1.5.1/payment/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     payments_by_premiums = OrderedDjangoFilterConnectionField(
         PaymentGQLType,
         premium_uuids=graphene.List(graphene.String, required=True),
         orderBy=graphene.List(of_type=graphene.String),
     )
 
     def resolve_payments(self, info, **kwargs):
+        if not info.context.user.has_perms(PaymentConfig.gql_query_payments_perms):
+            raise PermissionDenied(_("unauthorized"))
         filters = []
         # OFS-257: Create dynamic filters for the payment mutation
         additional_filter = kwargs.get('additional_filter', None)
         # go to process additional filter only when this arg of filter was passed into query
         if additional_filter:
             filters_from_signal = _get_additional_filter(
                 sender=self, additional_filter=additional_filter, user=info.context.user
```

### Comparing `openimis-be-payment-1.5.0/payment/services.py` & `openimis-be-payment-1.5.1/payment/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,18 @@
         """
         cur.execute(sql, (payment_id, audit_user_id,))
 
         if cur.description is None:  # 0 is considered as 'no result' by pyodbc
             res = None
         else:
             info = cur.fetchall()  # FETCH 'SELECT @ret' returned value
+            cur.nextset()
+            feedback = cur.fetchall()
             logger.info("matchPayment result: %s", info)
+            logger.info("matchPayment logs: %s", str(feedback))
         if cur.nextset() and cur.description:
             res = cur.fetchone()[0]
         if res:
             raise Exception(res)
 
 
 def match_payment(payment_id=None, payment=None, audit_user_id=None):
```

### Comparing `openimis-be-payment-1.5.0/payment/test_helpers.py` & `openimis-be-payment-1.5.1/payment/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.5.0/payment/tests.py` & `openimis-be-payment-1.5.1/payment/tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payment-1.5.0/setup.py` & `openimis-be-payment-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-payment',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Payment reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

