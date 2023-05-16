# Comparing `tmp/openimis-be-medical_pricelist-1.5.0.tar.gz` & `tmp/openimis-be-medical_pricelist-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-medical_pricelist-1.5.0.tar", last modified: Thu Nov 10 18:09:22 2022, max compression
+gzip compressed data, was "openimis-be-medical_pricelist-1.5.1.tar", last modified: Tue May 16 21:37:56 2023, max compression
```

## Comparing `openimis-be-medical_pricelist-1.5.0.tar` & `openimis-be-medical_pricelist-1.5.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:22.469909 openimis-be-medical_pricelist-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-11-10 18:09:22.465909 openimis-be-medical_pricelist-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:22.465909 openimis-be-medical_pricelist-1.5.0/medical_pricelist/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/medical_pricelist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/medical_pricelist/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3506 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/medical_pricelist/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)    10725 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/medical_pricelist/gql_mutations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:22.465909 openimis-be-medical_pricelist-1.5.0/medical_pricelist/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3691 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/medical_pricelist/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/medical_pricelist/migrations/0002_itemspricelistmutation_servicespricelistmutation.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/medical_pricelist/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4776 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/medical_pricelist/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     7632 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/medical_pricelist/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/medical_pricelist/services.py
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/medical_pricelist/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/medical_pricelist/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/medical_pricelist/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-10 18:09:13.000000 openimis-be-medical_pricelist-1.5.0/medical_pricelist/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:22.465909 openimis-be-medical_pricelist-1.5.0/openimis_be_medical_pricelist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-11-10 18:09:22.000000 openimis-be-medical_pricelist-1.5.0/openimis_be_medical_pricelist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-11-10 18:09:22.000000 openimis-be-medical_pricelist-1.5.0/openimis_be_medical_pricelist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 18:09:22.000000 openimis-be-medical_pricelist-1.5.0/openimis_be_medical_pricelist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-11-10 18:09:22.000000 openimis-be-medical_pricelist-1.5.0/openimis_be_medical_pricelist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-10 18:09:22.000000 openimis-be-medical_pricelist-1.5.0/openimis_be_medical_pricelist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 18:09:22.469909 openimis-be-medical_pricelist-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-11-10 18:09:21.000000 openimis-be-medical_pricelist-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:56.502879 openimis-be-medical_pricelist-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-16 21:37:56.502879 openimis-be-medical_pricelist-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:56.502879 openimis-be-medical_pricelist-1.5.1/medical_pricelist/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/gql_mutations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:56.502879 openimis-be-medical_pricelist-1.5.1/medical_pricelist/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/migrations/0002_itemspricelistmutation_servicespricelistmutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/migrations/0003_update_django_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/migrations/0004_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 21:37:45.000000 openimis-be-medical_pricelist-1.5.1/medical_pricelist/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:56.502879 openimis-be-medical_pricelist-1.5.1/openimis_be_medical_pricelist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-16 21:37:56.000000 openimis-be-medical_pricelist-1.5.1/openimis_be_medical_pricelist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-16 21:37:56.000000 openimis-be-medical_pricelist-1.5.1/openimis_be_medical_pricelist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:37:56.000000 openimis-be-medical_pricelist-1.5.1/openimis_be_medical_pricelist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 21:37:56.000000 openimis-be-medical_pricelist-1.5.1/openimis_be_medical_pricelist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 21:37:56.000000 openimis-be-medical_pricelist-1.5.1/openimis_be_medical_pricelist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:37:56.502879 openimis-be-medical_pricelist-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-16 21:37:55.000000 openimis-be-medical_pricelist-1.5.1/setup.py
```

### Comparing `openimis-be-medical_pricelist-1.5.0/LICENSE.md` & `openimis-be-medical_pricelist-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.5.0/PKG-INFO` & `openimis-be-medical_pricelist-1.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-medical_pricelist
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Medical Pricelist reference module.
 Home-page: https://openimis.org/
 Author: Eric Darchis
 Author-email: edarchis@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-medical_pricelist-1.5.0/README.md` & `openimis-be-medical_pricelist-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.5.0/medical_pricelist/apps.py` & `openimis-be-medical_pricelist-1.5.1/medical_pricelist/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.5.0/medical_pricelist/gql_mutations.py` & `openimis-be-medical_pricelist-1.5.1/medical_pricelist/gql_mutations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+import datetime
 from gettext import gettext as _
 import graphene
