# Comparing `tmp/openimis-be-contribution-1.5.0.tar.gz` & `tmp/openimis-be-contribution-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-contribution-1.5.0.tar", last modified: Thu Nov 10 18:09:51 2022, max compression
+gzip compressed data, was "openimis-be-contribution-1.5.1.tar", last modified: Tue May 16 21:38:17 2023, max compression
```

## Comparing `openimis-be-contribution-1.5.0.tar` & `openimis-be-contribution-1.5.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:51.726690 openimis-be-contribution-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-11-10 18:09:51.726690 openimis-be-contribution-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:51.722690 openimis-be-contribution-1.5.0/contribution/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/contribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/contribution/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/contribution/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     7670 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/contribution/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/contribution/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:51.722690 openimis-be-contribution-1.5.0/contribution/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/contribution/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/contribution/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2173 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/contribution/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3492 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/contribution/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     7833 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/contribution/services.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/contribution/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/contribution/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/contribution/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-10 18:09:36.000000 openimis-be-contribution-1.5.0/contribution/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:51.722690 openimis-be-contribution-1.5.0/openimis_be_contribution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-11-10 18:09:51.000000 openimis-be-contribution-1.5.0/openimis_be_contribution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-11-10 18:09:51.000000 openimis-be-contribution-1.5.0/openimis_be_contribution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 18:09:51.000000 openimis-be-contribution-1.5.0/openimis_be_contribution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-11-10 18:09:51.000000 openimis-be-contribution-1.5.0/openimis_be_contribution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-10 18:09:51.000000 openimis-be-contribution-1.5.0/openimis_be_contribution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 18:09:51.726690 openimis-be-contribution-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-11-10 18:09:50.000000 openimis-be-contribution-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:17.054045 openimis-be-contribution-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-16 21:38:17.054045 openimis-be-contribution-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:17.050045 openimis-be-contribution-1.5.1/contribution/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:17.050045 openimis-be-contribution-1.5.1/contribution/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/migrations/0002_add_premium_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/migrations/0003_alter_premium_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 21:38:04.000000 openimis-be-contribution-1.5.1/contribution/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:17.054045 openimis-be-contribution-1.5.1/openimis_be_contribution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-16 21:38:16.000000 openimis-be-contribution-1.5.1/openimis_be_contribution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-16 21:38:17.000000 openimis-be-contribution-1.5.1/openimis_be_contribution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:38:16.000000 openimis-be-contribution-1.5.1/openimis_be_contribution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-16 21:38:16.000000 openimis-be-contribution-1.5.1/openimis_be_contribution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 21:38:16.000000 openimis-be-contribution-1.5.1/openimis_be_contribution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:38:17.054045 openimis-be-contribution-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-16 21:38:14.000000 openimis-be-contribution-1.5.1/setup.py
```

### Comparing `openimis-be-contribution-1.5.0/LICENSE.md` & `openimis-be-contribution-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.5.0/PKG-INFO` & `openimis-be-contribution-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-contribution
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Policy reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-contribution-1.5.0/README.md` & `openimis-be-contribution-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.5.0/contribution/apps.py` & `openimis-be-contribution-1.5.1/contribution/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.5.0/contribution/gql_mutations.py` & `openimis-be-contribution-1.5.1/contribution/gql_mutations.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from payer.models import Payer
 from policy import models as policy_models
 from core.schema import OpenIMISMutation
 from django.contrib.auth.models import AnonymousUser
 from django.core.exceptions import PermissionDenied, ValidationError
 from django.utils.translation import gettext as _
 from core import datetime
