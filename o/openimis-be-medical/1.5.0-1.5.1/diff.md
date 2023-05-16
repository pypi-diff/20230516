# Comparing `tmp/openimis-be-medical-1.5.0.tar.gz` & `tmp/openimis-be-medical-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-medical-1.5.0.tar", last modified: Thu Nov 10 18:09:20 2022, max compression
+gzip compressed data, was "openimis-be-medical-1.5.1.tar", last modified: Tue May 16 21:37:50 2023, max compression
```

## Comparing `openimis-be-medical-1.5.0.tar` & `openimis-be-medical-1.5.1.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:20.316590 openimis-be-medical-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-11-10 18:09:20.312590 openimis-be-medical-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1761 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:20.312590 openimis-be-medical-1.5.0/medical/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/medical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/medical/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2221 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/medical/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)    10488 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/medical/gql_mutations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:20.312590 openimis-be-medical-1.5.0/medical/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3375 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/medical/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/medical/migrations/0002_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/medical/migrations/0003_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/medical/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6939 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/medical/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     7592 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/medical/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/medical/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/medical/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    17780 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/medical/tests_api.py
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/medical/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-10 18:09:11.000000 openimis-be-medical-1.5.0/medical/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:20.312590 openimis-be-medical-1.5.0/openimis_be_medical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-11-10 18:09:20.000000 openimis-be-medical-1.5.0/openimis_be_medical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-11-10 18:09:20.000000 openimis-be-medical-1.5.0/openimis_be_medical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 18:09:20.000000 openimis-be-medical-1.5.0/openimis_be_medical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-10 18:09:20.000000 openimis-be-medical-1.5.0/openimis_be_medical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-10 18:09:20.000000 openimis-be-medical-1.5.0/openimis_be_medical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 18:09:20.316590 openimis-be-medical-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-11-10 18:09:19.000000 openimis-be-medical-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:50.673645 openimis-be-medical-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-16 21:37:50.673645 openimis-be-medical-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:50.673645 openimis-be-medical-1.5.1/medical/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/gql_mutations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:50.673645 openimis-be-medical-1.5.1/medical/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/migrations/0002_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/migrations/0003_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/migrations/0004_add_missing_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/migrations/0005_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17780 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/tests_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 21:37:40.000000 openimis-be-medical-1.5.1/medical/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:50.673645 openimis-be-medical-1.5.1/openimis_be_medical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-16 21:37:50.000000 openimis-be-medical-1.5.1/openimis_be_medical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-16 21:37:50.000000 openimis-be-medical-1.5.1/openimis_be_medical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:37:50.000000 openimis-be-medical-1.5.1/openimis_be_medical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 21:37:50.000000 openimis-be-medical-1.5.1/openimis_be_medical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 21:37:50.000000 openimis-be-medical-1.5.1/openimis_be_medical.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:37:50.673645 openimis-be-medical-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-16 21:37:49.000000 openimis-be-medical-1.5.1/setup.py
```

### Comparing `openimis-be-medical-1.5.0/LICENSE.md` & `openimis-be-medical-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.5.0/PKG-INFO` & `openimis-be-medical-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-medical
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Medical reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-medical-1.5.0/README.md` & `openimis-be-medical-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.5.0/medical/apps.py` & `openimis-be-medical-1.5.1/medical/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.5.0/medical/gql_mutations.py` & `openimis-be-medical-1.5.1/medical/gql_mutations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import functools
 from gettext import gettext as _
 from operator import or_
 
+import django.db.models.base
 import graphene
 from core import assert_string_length, PATIENT_CATEGORY_MASK_ADULT, PATIENT_CATEGORY_MASK_MALE, \
     PATIENT_CATEGORY_MASK_MINOR, PATIENT_CATEGORY_MASK_FEMALE
 from core.schema import OpenIMISMutation
+from medical.exceptions import CodeAlreadyExistsError
 from django.contrib.auth.models import AnonymousUser
 from django.core.exceptions import ValidationError, PermissionDenied
 from medical.apps import MedicalConfig
 from medical.models import Service, ServiceMutation, Item, ItemMutation
 from medical.services import set_item_or_service_deleted
 
 