+import medical.models
 from core.schema import OpenIMISMutation
 from django.contrib.auth.models import AnonymousUser
 from django.core.exceptions import ValidationError, PermissionDenied
 from .apps import MedicalPricelistConfig
 from .models import (
     ServicesPricelist,
     ServicesPricelistDetail,
     ItemsPricelist,
     ItemsPricelistDetail,
     ServicesPricelistMutation,
     ItemsPricelistMutation,
 )
-from .services import set_pricelist_deleted
+from .services import set_pricelist_deleted, check_unique_name_items_pricelist, check_unique_name_services_pricelist
 from medical.models import Service, Item
 from location.models import Location
 
 
 class DetailPriceOverruleType(graphene.InputObjectType):
     uuid = graphene.UUID(required=True)
     price = graphene.Decimal()
@@ -34,40 +36,57 @@
 class ServicesPricelistInputType(ItemsOrServicesPricelistInputType):
     pass
 
 
 def create_or_update_pricelist(
     data, user, pricelist_model, service_or_item_model, detail_model
 ):
+    incoming_name = data['name']
+    pricelist_uuid = data.pop("uuid", None)
+    current_pricelist = pricelist_model.objects.filter(uuid=pricelist_uuid).first()
+    current_name = current_pricelist.name if current_pricelist else None
+
+    if current_name != incoming_name:
+        if isinstance(current_pricelist, ServicesPricelist):
+            if check_unique_name_services_pricelist(incoming_name):
+                raise ValidationError(
+                    _("mutation.service_name_duplicated"))
+        elif isinstance(current_pricelist, ItemsPricelist):
+            if check_unique_name_items_pricelist(incoming_name):
+                raise ValidationError(
+                    _("mutation.item_name_duplicated"))
+
     client_mutation_id = data.pop("client_mutation_id", None)
     data.pop("client_mutation_label", None)
     price_overrules = data.pop("price_overrules", None)
     added_details = data.pop("added_details", None)
     removed_details = data.pop("removed_details", None)
     if not data["audit_user_id"]:
         data["audit_user_id"] = user.id_for_audit
 
-    pricelist_uuid = data.pop("uuid", None)
     location_uuid = data.pop("location_id", None)
     data["location"] = (
         Location.objects.get(uuid=location_uuid) if location_uuid else None
     )
 
     if pricelist_uuid:
         pricelist = pricelist_model.objects.get(uuid=pricelist_uuid)