+from .services import check_unique_premium_receipt_code_within_product
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class PremiumBase:
     """
@@ -44,14 +45,26 @@
     premium.pay_type = None
     premium.is_photo_fee = None
     premium.is_offline = None
     premium.reporting_id = None
 
 
 def update_or_create_premium(data, user):
+    uuid = data.pop('uuid', None)
+    if uuid:
+        incoming_premium_receipt = data['receipt']
+        current_premium_receipt = Premium.objects.get(uuid=uuid).receipt
+        if current_premium_receipt != incoming_premium_receipt:
+            if check_unique_premium_receipt_code_within_product(code=data['receipt'], policy_uuid=data['policy_uuid']):
+                raise ValidationError(
+                    _("mutation.code_already_taken"))
+    else:
+        if check_unique_premium_receipt_code_within_product(code=data['receipt'], policy_uuid=data['policy_uuid']):
+            raise ValidationError(
+                _("mutation.code_already_taken"))
     if "client_mutation_id" in data:
         data.pop('client_mutation_id')
     if "client_mutation_label" in data:
         data.pop('client_mutation_label')
     now = datetime.datetime.now()
     data['audit_user_id'] = user.id_for_audit
     data['validity_from'] = now
```

### Comparing `openimis-be-contribution-1.5.0/contribution/gql_queries.py` & `openimis-be-contribution-1.5.1/contribution/gql_queries.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import graphene
 from graphene_django import DjangoObjectType
+
+from .apps import ContributionConfig
 from .models import Premium, PremiumMutation
 from core import prefix_filterset, ExtendedConnection
 from policy.schema import PolicyGQLType
+from django.core.exceptions import PermissionDenied
+from django.utils.translation import gettext as _
 
 
 class PremiumGQLType(DjangoObjectType):
     client_mutation_id = graphene.String()
 
     class Meta:
         model = Premium
@@ -19,14 +23,16 @@
             "is_photo_fee": ["exact"],
             "receipt": ["exact", "icontains"],
             **prefix_filterset("policy__", PolicyGQLType._meta.filter_fields)
         }
         connection_class = ExtendedConnection
 
     def resolve_client_mutation_id(self, info):
+        if not info.context.user.has_perms(ContributionConfig.gql_query_premiums_perms):
+            raise PermissionDenied(_("unauthorized"))
         premium_mutation = self.mutations.select_related(
             'mutation').filter(mutation__status=0).first()
         return premium_mutation.mutation.client_mutation_id if premium_mutation else None
 
 
 class PremiumMutationGQLType(DjangoObjectType):
     class Meta:
```

### Comparing `openimis-be-contribution-1.5.0/contribution/migrations/0001_initial.py` & `openimis-be-contribution-1.5.1/contribution/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.5.0/contribution/models.py` & `openimis-be-contribution-1.5.1/contribution/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import uuid
 
 from core import fields
 from core import models as core_models
 from django.db import models
 from django.utils.translation import gettext_lazy
+
+from core.datetimes.ad_datetime import datetime
 from policy.models import Policy
 from payer.models import Payer
 
 
 class PayTypeChoices(models.TextChoices):
     BANK_TRANSFER = "B", gettext_lazy("Bank transfer")
     CASH = "C", gettext_lazy("Cash")
@@ -41,18 +43,19 @@
         db_column="isPhotoFee", blank=True, null=True, default=False
     )
     is_offline = models.BooleanField(
         db_column="isOffline", blank=True, null=True, default=False
     )
     reporting_id = models.IntegerField(db_column="ReportingId", blank=True, null=True)
     audit_user_id = models.IntegerField(db_column="AuditUserID")
+    created_date = models.DateTimeField(db_column="CreatedDate", default=datetime.now)
     # rowid = models.TextField(db_column='RowID', blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblPremium'
 
 
 class PremiumMutation(core_models.UUIDModel, core_models.ObjectMutation):
     premium = models.ForeignKey(Premium, models.DO_NOTHING, related_name='mutations')
     mutation = models.ForeignKey(core_models.MutationLog, models.DO_NOTHING, related_name='premiums')
```

### Comparing `openimis-be-contribution-1.5.0/contribution/schema.py` & `openimis-be-contribution-1.5.1/contribution/schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .apps import ContributionConfig
 from location.apps import LocationConfig
 from django.utils.translation import gettext as _
 from core.schema import signal_mutation_module_before_mutating, OrderedDjangoFilterConnectionField, filter_validity
 # We do need all queries and mutations in the namespace here.
 from .gql_queries import *  # lgtm [py/polluting-import]
 from .gql_mutations import *  # lgtm [py/polluting-import]
+from .services import check_unique_premium_receipt_code_within_product
 
 
 class Query(graphene.ObjectType):
     premiums = OrderedDjangoFilterConnectionField(
         PremiumGQLType,
         client_mutation_id=graphene.String(),
         show_history=graphene.Boolean(),
@@ -20,14 +21,20 @@
         orderBy=graphene.List(of_type=graphene.String),
     )
     premiums_by_policies = OrderedDjangoFilterConnectionField(
         PremiumGQLType,
         policy_uuids=graphene.List(graphene.String, required=True),
         orderBy=graphene.List(of_type=graphene.String),
     )
+    validate_premium_code = graphene.Field(
+        graphene.Boolean,
+        code=graphene.String(required=True),
+        policy_uuid=graphene.String(required=True),
+        description="Checks that the specified premium code is unique for a given policy."
+    )
 
     def resolve_premiums(self, info, **kwargs):
         if not info.context.user.has_perms(ContributionConfig.gql_query_premiums_perms):
             raise PermissionDenied(_("unauthorized"))
         filters = []
         client_mutation_id = kwargs.get("client_mutation_id", None)
         if client_mutation_id:
@@ -49,14 +56,21 @@
 
     def resolve_premiums_by_policies(self, info, **kwargs):
         if not info.context.user.has_perms(ContributionConfig.gql_query_premiums_perms):
             raise PermissionDenied(_("unauthorized"))
         policies = policy_models.Policy.objects.values_list('id').filter(Q(uuid__in=kwargs.get('policy_uuids')))
         return Premium.objects.filter(Q(policy_id__in=policies), *filter_validity(**kwargs))
 
+    def resolve_validate_premium_code(self, info, **kwargs):
+        if not info.context.user.has_perms(ContributionConfig.gql_query_premiums_perms):
+            raise PermissionDenied(_("unauthorized"))
+        errors = check_unique_premium_receipt_code_within_product(code=kwargs['code'],
+                                                                  policy_uuid=kwargs['policy_uuid'])
+        return False if errors else True
+
 
 def set_premium_deleted(premium):
     try:
         premium.delete_history()
         return []
     except Exception as exc:
         return {
```

### Comparing `openimis-be-contribution-1.5.0/contribution/services.py` & `openimis-be-contribution-1.5.1/contribution/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,7 +243,17 @@
     )
 
 
 def _activate_insurees(policy, pay_date):
     policy.insuree_policies.filter(validity_to__isnull=True).update(
         effective_date=pay_date,
     )
+
+
+def check_unique_premium_receipt_code_within_product(code, policy_uuid):
+    from .models import Premium
+
+    policy = Policy.objects.select_related('product').filter(uuid=policy_uuid, validity_to__isnull=True).first()
+    exists = Premium.objects.filter(policy__product=policy.product, receipt=code, validity_to__isnull=True).exists()
+    if exists:
+        return [{"message": "Premium code %s already exists" % code}]
+    return []
```

### Comparing `openimis-be-contribution-1.5.0/contribution/test_helpers.py` & `openimis-be-contribution-1.5.1/contribution/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-contribution-1.5.0/openimis_be_contribution.egg-info/PKG-INFO` & `openimis-be-contribution-1.5.1/openimis_be_contribution.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-contribution
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Policy reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-contribution-1.5.0/openimis_be_contribution.egg-info/SOURCES.txt` & `openimis-be-contribution-1.5.1/openimis_be_contribution.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,13 +11,15 @@
 contribution/schema.py
 contribution/services.py
 contribution/test_helpers.py
 contribution/tests.py
 contribution/urls.py
 contribution/views.py
 contribution/migrations/0001_initial.py
+contribution/migrations/0002_add_premium_fields.py
+contribution/migrations/0003_alter_premium_options.py
 contribution/migrations/__init__.py
 openimis_be_contribution.egg-info/PKG-INFO
 openimis_be_contribution.egg-info/SOURCES.txt
 openimis_be_contribution.egg-info/dependency_links.txt
 openimis_be_contribution.egg-info/requires.txt
 openimis_be_contribution.egg-info/top_level.txt
```

### Comparing `openimis-be-contribution-1.5.0/setup.py` & `openimis-be-contribution-1.5.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-contribution',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Policy reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