@@ -116,28 +118,43 @@
 def update_or_create_item_or_service(data, user, item_service_model):
     client_mutation_id = data.pop('client_mutation_id', None)
     data.pop('client_mutation_label', None)
     item_service_uuid = data.pop('uuid') if 'uuid' in data else None
     # update_or_create(uuid=service_uuid, ...)
     # doesn't work because of explicit attempt to set null to uuid!
     data["audit_user_id"] = user.id_for_audit
+
+    incoming_code = data.get('code')
+    item_service = item_service_model.objects.filter(uuid=item_service_uuid).first()
+    current_code = item_service.code if item_service else None
+    if current_code != incoming_code:
+        check_if_code_already_exists(data, item_service_model)
+
     if item_service_uuid:
-        item_service = item_service_model.objects.get(uuid=item_service_uuid)
         reset_item_or_service_before_update(item_service)
         [setattr(item_service, key, data[key]) for key in data]
     else:
         item_service = item_service_model.objects.create(**data)
+
     item_service.save()
     if client_mutation_id:
         if isinstance(item_service, Service):
             ServiceMutation.object_mutated(user, client_mutation_id=client_mutation_id, service=item_service)
         elif isinstance(item_service, Item):
             ItemMutation.object_mutated(user, client_mutation_id=client_mutation_id, item=item_service)
 
 
+def check_if_code_already_exists(
+        data: dict,
+        item_service_model: django.db.models.base.ModelBase
+):
+    if item_service_model.objects.all().filter(code=data['code'], validity_to__isnull=True).exists():
+        raise CodeAlreadyExistsError(_("Code already exists."))
+
+
 class CreateOrUpdateItemOrServiceMutation(OpenIMISMutation):
     @classmethod
     def do_mutate(cls, perms, user, **data):
         if type(user) is AnonymousUser or not user.id:
             raise ValidationError(
                 _("mutation.authentication_required"))
         if not user.has_perms(perms):
@@ -220,15 +237,15 @@
             errors += set_item_or_service_deleted(service, "service")
         if len(errors) == 1:
             errors = errors[0]['list']
         return errors
 
 
 class ItemInputType(ItemOrServiceInputType):
-    package = graphene.String(required=True)
+    package = graphene.String()
     quantity = graphene.Decimal()
 
 
 class CreateItemMutation(CreateOrUpdateItemOrServiceMutation):
     _mutation_module = "medical"
     _mutation_class = "CreateItemMutation"
     item_service_model = Item
```

### Comparing `openimis-be-medical-1.5.0/medical/migrations/0001_initial.py` & `openimis-be-medical-1.5.1/medical/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.5.0/medical/migrations/0002_diagnosis.py` & `openimis-be-medical-1.5.1/medical/migrations/0002_diagnosis.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.5.0/medical/migrations/0003_mutations.py` & `openimis-be-medical-1.5.1/medical/migrations/0003_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.5.0/medical/schema.py` & `openimis-be-medical-1.5.1/medical/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from graphene_django.filter import DjangoFilterConnectionField
 from medical.gql_mutations import CreateServiceMutation, UpdateServiceMutation, DeleteServiceMutation, \
     CreateItemMutation, UpdateItemMutation, DeleteItemMutation
 
 from .apps import MedicalConfig
 from .models import Diagnosis, Item, Service
 import graphene_django_optimizer as gql_optimizer