+        if pricelist.validity_to:
+            raise ValidationError("User can not edit historical data")
         for (key, value) in data.items():
             setattr(pricelist, key, value)
     else:
         pricelist = pricelist_model.objects.create(**data)
     pricelist.save()
 
     if added_details is not None:
         for uuid in added_details:
             kwargs = {
-                "validity_to": None,  # We want to keep the history of items/services present in a pricelist
+                # We want to keep the history of items/services present in a pricelist
+                "validity_to": None,
                 detail_model.pricelist_field: pricelist,
                 f"{detail_model.model_prefix}__uuid": uuid,
             }
             detail_model.objects.update_or_create(
                 defaults={
                     detail_model.model_prefix: service_or_item_model.objects.get(
                         uuid=uuid
@@ -88,14 +107,18 @@
 
     if price_overrules is not None:
         for overrule in price_overrules:
             detail = pricelist.details.filter(
                 itemsvc__uuid=overrule["uuid"],
                 validity_to=None,
             ).get()
+            # Save history
+            if detail:
+                detail.save_history()
+            detail.validity_from = datetime.datetime.now()
             detail.price_overrule = overrule["price"]
             detail.save()
 
     if client_mutation_id:
         if isinstance(pricelist, ServicesPricelist):
             ServicesPricelistMutation.object_mutated(
                 user,
```

### Comparing `openimis-be-medical_pricelist-1.5.0/medical_pricelist/migrations/0001_initial.py` & `openimis-be-medical_pricelist-1.5.1/medical_pricelist/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.5.0/medical_pricelist/migrations/0002_itemspricelistmutation_servicespricelistmutation.py` & `openimis-be-medical_pricelist-1.5.1/medical_pricelist/migrations/0002_itemspricelistmutation_servicespricelistmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical_pricelist-1.5.0/medical_pricelist/models.py` & `openimis-be-medical_pricelist-1.5.1/medical_pricelist/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     pricelist_date = fields.DateField(db_column='DatePL')
     location = models.ForeignKey("location.Location", db_column="LocationId", blank=True, null=True,
                                  on_delete=models.DO_NOTHING, related_name='+')
     audit_user_id = models.IntegerField(db_column='AuditUserID')
     # row_id = models.BinaryField(db_column='RowID', blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblPLItems'
 
 
 class ItemsOrServicesPricelistDetailManager(models.Manager):
     def filter(self, *args, **kwargs):
         keys = [x for x in kwargs if "itemsvc" in x]
         for key in keys:
@@ -46,30 +46,30 @@
     audit_user_id = models.IntegerField(db_column='AuditUserID')
     # row_id = models.BinaryField(db_column='RowID', blank=True, null=True)
     model_prefix = "item"
     pricelist_field = 'items_pricelist'
     objects = ItemsOrServicesPricelistDetailManager()
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblPLItemsDetail'
 
 
 class ServicesPricelist(VersionedModel):
     id = models.AutoField(db_column='PLServiceID', primary_key=True)
     uuid = models.CharField(db_column='PLServiceUUID', max_length=36, default=uuid.uuid4, unique=True)
     name = models.CharField(db_column='PLServName', max_length=100)
     pricelist_date = fields.DateField(db_column='DatePL')
     location = models.ForeignKey("location.Location", db_column="LocationId", blank=True, null=True,
                                  on_delete=models.DO_NOTHING)
     audit_user_id = models.IntegerField(db_column='AuditUserID')
     # row_id = models.BinaryField(db_column='RowID', blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblPLServices'
 
 
 class ServicesPricelistDetail(VersionedModel, ItemsOrServicesPricelistDetail):
     id = models.AutoField(db_column='PLServiceDetailID', primary_key=True)
     services_pricelist = models.ForeignKey(ServicesPricelist, on_delete=models.CASCADE, db_column="PLServiceID",
                                           related_name='details')
@@ -80,15 +80,15 @@
     # row_id = models.BinaryField(db_column='RowID', blank=True, null=True)
     model_prefix = "service"
     pricelist_field = 'services_pricelist'
 
     objects = ItemsOrServicesPricelistDetailManager()
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblPLServicesDetail'
 
 
 class ItemsPricelistMutation(UUIDModel, ObjectMutation):
     pricelist = models.ForeignKey(ItemsPricelist, models.DO_NOTHING, related_name='mutations')
     mutation = models.ForeignKey(MutationLog, models.DO_NOTHING, related_name='items_pricelists')
```

### Comparing `openimis-be-medical_pricelist-1.5.0/medical_pricelist/schema.py` & `openimis-be-medical_pricelist-1.5.1/medical_pricelist/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import graphene
 from core import prefix_filterset, filter_validity, ExtendedConnection
 from django.core.exceptions import PermissionDenied
 from django.utils.translation import gettext as _
 from graphene_django import DjangoObjectType
 from graphene_django.filter import DjangoFilterConnectionField
 from django.db.models import Q
+from location.models import Location
 from .apps import MedicalPricelistConfig
 from medical.schema import ServiceGQLType
 from .models import (
     ItemsPricelist,
     ItemsPricelistDetail,
     ServicesPricelist,
     ServicesPricelistDetail,
@@ -20,14 +21,15 @@
     CreateItemsPricelistMutation,
     UpdateItemsPricelistMutation,
     DeleteItemsPricelistMutation,
 )
 from location.schema import LocationGQLType
 import graphene_django_optimizer as gql_optimizer
 import logging
+from .services import check_unique_name_items_pricelist, check_unique_name_services_pricelist
 
 logger = logging.getLogger(__file__)
 
 
 ServiceGQLType.fields = ["id", "name"]
 
 
@@ -99,15 +101,16 @@
     items = graphene.List(PriceCompactGQLType)
 
 
 def prices(element, parent, child, element_id, **kwargs):
     list_id = kwargs.get(element_id)
     if list_id is None:
         return []
-    element_list = element.objects.filter(Q(**{parent: list_id}), *filter_validity(**kwargs))
+    element_list = element.objects.filter(
+        Q(**{parent: list_id}), *filter_validity(**kwargs))
     return [
         PriceCompactGQLType(id=getattr(e, child), p=e.price_overrule)
         for e in element_list.all()
     ]
 
 
 class Query(graphene.ObjectType):
@@ -122,14 +125,24 @@
         location_uuid=graphene.String(),
     )
     items_pricelists = DjangoFilterConnectionField(
         ItemsPricelistGQLType,
         show_history=graphene.Boolean(),
         location_uuid=graphene.String(),
     )
+    validate_items_pricelist_name = graphene.Field(
+        graphene.Boolean,
+        items_pricelist_name=graphene.String(required=True),
+        description="Checks that the specified items pricelist name is unique."
+    )
+    validate_services_pricelist_name = graphene.Field(
+        graphene.Boolean,
+        services_pricelist_name=graphene.String(required=True),
+        description="Checks that the specified services pricelist name is unique."
+    )
 
     def resolve_pricelists(self, info, services_pricelist_id=None, items_pricelist_id=None, **kwargs):
         # When the caller requests a list of pricelists, they're filtered downstream. When they request a specific PL,
         # and don't have the right to browse all pricelists, we need to verify that they do have access to that PL
         if info.context.user.is_anonymous:
             raise PermissionDenied(_("unauthorized"))
         if services_pricelist_id or items_pricelist_id:
@@ -168,42 +181,69 @@
         ):
             raise PermissionDenied(_("unauthorized"))
         filters = []
         show_history = kwargs.get("show_history", False)
         if not show_history:
             filters = [*filter_validity(**kwargs)]
 
-        location_uuid = kwargs.get("location__uuid")
+        location_uuid = kwargs.get("location_uuid")
         if location_uuid is not None:
+            parent_location = Location.objects.filter(uuid=location_uuid).first().parent
             filters += [
                 Q(location__uuid=location_uuid)
-                | Q(location__parent__uuid=location_uuid)
+                | Q(location=parent_location)
+                | Q(location=None)
             ]
         query = ServicesPricelist.objects.filter(*filters).order_by("name")
+
+        # Filter according to the user location
+        query = query.filter(
+            Location.build_user_location_filter_query(info.context.user._u))
+
         return gql_optimizer.query(query.all(), info)
 
     def resolve_items_pricelists(self, info, **kwargs):
         if not info.context.user.has_perms(
             MedicalPricelistConfig.gql_query_pricelists_medical_items_perms
         ):
             raise PermissionDenied(_("unauthorized"))
         filters = []
         show_history = kwargs.get("show_history", False)
         if not show_history:
             filters = [*filter_validity(**kwargs)]
 
-        location_uuid = kwargs.get("location__uuid")
+        location_uuid = kwargs.get("location_uuid")
         if location_uuid is not None:
+            parent_location = Location.objects.filter(uuid=location_uuid).first().parent
             filters += [
                 Q(location__uuid=location_uuid)
-                | Q(location__parent__uuid=location_uuid)
+                | Q(location=parent_location)
+                | Q(location=None)
             ]
+
         query = ItemsPricelist.objects.filter(*filters).order_by("name")
+
+        # Filter according to the user location
+        query = query.filter(
+            Location.build_user_location_filter_query(info.context.user._u))
+
         return gql_optimizer.query(query.all(), info)
 
+    def resolve_validate_services_pricelist_name(self, info, **kwargs):
+        if not info.context.user.has_perms(MedicalPricelistConfig.gql_query_pricelists_medical_services_perms):
+            raise PermissionDenied(_("unauthorized"))
+        errors = check_unique_name_services_pricelist(name=kwargs['services_pricelist_name'])
+        return False if errors else True
+
+    def resolve_validate_items_pricelist_name(self, info, **kwargs):
+        if not info.context.user.has_perms(MedicalPricelistConfig.gql_query_pricelists_medical_items_perms):
+            raise PermissionDenied(_("unauthorized"))
+        errors = check_unique_name_items_pricelist(name=kwargs['items_pricelist_name'])
+        return False if errors else True
+
 
 class Mutation(graphene.ObjectType):
     create_services_pricelist = CreateServicesPricelistMutation.Field()
     update_services_pricelist = UpdateServicesPricelistMutation.Field()
     delete_services_pricelist = DeleteServicesPricelistMutation.Field()
 
     create_items_pricelist = CreateItemsPricelistMutation.Field()
```

### Comparing `openimis-be-medical_pricelist-1.5.0/medical_pricelist/services.py` & `openimis-be-medical_pricelist-1.5.1/medical_pricelist/services.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from gettext import gettext as _
+from .models import ServicesPricelist, ItemsPricelist
 
 
 def set_pricelist_deleted(pricelist):
     """
     Marks a price list as deleted
     :param pricelist: the object to mark as deleted
     :return: an empty array is everything goes well, an array with errors if any
@@ -19,7 +20,19 @@
                         f"pricelist.mutation.failed_to_delete_{pricelist.model_prefix}"
                     )
                     % {"uuid": pricelist.uuid},
                     "detail": pricelist.uuid,
                 }
             ],
         }
+
+
+def check_unique_name_services_pricelist(name):
+    if ServicesPricelist.objects.filter(name=name, validity_to__isnull=True).exists():
+        return [{"message": "Services pricelist name %s already exists" % name}]
+    return []
+
+
+def check_unique_name_items_pricelist(name):
+    if ItemsPricelist.objects.filter(name=name, validity_to__isnull=True).exists():
+        return [{"message": "Items pricelist name %s already exists" % name}]
+    return []
```

### Comparing `openimis-be-medical_pricelist-1.5.0/medical_pricelist/test_helpers.py` & `openimis-be-medical_pricelist-1.5.1/medical_pricelist/test_helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,40 @@
 from location.models import HealthFacility
-from medical_pricelist.models import ServicesPricelistDetail, ItemsPricelistDetail
+from medical_pricelist.models import (
+    ItemsPricelist,
+    ServicesPricelist,
+    ServicesPricelistDetail,
+    ItemsPricelistDetail
+)
+
+
+def create_test_item_pricelist(location_id, custom_props={}):
+    return ItemsPricelist.objects.create(
+        **{
+            "name": "test-item-price-list",
+            "location_id": location_id,
+            "pricelist_date": "2019-01-01",
+            "validity_from": "2019-01-01",
+            "audit_user_id": -1,
+            **custom_props
+        }
+    )
+
+
+def create_test_service_pricelist(location_id, custom_props={}):
+    return ServicesPricelist.objects.create(
+        **{
+            "name": "test-item-price-list",
+            "location_id": location_id,
+            "pricelist_date": "2019-01-01",
+            "validity_from": "2019-01-01",
+            "audit_user_id": -1,
+            **custom_props
+        }
+    )
 
 
 def add_service_to_hf_pricelist(service, hf_id=18, custom_props={}):
     hf = HealthFacility.objects.get(pk=hf_id)
     return ServicesPricelistDetail.objects.create(
         **{
             "services_pricelist": hf.services_pricelist,
```

### Comparing `openimis-be-medical_pricelist-1.5.0/openimis_be_medical_pricelist.egg-info/SOURCES.txt` & `openimis-be-medical_pricelist-1.5.1/openimis_be_medical_pricelist.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,13 +11,15 @@
 medical_pricelist/services.py
 medical_pricelist/test_helpers.py
 medical_pricelist/tests.py
 medical_pricelist/urls.py
 medical_pricelist/views.py
 medical_pricelist/migrations/0001_initial.py
 medical_pricelist/migrations/0002_itemspricelistmutation_servicespricelistmutation.py
+medical_pricelist/migrations/0003_update_django_scheme.py
+medical_pricelist/migrations/0004_set_managed_to_true.py
 medical_pricelist/migrations/__init__.py
 openimis_be_medical_pricelist.egg-info/PKG-INFO
 openimis_be_medical_pricelist.egg-info/SOURCES.txt
 openimis_be_medical_pricelist.egg-info/dependency_links.txt
 openimis_be_medical_pricelist.egg-info/requires.txt
 openimis_be_medical_pricelist.egg-info/top_level.txt
```

### Comparing `openimis-be-medical_pricelist-1.5.0/setup.py` & `openimis-be-medical_pricelist-1.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-medical_pricelist',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Medical Pricelist reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Eric Darchis',
```