+from .services import check_unique_code_item, check_unique_code_service
 
 
 class DiagnosisGQLType(DjangoObjectType):
     class Meta:
         model = Diagnosis
         interfaces = (graphene.relay.Node,)
         filter_fields = {
@@ -87,14 +88,24 @@
     medical_services_str = OrderedDjangoFilterConnectionField(
         ServiceGQLType,
         str=graphene.String(),
         date=graphene.Date(),
         orderBy=graphene.List(of_type=graphene.String),
         pricelist_uuid=graphene.UUID(),
     )
+    validate_item_code = graphene.Field(
+        graphene.Boolean,
+        item_code=graphene.String(required=True),
+        description="Checks that the specified item code is unique."
+    )
+    validate_service_code = graphene.Field(
+        graphene.Boolean,
+        service_code=graphene.String(required=True),
+        description="Checks that the specified service code is unique."
+    )
 
     def resolve_diagnoses_str(self, info, **kwargs):
         if not info.context.user.has_perms(MedicalConfig.gql_query_diagnosis_perms):
             raise PermissionDenied(_("unauthorized"))
         search_str = kwargs.get('str')
         if search_str is not None:
             return Diagnosis.objects \
@@ -107,15 +118,16 @@
         # OMT-281 allow listing of medical services even if the query right is not given
         # if not info.context.user.has_perms(MedicalConfig.gql_query_medical_items_perms):
         if info.context.user.is_anonymous:
             raise PermissionDenied(_("unauthorized"))
         search_str = kwargs.get("str")
         q = Item.objects.filter(*filter_validity(date))
         if pricelist_uuid is not None:
-            q = q.filter(pricelist_details__items_pricelist__uuid=pricelist_uuid)
+            q = q.filter(pricelist_details__items_pricelist__uuid=pricelist_uuid,
+                         pricelist_details__validity_to__isnull=True)
         if search_str is not None:
             q = q.filter(Q(code__icontains=search_str) | Q(name__icontains=search_str))
         return q
 
     def resolve_medical_items(
         self,
         info,
@@ -150,15 +162,16 @@
         # OMT-281 allow listing of medical services even if the query right is not given
         # if not info.context.user.has_perms(MedicalConfig.gql_query_medical_services_perms):
         if info.context.user.is_anonymous:
             raise PermissionDenied(_("unauthorized"))
         search_str = kwargs.get("str")
         q = Service.objects.filter(*filter_validity(date))
         if pricelist_uuid is not None:
-            q = q.filter(pricelist_details__services_pricelist__uuid=pricelist_uuid)
+            q = q.filter(pricelist_details__services_pricelist__uuid=pricelist_uuid,
+                         pricelist_details__validity_to__isnull=True)
         if search_str is not None:
             q = q.filter(Q(code__icontains=search_str) | Q(name__icontains=search_str))
         return q
 
     def resolve_medical_services(
         self,
         info,
@@ -182,14 +195,26 @@
             queryset = queryset.filter(
                 mutations__mutation__client_mutation_id=client_mutation_id
             )
         if not show_history:
             queryset = queryset.filter(*filter_validity(**kwargs))
         return gql_optimizer.query(queryset, info)
 
+    def resolve_validate_service_code(self, info, **kwargs):
+        if not info.context.user.has_perms(MedicalConfig.gql_query_medical_services_perms):
+            raise PermissionDenied(_("unauthorized"))
+        errors = check_unique_code_service(code=kwargs['service_code'])
+        return False if errors else True
+
+    def resolve_validate_item_code(self, info, **kwargs):
+        if not info.context.user.has_perms(MedicalConfig.gql_query_medical_items_perms):
+            raise PermissionDenied(_("unauthorized"))
+        errors = check_unique_code_item(code=kwargs['item_code'])
+        return False if errors else True
+
 
 class Mutation(graphene.ObjectType):
     create_service = CreateServiceMutation.Field()
     update_service = UpdateServiceMutation.Field()
     delete_service = DeleteServiceMutation.Field()
     create_item = CreateItemMutation.Field()
     update_item = UpdateItemMutation.Field()
```

### Comparing `openimis-be-medical-1.5.0/medical/test_helpers.py` & `openimis-be-medical-1.5.1/medical/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.5.0/medical/tests_api.py` & `openimis-be-medical-1.5.1/medical/tests_api.py`

 * *Files identical despite different names*

### Comparing `openimis-be-medical-1.5.0/openimis_be_medical.egg-info/PKG-INFO` & `openimis-be-medical-1.5.1/openimis_be_medical.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-medical
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Medical reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-medical-1.5.0/setup.py` & `openimis-be-medical-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-medical',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Medical reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

